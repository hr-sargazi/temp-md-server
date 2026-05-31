# Trawili / Airwallex Integration — Connectivity Incident Report

**Document version:** 1.0  
**Date:** 2026-05-31  
**Prepared by:** Neivan Pay / Lira Platform Engineering  
**Audience:** Internal CTO review · Trawili B2B support · Airwallex integration team  
**Status:** Open — blocking EUR/USD card payments via `trawili_airwallex`

---

## Executive summary

Card payments routed through **Trawili Airwallex** (`trawili_airwallex`) are failing in production with `PAYMENT_PROVIDER_UNAVAILABLE`. Our payment gateway (**neivan-pay**) successfully creates payment intents and resolves the correct provider route, but **outbound HTTPS calls to `https://core.trawili.com` never receive an HTTP response** from our server infrastructure.

Connectivity tests prove:

| Endpoint | IP | Result from our server |
|----------|-----|------------------------|
| `https://core.trawili.com/api/pricing` | `85.95.241.56` | **FAIL** — TLS OK, 0 bytes received, 30s timeout |
| `https://core.trawili.ir/api/pricing` | `87.236.212.243` | **OK** — HTTP 200, JSON pricing returned |

Because the Airwallex rail is configured to use **`core.trawili.com`** (international / `.com` domain), all Airwallex checkout attempts fail regardless of currency. This is an **upstream reachability issue**, not a bug in our payment API request format.

We request Trawili/Airwallex to investigate why `core.trawili.com` accepts TCP/TLS connections from our server but does not return HTTP responses, and to advise on the correct endpoint or IP allowlisting for our deployment region.

---

## Business impact

- **Affected flow:** International card payments (Airwallex) via payment links and plugin checkout  
- **Public API:** `https://pgm.liracards.com/api/v1`  
- **Example failing payment link:** `https://pgm.liracards.com/api/v1/l/6IWOrmNcuapMK2kf`  
- **User-facing error:**
  ```json
  {
    "success": false,
    "code": "PAYMENT_PROVIDER_UNAVAILABLE",
    "message": "payment provider is temporarily unavailable"
  }
  ```
- **Scope:** All payment intents processed through provider key `trawili_airwallex`  
- **Other providers:** Domestic routes (e.g. Zibal) and local discovery APIs continue to work

---

## System architecture (relevant path)

```
Customer browser
    → pgm.liracards.com (HAProxy / neivan-pay API)
        → POST /v1/payment-intents/{id}/process
            → Provider: trawili_airwallex
                → POST https://core.trawili.com/api/v2/generate_factor_airwallex/{public_key}
                    → [TIMEOUT — no HTTP response]
                        → 502 PAYMENT_PROVIDER_UNAVAILABLE
```

**Integration details:**

| Setting | Value |
|---------|-------|
| Provider key | `trawili_airwallex` |
| Trawili COM base URL | `https://core.trawili.com` |
| Trawili IR base URL | `https://core.trawili.ir` |
| Merchant public key | `745983475938475` |
| Callback base URL | `https://pgm.liracards.com/api` |
| Airwallex API path | `/api/v2/generate_factor_airwallex/{public_key}` |

Callback URL format (working as designed):

```
https://pgm.liracards.com/api/v1/providers/trawili_airwallex/callbacks
  ?payment_intent_id={pi_id}
  &tenant_id={tenant_id}
  &app_id={app_id}
```

---

## Symptoms in application logs

Service: `neivan-pay-core` · Build: `20260531T060847Z` · Environment: staging/production on `pgm.liracards.com`

### Typical failure sequence

1. Payment intent created — `POST /v1/payment-intents` → **201**
2. Provider discovery — `GET /v1/discovery/providers?currency=EUR&amount_minor=500` → **200** (local DB only; does not call Trawili)
3. Process intent — provider resolved to `trawili_airwallex`
4. Upstream call to Trawili — **fails after ~15s**

### Representative log lines

