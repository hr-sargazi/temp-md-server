# Lira / Neivan — Developer Handbook

Practical guide for working across the platform repos: setup, conventions, adding features, logging, and **debugging without internet** (local-only workflows).

Companion doc: **`architecture-deep-dive.md`** (system structure and design rationale).

---

## 1. Before you start

### 1.1 Repository map

Each project is a **separate Git repo**. Always `cd` into the repo before `git status`, `commit`, or `push`.

```bash
cd /Users/ubank/Documents/lira/<repo-name>
```

| Repo | You need installed | Typical dev command |
|------|-------------------|---------------------|
| `lira-virtual-card` | Go 1.26+, Docker, migrate | `go run ./cmd/api` |
| `neivan-pay` | Go 1.26+, Docker | `go run ./cmd/api` |
| `neivan-api-gateway` | Go 1.24+, Docker | `go run ./cmd` |
| `sunrate-proxy` | Go 1.26+, Docker | `go run ./cmd/server` |
| `sso` | Java 17, Maven | `./mvnw spring-boot:run` |
| `Liravirtualmastercardwebapp` | Node 18+, npm/pnpm | `npm run dev` |
| `neivan-api-gateway-interface` | Node 20+, npm | `npm run dev` |
| `neivan-pay-admin` | Node 22+, npm | `npm run dev` |
| `new-ui` | Node 20+, npm/pnpm | `npm run dev` |
| `sunrate-proxy-ui` | Node 22+, npm | `npm run dev` |
| `neivan-pay-integrations` | PHP 8.0+, Composer | `cd woocommerce && composer install` |
| `neivan-production` / `neivan-stageing` | Docker, make | `make up` (on server) |
| `observability-stack` | Docker, make | `make up` |
| `ingress-manifest` | Docker (for `make check`) | `make assemble` |

### 1.2 Copy env files first

Almost every runnable service has `.env.example` → copy to `.env` and fill secrets locally:

```bash
cp .env.example .env
```

Never commit `.env`. If a secret was committed, rotate it.

### 1.3 Which backend does my UI talk to?

| UI | Env var | Local default | Staging example |
|----|---------|---------------|-----------------|
| Liravirtualmastercardwebapp | `VITE_API_BASE_URL` | `http://127.0.0.1:8080/v1` | `https://stg.niwan.net/virtual/api/v1` |
| neivan-pay-admin | `VITE_API_BASE_URL` | `/v1` (Vite proxy) or `http://localhost:8080/v1` | path under Pay host |
| neivan-api-gateway-interface | `NEXT_PUBLIC_API_BASE_URL` | `http://localhost:8080` | `https://stg.niwan.net/gateway/api` |
| new-ui | `VITE_API_BASE_URL` | sand API in `.env` | varies |
| sunrate-proxy-ui | `VITE_API_URL` | `http://localhost:8080` | via gateway path |

---

## 2. Language requirements and basics

### 2.1 Go (lira-virtual-card, neivan-pay, neivan-api-gateway, sunrate-proxy)

| Topic | Standard in these repos |
|-------|-------------------------|
| Version | 1.24–1.26 per `go.mod` |
| Layout | `cmd/` binaries, `internal/` only (no public `pkg/` except rare cases) |
| HTTP | chi (Lira) or stdlib `ServeMux` 1.22+ (Pay, gateway, sunrate) |
| Logging | **`log/slog`** structured — not `fmt.Println` in production paths |
| Errors | Domain errors + `errors.Is` in mappers; return stable API codes |
| DB | PostgreSQL via pgx or GORM (sunrate); migrations in `migrations/` |
| Tests | `go test ./...`; table-driven tests; `httptest` for handlers |
| Config | `os.Getenv` or Viper (gateway); document in `.env.example` |

**Minimal new handler checklist:**

1. Parse request in `delivery/http*`
2. Call `application` use case
3. Map error to envelope / `error_mapper`
4. Log with `slog.InfoContext` / `ErrorContext` and request ID if available

**Run tests offline:**

```bash
go test ./... -count=1
go test ./internal/application/payment/... -v -run TestName
```

**Race detector (CI-style):**

```bash
go test ./... -race -count=1
```

### 2.2 TypeScript / React (frontends)

