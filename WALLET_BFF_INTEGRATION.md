# Wallet BFF — Integration Guide (KYC + Card Platform)

**Status:** Active  
**Last updated:** 2026-06-30  
**Audience:** Wallet BFF engineers  
**Staging tenant:** `wallet-stage`  
**Staging KYC profile:** `wallet-stage`

Complete reference for integrating the wallet BFF with **lira-kyc** and **lira-card-platform**: base URLs, authentication, every tenant-facing API with payloads, card platform B2B APIs, trusted internal routes, and inbound webhooks.

Related: [TENANT_INTEGRATION_CONTRACT.md](./TENANT_INTEGRATION_CONTRACT.md), `neivan-stageing/docs/wallet-stage-seeding.md`

---

## Part 1 — Base URLs (staging)

KYC is a **standalone service** on its own path (not under `/card-platform/`).

| Service | Staging base URL | Notes |
|---------|------------------|-------|
| **KYC API** | `https://stg.niwan.net/kyc/api` | HAProxy strips `/kyc/api/` prefix |
| **Card platform API** | `https://stg.niwan.net/card-platform/api` | HAProxy strips `/card-platform/api/` |
| **Card platform admin UI** | `https://stg.niwan.net/card-platform/` | Next.js `basePath=/card-platform` |
| **Shahkar** (BFF registration) | `https://stg.niwan.net/gateway/api/gateway/shahkar/matching` | Via Neivan gateway |

**Legacy:** `https://stg.niwan.net/card-platform/kyc/api/*` → **301** → `/kyc/api/*`

**Docker internal (same host):**

| From | To |
|------|-----|
| Platform → KYC | `http://lira-kyc-api:8080` |
| KYC → Platform | `http://card-platform-api:8080` |

### Wallet BFF env (staging)

```bash
KYC_BASE_URL=https://stg.niwan.net/kyc/api
KYC_TENANT_SLUG=wallet-stage
KYC_PROFILE_SLUG=wallet-stage
KYC_API_KEY=lkyckey_wallet_stage_staging_001

CARD_PLATFORM_BASE_URL=https://stg.niwan.net/card-platform/api
CARD_PLATFORM_API_KEY=lcpkey_wallet_stage_staging_001
CARD_PLATFORM_INTERNAL_TOKEN=<shared APP_INTERNAL_SERVICE_TOKEN>
CARD_PLATFORM_WEBHOOK_SECRET=<webhook secret>
```

Append `/v1/...` to base URLs in client code.

---

## Part 2 — Authentication

### KYC tenant API (`/v1/kyc/*`)

| Header | Required | Value |
|--------|----------|-------|
| `Authorization` | Yes | `Bearer <kyc-api-key>` |
| `X-Tenant-Slug` | Yes | `wallet-stage` |
| `X-User-Ref` | Yes | Stable opaque user id (e.g. your user UUID string) |
| `Content-Type` | POST | `application/json` |

**API key scopes** (seed keys get all):

| Scope | Routes |
|-------|--------|
| `kyc:read:progress` | GET progress, gate |
| `kyc:write:steps` | OTP, identity verify, upload |
| `kyc:read:bundle` | GET bundle |
| `kyc:write:review` | POST step decision |
| `kyc:write:reset` | POST submission reset |
| `kyc:write:external-rejection` | POST external rejection |

### Card platform B2B (`/v1/*`)

| Header | Required on | Value |
|--------|-------------|-------|
| `X-Api-Key` | All B2B routes | Card platform tenant API key |
| `X-User-Ref` | User-scoped routes | Same `userRef` as KYC |
| `Idempotency-Key` | `POST /fulfillments`, `POST /cards/:id/operations` | Unique per create |
| `Content-Type` | POST | `application/json` |

### Card platform internal (trusted BFF)

| Header | Value |
|--------|-------|
| `Authorization` | `Bearer <CARD_PLATFORM_INTERNAL_TOKEN>` |

Used for post-payment fulfillment start. **Never expose this token to the PWA.**