```
level=INFO  msg="payment: calling provider authorize"
  payment_intent_id=pi_1780210482132406406
  amount_minor=500 currency=EUR provider_key=trawili_airwallex

level=WARN  msg="provider: upstream http call failed"
  provider=trawili_airwallex operation=create_factor http_method=POST
  url=https://core.trawili.com/api/v2/generate_factor_airwallex/745983475938475
  duration_ms=15012
  error="Post \"https://core.trawili.com/api/v2/generate_factor_airwallex/745983475938475\":
         context deadline exceeded (Client.Timeout exceeded while awaiting headers)"

level=WARN  msg="payment intent process failed"
  http_status=502 error_code=PAYMENT_PROVIDER_UNAVAILABLE
```

### Intermittent HTTP/2 protocol errors (same upstream)

```
level=INFO  msg="protocol error: received *http.http2GoAwayFrame before a SETTINGS frame"

level=WARN  msg="provider: upstream http call failed"
  duration_ms=5125
  error="Post \"https://core.trawili.com/api/v2/generate_factor_airwallex/745983475938475\":
         connection error: PROTOCOL_ERROR"
```

### Example request body sent by neivan-pay (verified correct vs. Trawili Postman collection)

```json
{
  "private_key": "<merchant-private-key>",
  "currency": "EUR",
  "value": "5",
  "name": "pi_1780210482132406406",
  "discription": "neivan-pay pi_178021048213240640",
  "call_back": "https://pgm.liracards.com/api/v1/providers/trawili_airwallex/callbacks?payment_intent_id=pi_1780210482132406406&tenant_id=ten_1779884494267305920&app_id=app_1779884653585468523"
}
```

Field notes:

- `value: "5"` is correct for `amount_minor: 500` (€5.00)
- `name` / `discription` truncated to 32 characters (Airwallex descriptor limit)
- `call_back` URL-encoded query parameters are intentional

---

## Connectivity test results (from production server)

Tests executed directly on the same host running `neivan-pay-core` (not from a developer laptop).

### Test 1 — `core.trawili.com` via HTTP/2 (default)

```bash
curl -v --max-time 30 https://core.trawili.com/api/pricing
```

**Result: FAIL**