| Repo | TS strict? | Router | State |
|------|------------|--------|-------|
| neivan-api-gateway-interface | **yes** (`strict: true`) | Next App Router | hooks + `useApiResource` |
| neivan-pay-admin | **yes** | react-router v7 | hooks + repositories |
| new-ui | **yes** (strict + extra flags) | react-router | Context + TanStack Query |
| sunrate-proxy-ui | **yes** (`tsc -b`) | react-router v7 | AuthContext |
| Liravirtualmastercardwebapp | loose (no root tsconfig) | react-router v7 | Context |

**Rules:**

- **neivan-pay-admin:** no hardcoded UI strings — use `src/i18n/en/*.json` and `fa/*.json`.
- Prefer extending existing `http()` / `client.ts` rather than raw `fetch` scattered in components.
- Match existing component library (shadcn/Radix/Tailwind) in each repo.

**Lint / build offline:**

```bash
npm run lint
npm run build    # catches TS errors in strict repos
npm run test     # neivan-pay-admin (vitest)
```

### 2.3 Java (sso)

| Topic | Standard |
|-------|----------|
| Version | Java 17, Spring Boot 3.0.x |
| Build | `./mvnw clean package` |
| API | `@RestController` → `@Service` → JPA repository |
| DTO mapping | MapStruct in `model/mapper/` |
| Security | `SecurityConfig` — update matchers for new public routes |
| Config | `application.yml` profiles (`dev`, `prod`) |

**Run offline:**

```bash
./mvnw spring-boot:run
# or
./mvnw test
```

### 2.4 PHP (neivan-pay-integrations)

| Topic | Standard |
|-------|----------|
| PHP | **8.0+** (see `docs/compatibility.md`) |
| Architecture | Clean Architecture — UI ≠ business logic |
| SDK | `packages/php-sdk` — test with PHPUnit, **95% line coverage target** |
| Woo | Path repo to SDK via `composer.json` |

```bash
cd packages/php-sdk && composer install && vendor/bin/phpunit
cd woocommerce && composer install
```

---

## 3. Local development recipes

### 3.1 Virtual card stack

**Terminal 1 — API:**

```bash
cd lira-virtual-card
cp .env.example .env
# set DATABASE_URL, REDIS_ADDR, JWT_SECRET, etc.
docker compose up -d postgres redis   # if using compose DB
go run ./cmd/api
```

**Terminal 2 — worker (if testing fulfillment / queues):**

```bash
go run ./cmd/worker
```

**Terminal 3 — user panel:**

```bash
cd Liravirtualmastercardwebapp
cp .env.example .env
# VITE_API_BASE_URL=http://127.0.0.1:8080/v1
npm install && npm run dev
# → http://localhost:5173
```

**Health check:**

```bash
curl -sS http://127.0.0.1:8080/v1/health
curl -sS http://127.0.0.1:8080/v1/ready
```

### 3.2 Neivan Pay stack

```bash
cd neivan-pay
cp .env.example .env
make migrate-up    # or docker migrate per Makefile
go run ./cmd/api
```

**Worker (webhooks / reconcile):**

```bash
go run ./cmd/worker
```

**Admin UI with API proxy (avoids CORS):**

```bash
cd neivan-pay-admin
# .env: VITE_API_BASE_URL=/v1
# vite.config proxies /v1 → PAY_API_PROXY_TARGET=http://localhost:8080
npm run dev
```

**Admin UI fully offline (mock data):**

```bash
# omit VITE_API_BASE_URL — uses MockAdminRepository
npm run dev
```

### 3.3 API Gateway stack

```bash
cd neivan-api-gateway
cp .env.example .env
docker compose up -d   # postgres/redis per README
go run ./cmd
```

```bash
cd neivan-api-gateway-interface
cp .env.example .env
# NEXT_PUBLIC_API_BASE_URL=http://localhost:8080
npm run dev
# → http://localhost:3000
```

**No mock mode** — gateway UI requires a running `neivan-api-gateway`.

### 3.4 Sunrate proxy stack

```bash
cd sunrate-proxy
cp .env.example .env
go run ./cmd/server
```

```bash
cd sunrate-proxy-ui
cp .env.example .env
# VITE_API_URL=http://localhost:8080
npm run dev
```

Enable CORS in proxy env for browser origin. Use **Automation Tests** page for a 21-step live checklist.

### 3.5 SSO

```bash
cd sso
./mvnw spring-boot:run
# default http://localhost:8095
```

Requires local Postgres/Redis per `application.yml` dev profile.

---

## 4. How to add a feature (developer checklist)

### 4.1 Any cross-repo feature