### Error envelopes

**KYC** (flat):

```json
{ "code": "VALIDATION_FAILED", "message": "..." }
```

**Card platform B2B** (wrapped):

```json
{ "success": false, "error": { "code": "KYC_GATE_BLOCKED", "message": "..." } }
```

**Card platform internal** (flat):

```json
{ "code": "VALIDATION_FAILED", "message": "..." }
```

---

## Part 3 — KYC tenant API (`lira-kyc`)

All paths relative to `{KYC_BASE_URL}` e.g. `https://stg.niwan.net/kyc/api`.

**Common query:** `?profile=wallet-stage` (optional — defaults to tenant default profile)

### Health (no auth)

| Method | Path | Response 200 |
|--------|------|--------------|
| GET | `/health` | `{"status":"ok"}` |
| GET | `/livez` | `{"status":"ok"}` |
| GET | `/readyz` | `{"status":"ok","checks":{"postgres":"ok","redis":"ok"}}` or **503** |

---

### GET `/v1/kyc/progress`

**Scope:** `kyc:read:progress`

**Response 200:**

```json
{
  "profileId": "wallet-stage",
  "profileVersion": 1,
  "defaultGate": "onboarding",
  "steps": [
    {
      "key": "email_otp",
      "type": "otp_email",
      "required": true,
      "status": "pending",
      "reviewNote": "",
      "showNoteToUser": false,
      "reuploadRequired": false
    },
    {
      "key": "phone_otp",
      "type": "otp_phone",
      "required": true,
      "status": "pending",
      "reviewNote": "",
      "showNoteToUser": false,
      "reuploadRequired": false
    }
  ],
  "gates": {
    "onboarding": {
      "gateId": "onboarding",
      "allowed": false,
      "profileId": "wallet-stage",
      "profileVersion": 1,
      "missingSteps": [
        { "key": "email_otp", "type": "otp_email", "reason": "not_accepted" }
      ]
    }
  },
  "gate": {
    "gateId": "onboarding",
    "allowed": false,
    "profileId": "wallet-stage",
    "profileVersion": 1,
    "missingSteps": []
  }
}
```

**Step statuses:** `pending`, `submitted`, `under_review`, `accepted`, `rejected`, `skipped`

---

### GET `/v1/kyc/gate`