- TCP connect to `85.95.241.56:443` — success
- TLS 1.3 handshake — success
- Certificate valid (Let's Encrypt, CN=`core.trawili.com`)
- ALPN negotiated: **h2** (HTTP/2)
- Request sent: `GET /api/pricing HTTP/2`
- Response: **0 bytes received**
- Exit: `curl: (28) Operation timed out after 30000 milliseconds with 0 bytes received`

### Test 2 — `core.trawili.com` via HTTP/1.1

```bash
curl -v --http1.1 --max-time 30 https://core.trawili.com/api/pricing
```

**Result: FAIL**

- Same as Test 1 except ALPN negotiated: **http/1.1**
- Request sent: `GET /api/pricing HTTP/1.1`
- Response: **0 bytes received, 30s timeout**

**Conclusion:** Not an HTTP/2-specific issue. The `.com` endpoint is unreachable at the application layer from our server regardless of protocol version.

### Test 3 — Airwallex create-factor endpoint

```bash
curl -v --max-time 30 -X POST -H "Content-Type: application/json" \
  -d '{"private_key":"<key>","currency":"EUR","value":"5","name":"test","discription":"test","call_back":"https://pgm.liracards.com/api/v1/providers/trawili_airwallex/callbacks?payment_intent_id=test"}' \
  https://core.trawili.com/api/v2/generate_factor_airwallex/745983475938475
```

**Result: FAIL**

- TLS handshake — success
- HTTP/2 request fully uploaded
- Response: **0 bytes received, 30s timeout**

This matches neivan-pay behaviour exactly.

### Test 4 — `core.trawili.ir` pricing (control / comparison)

```bash
curl -v --max-time 30 https://core.trawili.ir/api/pricing
```

**Result: SUCCESS**

- TCP connect to `87.236.212.243:443` — success
- TLS 1.3 + HTTP/2 — success
- Response: **HTTP/2 200**
- Body:
  ```json
  {"selling":3788,"buying":3560,"USD_sell":172609,"USD_buy":163350,"EUR_sell":204222,"EUR_buy":186200,"TRY_sell":3788,"TRY_buy":3560}
  ```

**Conclusion:** Outbound HTTPS from our server works in general. Only `core.trawili.com` is affected.

### Test 5 — Server public IP lookup

```bash
curl -s ifconfig.me
```

**Result:** `403 Forbidden` (blocked by ifconfig.me from our network)

> **Action required from our side:** Provide Trawili with our server's outbound public IP via hosting provider (Abrha PaaS / server console). Trawili should confirm whether this IP is blocked, rate-limited, or requires allowlisting.

---

## Cross-network comparison (external verification)

From a network outside our production server, `core.trawili.com` **does respond** (latency ~0.7–2s). This confirms Trawili's service is not globally down; the failure is **specific to the path between our server IP/region and `85.95.241.56`**.

| Test | Network | Endpoint | Result |
|------|---------|----------|--------|
| Pricing | External | `core.trawili.com/api/pricing` | Intermittent (sometimes timeout, sometimes OK) |
| Airwallex + USD | External | `generate_factor_airwallex` | **200 OK** — returns `order_number` + `url_payment` |
| Airwallex + EUR | External | `generate_factor_airwallex` | **200 OK** but `status: 0` — `"currency = null select TRY , USD , EUR"` |
| Moneyro + EUR | External | `generate_factor` | **200 OK** — returns payment URL |

This secondary finding suggests a **separate Trawili API issue**: the Airwallex endpoint may not correctly accept EUR even when reachable. However, this is moot until `.com` connectivity from our server is restored.

---

## Root cause analysis

### Confirmed

1. **neivan-pay integration is functioning correctly** — intent creation, routing, payload construction, and error mapping all behave as designed.
2. **`core.trawili.com` is unreachable from our server** — TLS terminates but no HTTP response is returned within 30 seconds.
3. **`core.trawili.ir` is reachable from the same server** — proves general outbound HTTPS is healthy.
4. **Failure is not HTTP/2-specific** — HTTP/1.1 shows identical timeout behaviour.

### Most likely causes (require Trawili confirmation)

| Hypothesis | Evidence |
|------------|----------|
| **IP / region block or silent drop on `.com` edge** | `.ir` works, `.com` does not, from same host |
| **Trawili `.com` backend unavailable for certain client ASNs** | External networks get responses; our server does not |
| **Firewall / WAF rule on Trawili side** | Connection accepted at TLS layer, request never answered |
| **Routing asymmetry** | Outbound SYN succeeds; return traffic dropped |

### Ruled out

| Hypothesis | Why ruled out |
|------------|---------------|
| Invalid request JSON | Same timeout on simple `GET /api/pricing` |
| Wrong credentials | No HTTP response received to parse |
| neivan-pay bug | Raw `curl` from same host reproduces issue |
| DNS failure | Resolves correctly to `85.95.241.56` |
| TLS / certificate error | Handshake completes successfully |
| Callback URL misconfiguration | Failure occurs before any response |

---

## Questions for Trawili / Airwallex team

Please investigate and respond to the following:

1. **Why does `core.trawili.com` (`85.95.241.56`) accept TLS connections from our server but return zero HTTP bytes?**
2. **Is our server's outbound IP blocked, geo-filtered, or rate-limited on the `.com` infrastructure?**  
   We will provide the exact IP upon request from our hosting provider.
3. **Should merchants deployed in Iran / Middle East use `core.trawili.ir` instead of `core.trawili.com` for Airwallex?**  
   Is `generate_factor_airwallex` available on the `.ir` domain?
4. **Is the Airwallex rail (`/api/v2/generate_factor_airwallex`) intended to support EUR?**  
   When reachable from external networks, EUR requests return `"currency = null"` while USD succeeds on the same endpoint.
5. **Are there known maintenance windows, IP allowlist requirements, or alternate endpoints** we should configure?
6. **Can you provide server-side logs** for requests from our IP to `745983475938475` (public key) around **2026-05-31 06:54–07:03 UTC**?

---

## Information to provide Trawili (on request)

| Item | Value |
|------|-------|
| Merchant public key | `745983475938475` |
| Merchant private key | Available securely on request (not included in this document) |
| Callback URL pattern | `https://pgm.liracards.com/api/v1/providers/trawili_airwallex/callbacks?...` |
| Sample payment intent IDs | `pi_1780210482132406406`, `pi_1780210501184687905`, `pi_1780210943080185746` |
| Tenant ID | `ten_1779884494267305920` |
| App ID | `app_1779884653585468523` |
| Failure window (UTC) | 2026-05-31 06:52 – 07:03 |
| Server outbound IP | **Pending** — retrieve from hosting provider |

---

## Recommended actions

### For Trawili / Airwallex (blocking)

- [ ] Investigate `core.trawili.com` reachability from our server IP/ASN
- [ ] Confirm whether IP allowlisting is required for B2B API access
- [ ] Advise correct base URL for our deployment region (`.com` vs `.ir`)
- [ ] Fix or document EUR support on `generate_factor_airwallex`
- [ ] Share incident reference and ETA for resolution

### For Neivan / Lira platform (internal)

- [ ] Retrieve and share server outbound public IP with Trawili
- [ ] Open formal support ticket with Trawili B2B including this document
- [ ] Pause or hide `trawili_airwallex` in payment link checkout until resolved
- [ ] Evaluate interim routing: EUR → `trawili_moneyro` via `.com` (if/when `.com` connectivity restored) or domestic alternatives
- [ ] After Trawili fix: run end-to-end test with USD and EUR on Airwallex rail
- [ ] Confirm deployed image uses `TRAWILI_HTTP_TIMEOUT_SECONDS=30` (logs showed ~15s timeout on some builds)

### Optional engineering hardening (after upstream fix)

- Force HTTP/1.1 on Trawili client if HTTP/2 instability persists
- Add provider health check that probes `core.trawili.com` before offering Airwallex in discovery
- Restrict `trawili_airwallex` catalog currencies to USD until Trawili confirms EUR support

---

## Timeline

| Time (UTC) | Event |
|------------|-------|
| 2026-05-31 06:52 | Payment link checkout fails — `PAYMENT_PROVIDER_UNAVAILABLE` |
| 2026-05-31 06:54–07:03 | Repeated payment intent failures — all timeout at ~15s on `core.trawili.com` |
| 2026-05-31 06:55 | Intermittent HTTP/2 `PROTOCOL_ERROR` on same endpoint |
| 2026-05-31 07:02 | Failures continue after brief pause |
| 2026-05-31 07:15 | Server-side curl confirms: `.com` timeout, `.ir` OK |

---

## Appendix A — API reference (Trawili B2B Airwallex)

Per Trawili Postman collection (`trawili_B2B.postman_Airwallex.json`):

```
POST https://core.trawili.com/api/v2/generate_factor_airwallex/{{public_key}}
Content-Type: application/json

{
  "private_key": "<merchant-private-key>",
  "currency": "USD",
  "value": "10",
  "name": "order-name",
  "discription": "order description",
  "call_back": "https://merchant.example/callback"
}
```

Expected success response (observed externally with USD):

```json
{
  "order_number": "341793149",
  "url_payment": "https://core.trawili.com/airwallex/341793149"
}
```

---

## Appendix B — neivan-pay error mapping (for reference)

| Upstream condition | neivan-pay error code | HTTP status |
|--------------------|----------------------|-------------|
| Timeout / connection failure | `PAYMENT_PROVIDER_UNAVAILABLE` | 502 |
| Trawili `status: 0` rejection | Provider rejected (different code) | 4xx/502 |
| Missing redirect URL in response | Provider response invalid | 502 |

Current failures map to **`PAYMENT_PROVIDER_UNAVAILABLE`** because no HTTP response is received.

---

## Document history

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2026-05-31 | Neivan Pay Engineering | Initial incident report |

---

*For questions regarding this document, contact the Neivan Pay platform team.*