1. Create epic folder: `docs/epics/<name>/` with `analysis.md`, `roadmap.md`, `checklist.md`.
2. Define API contract (JSON shape, error codes, auth) **before** UI polish.
3. Implement backend first if security or money movement is involved.
4. Wire frontend to real API — avoid client-side authority for limits/eligibility/payment state.
5. Record verification steps in `checklist.md`.

### 4.2 Go API endpoint (all Go services)

| Step | Location |
|------|----------|
| 1. Domain model / errors | `internal/domain/` |
| 2. Port interface | `internal/ports/` |
| 3. Use case | `internal/application/<feature>/` |
| 4. Postgres / client adapter | `internal/infrastructure/` |
| 5. HTTP handler | `internal/delivery/http*` |
| 6. Route registration | `router.go` or `server.go` |
| 7. Wire in composition root | `internal/app/` |
| 8. Test | `*_test.go` next to use case and handler |
| 9. Env | `.env.example` + service README |

### 4.3 React / Next screen

| Step | Lira panel | Pay admin | Gateway UI |
|------|------------|-----------|------------|
| Page | `src/app/components/screens/` | `src/presentation/features/` | `src/app/(admin)/admin/.../page.tsx` |
| Route | `src/app/routes.tsx` | `src/presentation/App.tsx` | file-based App Router |
| API call | `src/api/client.ts` | repository + `http-client.ts` | `src/shared/lib/http.ts` |
| i18n | `src/i18n/translations.ts` | `src/i18n/en`, `fa` | `src/shared/i18n/` |

### 4.4 WooCommerce / PHP

1. SDK method in `packages/php-sdk` + tests.
2. Use case in plugin `src/Application/`.
3. Presentation: gateway class or REST controller.
4. Symlink plugin into local WordPress `wp-content/plugins/`.
5. Copy vendored build to `neivan-stageing/services/wc-shop/plugins/` for staging tests.

---

## 5. Logging — how to add and where to read

### 5.1 Go services

**Pattern:** use `log/slog` with context:

```go
slog.InfoContext(ctx, "payment intent created",
    slog.String("intent_id", id),
    slog.String("tenant_id", tenantID),
)
```

**Enable verbose logs:**

| Repo | Env vars |
|------|----------|
| lira-virtual-card | `LOG_LEVEL=debug`, `LOG_FORMAT=json`, `GATEWAY_DEBUG=1`, `WEBHOOK_SIGNATURE_DEBUG=1` |
| neivan-pay | `LOG_LEVEL=debug`, `PAY_HTTP_DEBUG=1`, `WEBHOOK_SIGNATURE_DEBUG=1` |
| neivan-api-gateway | Viper log level in config / README |

**Where logs go:**

| Repo | Destination |
|------|-------------|
| lira-virtual-card | stderr (Docker captures stdout/stderr) |
| neivan-pay | stderr + optional file `LOG_FILE_PATH` (default `logs/neivan-pay.log`) |
| sunrate-proxy | middleware request logging |

**Warning:** `*_HTTP_DEBUG` and `WEBHOOK_SIGNATURE_DEBUG` may log secrets — disable after troubleshooting.

### 5.2 Frontends

| Technique | When |
|-----------|------|
| Browser DevTools → Network | API status, payload shape, CORS |
| `console.log` in dev only | Temporary; remove before merge |
| Vite proxy errors | Pay admin `/v1` proxy mis-target |
| `MOCK_MODE` (Lira panel) | UI-only offline — see `MOCK_MODE_INFO.md` |

### 5.3 SSO (Java)

`application.yml`:

```yaml
logging:
  level:
    com.farda.sso: DEBUG
```

Logback: `src/main/resources/logback-spring.xml`.

Feign debug: package `com.farda.zeepaylogging` (per existing config).

### 5.4 PHP / WordPress

- Woo plugin: `NEIVAN_PAY_WC_DEBUG=1` in `neivan-stageing/services/wc-shop/.env`
- Grep container logs for `neivan-pay-wc`
- WooCommerce → Status → Logs

### 5.5 Production / staging (no IDE)