**Scope:** `kyc:read:progress`  
**Query:** `profile`, `gate` (default: profile's `defaultGate` → `onboarding` for wallet-stage)

**Response 200:**

```json
{
  "gateId": "onboarding",
  "allowed": false,
  "profileId": "wallet-stage",
  "profileVersion": 1,
  "missingSteps": [
    { "key": "email_otp", "type": "otp_email", "reason": "not_accepted" }
  ]
}
```

**400** `KYC_GATE_NOT_FOUND` if unknown gate.

---

### POST `/v1/kyc/steps/:stepKey/otp/send`

**Scope:** `kyc:write:steps`

**Request (email_otp):**

```json
{ "email": "user@example.com" }
```

**Request (phone_otp):**

```json
{ "phone": "+989361234567" }
```

**Response 200:**

```json
{
  "expiresAt": "2026-07-01T12:05:00Z",
  "resendAvailableAt": "2026-07-01T12:06:00Z",
  "otp": "123456"
}
```

`otp` field only when KYC `debug=true` (never in production).

**429** resend cooldown; **502** delivery failure.

---

### POST `/v1/kyc/steps/:stepKey/otp/verify`

**Scope:** `kyc:write:steps`

**Request:**

```json
{ "otp": "123456" }
```

**Response 200:**

```json
{ "status": "ok" }
```

---

### POST `/v1/kyc/steps/:stepKey/identity/verify`

**Scope:** `kyc:write:steps`  
**Not used in wallet-stage profile** (Shahkar runs in BFF). Documented for other profiles.

**Request:**

```json
{ "nationalCode": "3660743224", "mobileNumber": "09361234567" }
```

**Response 200:**

```json
{ "stepKey": "shahkar_match", "status": "accepted", "matched": true }
```

**422** `KYC_IDENTITY_NOT_MATCHED`

---

### POST `/v1/kyc/steps/:stepKey/upload/presign`

**Scope:** `kyc:write:steps`  
**Not used in wallet-stage v1** (no document steps).

**Request:**

```json
{ "contentType": "application/pdf" }
```

**Response 200:**

```json
{
  "stepKey": "contract",
  "objectKey": "wallet-stage/user/contract/uuid.pdf",
  "uploadUrl": "https://s3.niwan.net/...",
  "expiresAt": "2026-07-01T12:15:00Z",
  "contentType": "application/pdf"
}
```

---

### POST `/v1/kyc/steps/:stepKey/upload/confirm`

**Scope:** `kyc:write:steps`

**Request:**

```json
{
  "objectKey": "wallet-stage/user/contract/uuid.pdf",
  "contentType": "application/pdf",
  "byteSize": 102400
}
```

**Response 200:** `{ "status": "ok" }`

---

### GET `/v1/kyc/bundle`

**Scope:** `kyc:read:bundle`  
**Query:** `profile`, `gate` (e.g. `card_issuance` for card programs)

**Not needed for wallet-stage onboarding-only flow.** Platform worker uses internal bundle API for issuance.

**Response 200:**

```json
{
  "profileId": "wallet-stage",
  "profileVersion": 1,
  "gateId": "card_issuance",
  "userRef": "user-uuid",
  "documents": [
    {
      "stepKey": "contract",
      "docType": "contract",
      "contentType": "application/pdf",
      "downloadUrl": "https://...",
      "expiresAt": "2026-07-01T12:00:00Z"
    }
  ]
}
```

---

### POST `/v1/kyc/steps/:stepKey/decision`

**Scope:** `kyc:write:review`  
**Tenant reviewer API** — wallet BFF typically does not call this; ops use admin UI.

**Request:**

```json
{ "accept": true, "reviewNote": "", "showNoteToUser": false }
```

**Response 200:** `{ "status": "ok" }`

---

### POST `/v1/kyc/submissions/reset`

**Scope:** `kyc:write:reset`

**Request (optional):**

```json
{ "mode": "reset_all" }
```

**Response 200:**

```json
{ "mode": "reset_all", "resetSteps": ["email_otp", "phone_otp"] }
```

---

### POST `/v1/kyc/submissions/external-rejection`

**Scope:** `kyc:write:external-rejection`

**Request:**

```json
{ "note": "external provider rejected" }
```

**Response 200:**

```json
{ "mode": "reset_all", "rejectedSteps": ["email_otp"] }
```

---

## Part 4 — Card platform B2B API (`lira-card-platform`)

All paths relative to `{CARD_PLATFORM_BASE_URL}` e.g. `https://stg.niwan.net/card-platform/api`.

Success responses: `{ "success": true, "data": <payload> }`

### Programs (API key only — no `X-User-Ref`)

#### GET `/v1/programs`

**Response `data`:**

```json
{
  "items": [
    {
      "slug": "mock-usd-config-1",
      "name": "Mock USD Standard",
      "provider": "mock-twocards",
      "currency": "USD",
      "status": "active",
      "availability": { "type": "on_demand", "inStock": true, "availableCount": null },
      "capabilities": ["top_up", "add_pin"],
      "kyc": { "profileSlug": "wallet-stage" }
    }
  ]
}
```

#### GET `/v1/programs/:slug`

**Response `data`:** program detail + `kyc.gate` (e.g. `card_issuance`).

#### GET `/v1/programs/:slug/eligibility`

**Query or header:** `userRef` / `X-User-Ref` required.

**Eligible `data`:**

```json
{
  "eligible": true,
  "program": { "slug": "...", "name": "...", "kyc": { "profileSlug": "wallet-stage", "gate": "card_issuance" } },
  "blockers": []
}
```

**403** when blocked: `error.code` = `KYC_GATE_BLOCKED`, `INSUFFICIENT_POOL_STOCK`, etc.

---

### Fulfillments (`X-Api-Key` + `X-User-Ref`)

#### POST `/v1/fulfillments`

**Headers:** `Idempotency-Key` required (stored as `externalPaymentRef`).

**Request:**

```json
{ "programSlug": "mock-usd-config-1" }
```

**Response 202 `data`:**

```json
{
  "id": "fulfillment-uuid",
  "tenantId": "tenant-uuid",
  "userRef": "user-uuid",
  "programSlug": "mock-usd-config-1",
  "externalPaymentRef": "your-idempotency-key",
  "status": "queued",
  "failure": null,
  "cardId": null,
  "createdAt": "2026-07-01T12:00:00Z",
  "updatedAt": "2026-07-01T12:00:00Z"
}
```

**Statuses:** `queued`, `submitted`, `polling`, `succeeded`, `failed`, `kyc_required`, `cancelled`

#### GET `/v1/fulfillments/:id`

**Response 200:** same fulfillment `View`.

---

### Cards (`X-Api-Key` + `X-User-Ref`)

#### GET `/v1/cards`

**Query:** `limit` (optional)

**Response `data`:**

```json
{
  "items": [
    {
      "id": "card-uuid",
      "userRef": "user-uuid",
      "programSlug": "mock-usd-config-1",
      "status": "active",
      "display": { "last4": "4242", "expiryMonth": 12, "expiryYear": 2028, "brand": "visa" },
      "balance": { "amount": "100.00", "currency": "USD" },
      "issuedAt": "2026-07-01T12:00:00Z"
    }
  ]
}
```

#### GET `/v1/cards/:id`

**Response 200:** single card view.

---

### Card operations (`X-Api-Key` + `X-User-Ref` + `Idempotency-Key` on POST)

#### POST `/v1/cards/:id/operations`

**Request:**

```json
{
  "type": "top_up",
  "amount": "50.00",
  "currency": "USD",
  "newPin": "",
  "oldPin": ""
}
```

**Types:** `top_up` | `add_pin` | `change_pin`

**Response 202 `data`:**

```json
{
  "id": "op-uuid",
  "cardId": "card-uuid",
  "userRef": "user-uuid",
  "type": "top_up",
  "status": "queued",
  "amount": "50.00",
  "currency": "USD",
  "failureCode": "",
  "failureMessage": "",
  "createdAt": "...",
  "updatedAt": "..."
}
```

#### GET `/v1/cards/:id/operations/:operationId`

**Response 200:** operation view.

---

### Card onboarding (`X-Api-Key` + `X-User-Ref`)

#### GET `/v1/cards/:id/onboarding`

**Response `data`:**

```json
{
  "phase": "set_pin",
  "complete": false,
  "steps": [
    { "key": "set_pin", "type": "set_credentials", "status": "required" }
  ],
  "capabilities": ["top_up"],
  "blockedCapabilities": ["top_up"]
}
```

#### POST `/v1/cards/:id/onboarding/steps/:key/submit`

**set_credentials:** `{ "newPin": "1234" }`  
**document_upload:** `{ "objectKey": "...", "contentType": "image/jpeg" }`

#### POST `/v1/cards/:id/onboarding/steps/:key/acknowledge`

No body (user_acknowledgment steps).

#### GET `/v1/onboarding-content/:contentKey`

**Query:** `locale` (default `en`) — API key only.

---

## Part 5 — Card platform internal API (trusted BFF)

Base: `{CARD_PLATFORM_BASE_URL}` — paths are **not** under `/v1/`.

### POST `/internal/v1/fulfillments/start`

**Use after payment confirmed** (preferred over B2B POST when BFF holds internal token).

**Request:**

```json
{
  "tenantId": "platform-tenant-uuid",
  "userRef": "user-uuid",
  "programSlug": "mock-usd-config-1",
  "externalPaymentRef": "invoice-uuid-or-payment-id"
}
```

**Response 202:**

```json
{ "fulfillmentId": "ful-uuid", "status": "queued" }
```

**Note:** This path does not run eligibility at HTTP layer — BFF must verify KYC gate before calling.

### POST `/internal/v1/platform/tenant-events`

KYC → platform relay only (not called by wallet BFF).

---

## Part 6 — Inbound webhooks (card platform → wallet BFF)

### BFF route

| Item | Value |
|------|-------|
| **Method** | `POST` |
| **Path** | `/v1/internal/card-platform/webhooks` |
| **Staging URL** | `https://stg.niwan.net/wallet/api/v1/internal/card-platform/webhooks` |
| **Auth** | HMAC `X-Lira-Signature` — not user JWT |

Configure in platform admin:

```
PUT /v1/admin/tenants/{tenantId}/card-webhook
{ "url": "...", "secret": "..." }
```

### Request format

**Headers:**

| Header | Value |
|--------|-------|
| `Content-Type` | `application/json` |
| `X-Lira-Signature` | `sha256=<lowercase-hex-hmac>` |

**Body envelope:**

```json
{
  "id": "550e8400-e29b-41d4-a716-446655440000",
  "type": "kyc.gate.opened",
  "occurredAt": "2026-06-30T12:00:00Z",
  "tenantSlug": "wallet-stage",
  "userRef": "user-uuid",
  "data": {}
}
```

**BFF response:** HTTP **2xx** within 15s. Platform retries up to **8** times (~2s apart) on failure.

### Signature verification (required)

```
MAC = HMAC-SHA256(key = cardWebhookSecret, message = raw_request_body_bytes)
X-Lira-Signature = "sha256=" + lowercase_hex(MAC)
```

```go
func verifyLiraSignature(secret string, body []byte, header string) bool {
    mac := hmac.New(sha256.New, []byte(strings.TrimSpace(secret)))
    mac.Write(body)
    expected := "sha256=" + hex.EncodeToString(mac.Sum(nil))
    return hmac.Equal([]byte(expected), []byte(strings.TrimSpace(header)))
}
```

- Use **raw body bytes** before JSON parse.
- Reject missing/invalid signature with **401**.
- Compare with **constant-time** equality.

### Idempotency (required)

1. **Dedupe on `event.id`** — store seen IDs; ignore duplicates.
2. **Version guard** — for events with `data.resourceVersion`, only apply if newer than last seen for that resource (`fulfillment:{id}`, `card:{id}`, `operation:{id}`).
3. KYC relay events usually have **no** `resourceVersion` — dedupe on `event.id` only.

### Event catalog

Routing key (AMQP): `tenant.{tenantSlug}.card.{eventType}`

#### KYC relay (`kyc.*`) — **active today**

| Type | When | Key `data` fields |
|------|------|-------------------|
| `kyc.step.submitted` | Step submitted | `profileSlug`, `profileVersion`, `stepKey` |
| `kyc.step.accepted` | Step accepted | same |
| `kyc.step.rejected` | Step rejected | same |
| `kyc.gate.opened` | Gate allowed | + `gateId`, `gateAllowed: true` |
| `kyc.gate.closed` | Gate blocked | + `gateAllowed: false` |
| `kyc.provider_rejected` | Provider rejection | `profileSlug`, `profileVersion` |
| `kyc.external_rejected` | External rejection | same |
| `kyc.submission.reset` | Reset | + `mode` |

**Wallet-stage example:**

```json
{
  "id": "...",
  "type": "kyc.gate.opened",
  "tenantSlug": "wallet-stage",
  "userRef": "user-uuid",
  "data": {
    "profileSlug": "wallet-stage",
    "profileVersion": 1,
    "stepKey": "phone_otp",
    "gateId": "onboarding",
    "gateAllowed": true
  }
}
```

**BFF action:** mark user onboarding complete when `gateId=onboarding` and `gateAllowed=true`.

#### Fulfillment (`fulfillment.*`)

| Type | Emitted today? |
|------|----------------|
| `fulfillment.succeeded` | Yes |
| `fulfillment.failed` | Yes |
| `fulfillment.kyc_required` | Yes |
| `fulfillment.queued`, `submitted`, `polling`, `cancelled` | No (defined, not wired) |

**`data` shape:**

```json
{
  "fulfillmentId": "uuid",
  "programSlug": "mock-usd-config-1",
  "status": "succeeded",
  "resourceVersion": 3,
  "cardId": "uuid"
}
```

#### Card / operation / onboarding events

Defined but **not emitted** yet: `card.created`, `operation.*`, `card.onboarding.*`. Implement handlers that log unknown types.

### Webhook security checklist

- [ ] Route not behind user JWT
- [ ] Secret in env/secrets manager, never in git
- [ ] Constant-time HMAC compare on raw body
- [ ] `event.id` dedupe with unique constraint
- [ ] `resourceVersion` guard for fulfillment/card/operation
- [ ] Return 2xx after durable enqueue
- [ ] Reject wrong `tenantSlug`

---

## Part 7 — Wallet-stage end-to-end flow

```mermaid
sequenceDiagram
  participant App as Wallet PWA
  participant BFF as Wallet BFF
  participant Shahkar as Shahkar
  participant KYC as lira-kyc
  participant CP as card-platform

  App->>BFF: Register (nationalCode, mobile, email)
  BFF->>Shahkar: POST matching
  BFF->>BFF: Create user
  App->>BFF: Login
  BFF->>KYC: POST .../email_otp/send + verify
  BFF->>KYC: POST .../phone_otp/send + verify
  KYC->>CP: Relay kyc.gate.opened
  CP->>BFF: Webhook
  BFF-->>App: Onboarding complete
```

### Example: email OTP via BFF

```http
POST https://stg.niwan.net/kyc/api/v1/kyc/steps/email_otp/otp/send?profile=wallet-stage
Authorization: Bearer lkyckey_wallet_stage_staging_001
X-Tenant-Slug: wallet-stage
X-User-Ref: a1b2c3d4-e5f6-7890-abcd-ef1234567890
Content-Type: application/json

{"email":"user@example.com"}
```

```http
POST https://stg.niwan.net/kyc/api/v1/kyc/steps/email_otp/otp/verify?profile=wallet-stage
...

{"otp":"123456"}
```

Poll gate:

```http
GET https://stg.niwan.net/kyc/api/v1/kyc/gate?profile=wallet-stage&gate=onboarding
...
```

---

## Part 8 — Common error codes

### KYC

| Code | HTTP | Meaning |
|------|------|---------|
| `KYC_UNAUTHORIZED` | 401 | Bad/missing API key |
| `KYC_FORBIDDEN` | 403 | Missing scope |
| `KYC_GATE_NOT_FOUND` | 400 | Unknown gate |
| `KYC_STEP_NOT_FOUND` | 404 | Unknown step |
| `KYC_STEP_LOCKED` | 409 | Step not yet available |
| `VALIDATION_FAILED` | 400 | Bad body |

### Card platform B2B

| Code | HTTP | Meaning |
|------|------|---------|
| `KYC_UNAUTHORIZED` | 401 | Bad API key |
| `KYC_GATE_BLOCKED` | 403 | Eligibility KYC gate |
| `PROGRAM_NOT_FOUND` | 404 | Unknown program |
| `FULFILLMENT_NOT_FOUND` | 404 | Unknown fulfillment |
| `CARD_NOT_FOUND` | 404 | Unknown card |
| `VALIDATION_FAILED` | 400 | Missing header/body |

---

## Part 9 — Deploy notes

After moving KYC to `/kyc/api/`:

1. `make haproxy-reload` on staging host
2. Rebuild card-platform UI if `NEXT_PUBLIC_KYC_API_URL` changed
3. Update wallet BFF `KYC_BASE_URL`
4. Old clients hitting `/card-platform/kyc/api/` get 301 redirect