| Source | Path / command |
|--------|----------------|
| Docker container logs | `docker logs <container> --tail 200 -f` |
| Pay log file (if mounted) | `logs/neivan-pay.log` inside container |
| HAProxy (staging) | `neivan-stageing/infrastructure/haproxy/logs/` |
| Central Loki | Grafana Explore — `{container=~"...`}` on observability host |
| Alloy | `observability-stack/alloy/config.remote-example.alloy` |

---

## 6. Debugging without internet

Use this when CDN, provider sandboxes, or package registries are unreachable.

### 6.1 What still works offline

| Activity | Requirement |
|----------|-------------|
| `go test ./...` | vendored/modules already cached |
| `npm run dev` / `build` | `node_modules` present |
| `./mvnw test` | `.m2` cache populated |
| Docker Compose local DB | images already pulled |
| Pay admin UI | omit `VITE_API_BASE_URL` → mocks |
| Lira panel UI | `MOCK_MODE = true` in `AuthContext.tsx` / `CardsContext.tsx` |
| HAProxy config check | local `haproxy -c` via Docker image |
| Postgres inspection | `docker exec -it shared-postgres psql -U ...` |

### 6.2 What breaks without internet

- Provider callbacks (Zibal, Trawili, Sunrate upstream)
- SSO → Zeepay Feign calls
- CDN-hosted assets (use local Vite dev server instead)
- `docker pull` / `npm install` / `go mod download` if cache empty
- Webhook delivery to external merchant URLs

**Workaround:** use in-memory repos (Pay tests), mock repositories (Pay admin), `MOCK_MODE` (Lira UI), and recorded Postman collections for request shape reference.

### 6.3 Offline debugging decision tree

```text
UI broken?
├─ Static assets 404 → check vite base path vs HAProxy path
├─ API 401 → token env / localStorage keys (see Auth sections below)
├─ API CORS → use Vite proxy or same-origin path routing
└─ Wrong data → MOCK_MODE still on? wrong VITE_API_BASE_URL?

API broken?
├─ Won't start → .env missing DATABASE_URL / JWT secrets
├─ 500 + DB error → migrations applied? connection string?
├─ 502 at edge → container down (docker ps on public-shared network)
└─ Provider error → grep PAY_HTTP_DEBUG / provider logs (needs network for live provider)

Payment stuck?
├─ Worker running? (neivan-pay cmd/worker)
├─ webhook_deliveries table rows?
├─ WEBHOOK_SIGNATURE_DEBUG for HMAC mismatches
└─ intent status in DB vs provider callback logs
```

### 6.4 Local curl cheatsheet (no browser)

```bash
# Lira health
curl -sS http://127.0.0.1:8080/v1/health

# Pay discovery (replace token)
curl -sS -H "Authorization: Bearer $APP_TOKEN" \
  http://127.0.0.1:8080/v1/discovery

# Gateway health
curl -sS http://127.0.0.1:8080/health

# Sunrate proxy
curl -sS http://127.0.0.1:8080/health
```

### 6.5 Database inspection (offline)

```bash
# example: enter staging postgres container
docker exec -it shared-postgres psql -U postgres -d neivan_pay

# useful tables (Pay)
# payment_intents, webhook_deliveries, tenants

# useful tables (Lira)
# cards, invoices, fulfillments — see migrations/
```

### 6.6 HAProxy / routing (on server, no external net)

```bash
# validate config
make haproxy-reload   # in neivan-production or neivan-stageing

# origin test
curl -sS -H 'Host: stg.niwan.net' http://127.0.0.1/gateway/api/health
curl -sS -H 'Host: pgm.liracards.com' -k https://127.0.0.1/api/v1/health
```

**503 NOSRV:** backend container name mismatch — read `neivan-stageing/docs/gateway-sunrate-troubleshooting.md`.

---

## 7. Auth tokens and storage (common confusion)

| App | Storage key | Header |
|-----|-------------|--------|
| Lira panel | localStorage session / bearer | `Authorization: Bearer` (see `client.ts`) |
| Gateway admin UI | `neivan_admin_token` | `Authorization: Bearer` |
| Gateway tenant UI | `neivan_tenant_token` | `Authorization: Bearer` |
| Pay admin | admin session helpers / `VITE_ADMIN_TOKEN` | Bearer via `HttpClient` |
| new-ui | `liracard_token` | axios interceptor |
| sunrate-proxy-ui | `admin_api_key` | `X-Api-Key` |
| Pay merchant API | app token from admin | `Authorization: Bearer` |
| Gateway proxy | tenant API key | per gateway docs |

**401 loop in UI:** clear localStorage keys for that app and re-login.

---

## 8. Common issues and where to look

| Symptom | Likely cause | Where to look |
|---------|--------------|---------------|
| Panel blank after deploy | Wrong `base` in Vite/Next build | `vite.config.ts`, `next.config.ts`, HAProxy strip rules |
| `/v1` 404 | Missing strip prefix or wrong public URL | `haproxy.cfg`, `API_PUBLIC_BASE_URL` in service `.env` |
| Gateway 503 | Stg/prod compose project collision | `make gateway-sunrate-ps`, troubleshooting doc |
| Pay webhook not firing | Worker not running | `cmd/worker`, `webhook_deliveries` table |
| Trawili intent stuck | Provider callback / signature | `PAY_HTTP_DEBUG`, Postman collection |
| Lira card fulfillment pending | Redis worker / queue | `cmd/worker`, redis queue infra |
| SSO login fails locally | DB/Redis not up | `application.yml` dev profile |
| Woo checkout no methods | Discovery URL wrong | plugin settings → must be Pay **API** base URL |
| PHP plugin white screen | `composer install` not run | `woocommerce/vendor/` |

---

## 9. Testing expectations

| Repo | Command | Notes |
|------|---------|-------|
| Go services | `go test ./...` | run before every PR |
| neivan-pay | `make ci` | includes OpenAPI lint |
| neivan-pay-admin | `npm run test` | vitest |
| php-sdk | `vendor/bin/phpunit` | coverage target 95% |
| sso | `./mvnw test` | CI may skip — run locally |
| sunrate-proxy-ui | Automation Tests page | manual integration |

**Integration without internet:** prefer unit tests + mocks; use recorded JSON fixtures in `*_test.go`.

---

## 10. Deployment touchpoints (when you change code)

| Change type | Also update |
|-------------|-------------|
| New API route (public path) | `neivan-production` or `neivan-stageing` `haproxy.cfg` |
| New env var | service `.env.example` + deployed `.env` on server |
| Frontend base path | rebuild Docker image + HAProxy ACL |
| DB schema | migrations + `make migrate-up` on target env |
| Woo plugin | `neivan-pay-integrations` → copy to `wc-shop/plugins/` on staging |
| New log labels | Alloy config on host (`observability-stack/fleet/`) |

**Image build scripts:** many repos have `scripts/imageManager.sh` for stage/prod tags (`neivantech/*` on Docker Hub).

---

## 11. Quick reference — entry files only

| Repo | Start reading here |
|------|-------------------|
| lira-virtual-card | `cmd/api/main.go` → `internal/app/run.go` → `internal/delivery/http/router.go` |
| neivan-pay | `cmd/api/main.go` → `internal/app/api.go` → `internal/delivery/httpapi/router.go` |
| neivan-api-gateway | `cmd/main.go` → `internal/app/server.go` |
| sunrate-proxy | `cmd/server/main.go` → `internal/transport/http/router.go` |
| sso | `SsoApplication.java` → `controller/` → `SecurityConfig.java` |
| Liravirtualmastercardwebapp | `src/main.tsx` → `src/app/routes.tsx` → `src/api/client.ts` |
| neivan-api-gateway-interface | `src/app/page.tsx` → `src/shared/lib/http.ts` |
| neivan-pay-admin | `src/main.tsx` → `src/presentation/App.tsx` → `admin-repository-factory.ts` |
| neivan-pay-integrations | `docs/architecture.md` → `packages/php-sdk` → `woocommerce/neivan-pay-woocommerce.php` |
| neivan-stageing | `README.md` → `infrastructure/haproxy/haproxy.cfg` → `Makefile` |
| observability-stack | `README.md` → `deploy/docker-compose.yml` |

---

## 12. Glossary

| Term | Meaning |
|------|---------|
| BFF | Backend-for-frontend (`lira-virtual-card` for panel) |
| Discovery | Pay endpoint listing available payment providers for amount/currency |
| Payment intent | Pay core object representing a payment attempt |
| API set | Gateway grouping of routes/backends for a tenant |
| Fulfillment | Lira async job completing purchase (card issue, top-up, package) |
| Path strip | HAProxy removes prefix before forwarding to backend |
| Tenant (Pay) | Merchant application using Neivan Pay |
| Tenant (gateway) | Organization whose API keys proxy to backends |

---

## 13. Related files in this workspace

- `README.md` — workspace overview + epic rules
- `docs/epics/README.md` — epic index
- `docs/architecture-deep-dive.md` — structure, principles, system design
- `unified-commits-report.md` / `unified-commits-report-expanded.md` — commit history reports

When in doubt: **read the repo’s `.env.example` and architecture markdown first**, then follow the composition root (`internal/app`) from the entry binary down to the handler you need to change.
