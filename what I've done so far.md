# Unified Commit Report (Expanded)

- Generated: 2026-06-02 17:54:01
- Scope: listed repositories; local and remote branches
- Matching: author OR committer fields matched by broad alias tokens
- Alias tokens: names=['hamid', 'hami', 'hamed'], emails=['hamid', 'hamsaa.ir', 'niwan', 'neivan']
- Repositories with matches: 15
- Branches with matches: 61
- Total matched commits (branch-scoped listing): 2221

## Category Totals

- Features: 841
- Bug Fixes: 686
- Refactors: 5
- Docs: 97
- Chores: 223
- Merges: 48
- Other: 321

## lira-virtual-card

- Branches with matches: 4
- Commits listed in this repo section: 300

### Branch `main` (76)

#### Features (48)

- `2026-06-02` `e202966f` feat(onboarding): provide invoice entrypoint for no-card users  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `a8d1a1ae` feat(invoices): embed assignment summary in list response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-01` `b218b716` feat(kyc): make Tier 1 required channels configurable via app_kv  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `6192f7fd` Add imageManager.sh for stage/prod image publish.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `fd756926` feat: add payment delegation, payer auth, and contact payer linking  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `520cdfd4` feat: expose Neivan Pay provider discovery on checkout BFF  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `a6a75e34` feat: improve Neivan Pay invoicing integration and HTTP debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `48f0f096` feat: integrate invoicing with Neivan Pay orchestration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `bdd70285` feat(fulfillment): gateway card top-up via 200cards API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `a8a2254b` feat(cards): allow nickname-only post-purchase setup without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `9ee9f503` feat(fulfillment): gateway transaction packages via purchase-settlement  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `8eb12d52` feat(transactions): sync issuer auth/settlements to DB and expose GET /v1/transactions  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `8c131b9f` feat(cards): proxy query-card-info for full PAN and CVV on GET /cards/{id}  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `11cceca1` feat(cards): return transactionQuotaRemaining from issuer settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `ca9b3866` feat(cards): wire post-purchase setup and change-pin to gateway PIN APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `49f47e22` feat(gateway): add Neivan gateway client and gatewayprobe CLI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `e5be9b94` feat(admin): add user, config, kyc, limits and finance admin APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `dbcbefe5` feat(otp): add per-flow ttl config and resend timer metadata  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c95b23ca` feat(card-limits): add global and per-user max cards resolution  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8d077003` feat(admin): add admin auth login and admin management cli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `563d5525` feat(otp): include expiry time in sms and email content  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `549daf2a` feat(cli): add cardlimitcli and document docker compose usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `f0b927d6` feat: authenticated change-password and transaction-package fulfillment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `d6f70168` feat(cards): add PUT /cards/{id}/label and POST /cards/{id}/change-pin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `6d31f91e` feat(kyc): Tier 1 verification, SMS/email OTP, and ops hardening  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `5ef8b0ce` feat(transaction-packages): payment methods on pricing and POST quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `56db61c1` feat(cards): issuance pricing methods and quote endpoint  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `391d4a35` feat(pricing): transaction packages from KV with GET /transaction-packages/pricing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `ce7ca513` feat(recharge): add pricing, quote, and rates endpoints  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1199231b` feat(topup): balance credit on fulfillment, invoice metadata in API, result columns  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f73ed0f2` feat(cards): create fulfilled cards as pending_setup  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `b48d7e17` feat(cards): POST complete-setup to activate pending_setup cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `97d12362` feat: implement async fulfillment worker and expand backend coverage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `7a0e36f1` feat: invoices and Zibal payment intents API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d44acb48` feat(smtp): submission TLS, optional cleartext auth, and mail headers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c2018d99` feat: GET /v1/cards — list user cards from Postgres  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `a1edf502` feat: app_kv, issuance pricing API, kvcatalog, kvcli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `583a1fb7` feat(auth): add backend-driven device challenge flow and CORS support  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `792f152d` feat: log Redis/Postgres startup connectivity state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-05` `8b3f17e5` Add route delivery doc §6.3, Kavenegar SMS and SMTP email OTP  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `be218cae` feat(phase1): observability, logging, recover, timeouts, CI; close Phase 0  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `b2d476a3` feat(auth): JWT (HS256), migrations, password login, profile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `9d60a7a9` docs: add PRD, technical spec, and canonical database schema  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `99d3d8cd` feat(auth): B2C /v1/auth/* API, OTP tables, dual-session, rate limits  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `89aa9b4a` feat(auth): per-mobile OTP resend cooldown via Redis  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `58075232` feat: Phase 0 API contract (Postman) and Go skeleton with GET /v1/health  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `501ae1c2` feat: config, Postgres/Redis wiring, GET /v1/ready  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `35493574` feat(docker): add PostgreSQL and Redis to compose stack  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (18)

- `2026-06-02` `4a7ba4cd` fix(card-cap): exclude open invoices from slot ceiling  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `1bb1b2c0` fix(card-cap): count active card-purchase requests as used slots  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-01` `b336eafb` fix(kyc): do not re-require channels already verified after policy bump  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `cdc095a2` fix: Neivan Pay return sync and webhook signature diagnostics  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `edee4796` fix(cards): sync masked PAN and expiry on list from issuer query-card-info  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `b56e6a0f` fix(fulfillment): increment quota on package purchase instead of SET from settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `63b3d8ec` fix(fulfillment): sync transaction quota from issuer settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `51ce183a` fix(fulfillment): complete transaction packages without request-status poll  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `56134d6e` feat(fulfillment): gateway issuance, admin restart, and payment path fixes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `fc4c6b57` fix(issuance): return IRR pricing and use configured USD base quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `d7ec27a7` fix(invoices): normalize legacy IRT amounts to IRR in API DTOs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `9eda3535` fix(auth): remove national id from signup flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `5c39a41e` fix(packages): return IRR display currency in quote response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `1af18d33` fix(kyc): mark signup email verified in tier1  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `b51b69e7` fix(kyc): persist tier1 verification for users missing kyc row  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `59f7a6b1` fix(fx): treat Tetherland price as Toman and convert to IRR (Rials)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `bb9d40d6` fix: expose payment envs and idempotency header in CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `df16f1a6` fix(auth): device fingerprint hash, login SQL casts, SMS/Kavenegar docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (2)

- `2026-04-11` `4baf2350` docs and ops: Postman auth flows, SMTP env examples, compose SMTP passthrough  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `3c3d53a2` docs: .env.example hints for local DATABASE_URL/REDIS_ADDR  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (5)

- `2026-05-16` `888bb5e1` docker images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `e6268b8d` chore: expand .gitignore for build artifacts and tooling  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `9d4c9c6a` chore: updates gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `717e6a00` chore: stop tracking vendor/ (keep local copy ignored)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `334ab50d` chore: Go 1.26.0 toolchain, Dockerfile (Alpine), Docker Compose  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-05-26` `1057c821` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `cdb246a3` Dockerfile: pull builder and runtime images from hub.hamdocker.ir mirrors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-05` `f4c0dd12` Auth send-otp: intent, email lookup, signup email OTP / login SMS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `newgit/main` (72)

#### Features (46)

- `2026-06-01` `b218b716` feat(kyc): make Tier 1 required channels configurable via app_kv  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `6192f7fd` Add imageManager.sh for stage/prod image publish.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `fd756926` feat: add payment delegation, payer auth, and contact payer linking  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `520cdfd4` feat: expose Neivan Pay provider discovery on checkout BFF  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `a6a75e34` feat: improve Neivan Pay invoicing integration and HTTP debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `48f0f096` feat: integrate invoicing with Neivan Pay orchestration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `bdd70285` feat(fulfillment): gateway card top-up via 200cards API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `a8a2254b` feat(cards): allow nickname-only post-purchase setup without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `9ee9f503` feat(fulfillment): gateway transaction packages via purchase-settlement  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `8eb12d52` feat(transactions): sync issuer auth/settlements to DB and expose GET /v1/transactions  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `8c131b9f` feat(cards): proxy query-card-info for full PAN and CVV on GET /cards/{id}  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `11cceca1` feat(cards): return transactionQuotaRemaining from issuer settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `ca9b3866` feat(cards): wire post-purchase setup and change-pin to gateway PIN APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `49f47e22` feat(gateway): add Neivan gateway client and gatewayprobe CLI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `e5be9b94` feat(admin): add user, config, kyc, limits and finance admin APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `dbcbefe5` feat(otp): add per-flow ttl config and resend timer metadata  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c95b23ca` feat(card-limits): add global and per-user max cards resolution  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8d077003` feat(admin): add admin auth login and admin management cli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `563d5525` feat(otp): include expiry time in sms and email content  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `549daf2a` feat(cli): add cardlimitcli and document docker compose usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `f0b927d6` feat: authenticated change-password and transaction-package fulfillment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `d6f70168` feat(cards): add PUT /cards/{id}/label and POST /cards/{id}/change-pin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `6d31f91e` feat(kyc): Tier 1 verification, SMS/email OTP, and ops hardening  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `5ef8b0ce` feat(transaction-packages): payment methods on pricing and POST quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `56db61c1` feat(cards): issuance pricing methods and quote endpoint  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `391d4a35` feat(pricing): transaction packages from KV with GET /transaction-packages/pricing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `ce7ca513` feat(recharge): add pricing, quote, and rates endpoints  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1199231b` feat(topup): balance credit on fulfillment, invoice metadata in API, result columns  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f73ed0f2` feat(cards): create fulfilled cards as pending_setup  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `b48d7e17` feat(cards): POST complete-setup to activate pending_setup cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `97d12362` feat: implement async fulfillment worker and expand backend coverage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `7a0e36f1` feat: invoices and Zibal payment intents API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d44acb48` feat(smtp): submission TLS, optional cleartext auth, and mail headers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c2018d99` feat: GET /v1/cards — list user cards from Postgres  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `a1edf502` feat: app_kv, issuance pricing API, kvcatalog, kvcli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `583a1fb7` feat(auth): add backend-driven device challenge flow and CORS support  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `792f152d` feat: log Redis/Postgres startup connectivity state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-05` `8b3f17e5` Add route delivery doc §6.3, Kavenegar SMS and SMTP email OTP  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `be218cae` feat(phase1): observability, logging, recover, timeouts, CI; close Phase 0  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `b2d476a3` feat(auth): JWT (HS256), migrations, password login, profile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `9d60a7a9` docs: add PRD, technical spec, and canonical database schema  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `99d3d8cd` feat(auth): B2C /v1/auth/* API, OTP tables, dual-session, rate limits  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `89aa9b4a` feat(auth): per-mobile OTP resend cooldown via Redis  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `58075232` feat: Phase 0 API contract (Postman) and Go skeleton with GET /v1/health  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `501ae1c2` feat: config, Postgres/Redis wiring, GET /v1/ready  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `35493574` feat(docker): add PostgreSQL and Redis to compose stack  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (16)

- `2026-06-01` `b336eafb` fix(kyc): do not re-require channels already verified after policy bump  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `cdc095a2` fix: Neivan Pay return sync and webhook signature diagnostics  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `edee4796` fix(cards): sync masked PAN and expiry on list from issuer query-card-info  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `b56e6a0f` fix(fulfillment): increment quota on package purchase instead of SET from settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `63b3d8ec` fix(fulfillment): sync transaction quota from issuer settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `51ce183a` fix(fulfillment): complete transaction packages without request-status poll  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `56134d6e` feat(fulfillment): gateway issuance, admin restart, and payment path fixes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `fc4c6b57` fix(issuance): return IRR pricing and use configured USD base quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `d7ec27a7` fix(invoices): normalize legacy IRT amounts to IRR in API DTOs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `9eda3535` fix(auth): remove national id from signup flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `5c39a41e` fix(packages): return IRR display currency in quote response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `1af18d33` fix(kyc): mark signup email verified in tier1  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `b51b69e7` fix(kyc): persist tier1 verification for users missing kyc row  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `59f7a6b1` fix(fx): treat Tetherland price as Toman and convert to IRR (Rials)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `bb9d40d6` fix: expose payment envs and idempotency header in CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `df16f1a6` fix(auth): device fingerprint hash, login SQL casts, SMS/Kavenegar docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (2)

- `2026-04-11` `4baf2350` docs and ops: Postman auth flows, SMTP env examples, compose SMTP passthrough  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `3c3d53a2` docs: .env.example hints for local DATABASE_URL/REDIS_ADDR  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (5)

- `2026-05-16` `888bb5e1` docker images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `e6268b8d` chore: expand .gitignore for build artifacts and tooling  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `9d4c9c6a` chore: updates gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `717e6a00` chore: stop tracking vendor/ (keep local copy ignored)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `334ab50d` chore: Go 1.26.0 toolchain, Dockerfile (Alpine), Docker Compose  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-05-26` `1057c821` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `cdb246a3` Dockerfile: pull builder and runtime images from hub.hamdocker.ir mirrors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-05` `f4c0dd12` Auth send-otp: intent, email lookup, signup email OTP / login SMS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/HEAD` (76)

#### Features (48)

- `2026-06-02` `e202966f` feat(onboarding): provide invoice entrypoint for no-card users  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `a8d1a1ae` feat(invoices): embed assignment summary in list response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-01` `b218b716` feat(kyc): make Tier 1 required channels configurable via app_kv  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `6192f7fd` Add imageManager.sh for stage/prod image publish.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `fd756926` feat: add payment delegation, payer auth, and contact payer linking  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `520cdfd4` feat: expose Neivan Pay provider discovery on checkout BFF  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `a6a75e34` feat: improve Neivan Pay invoicing integration and HTTP debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `48f0f096` feat: integrate invoicing with Neivan Pay orchestration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `bdd70285` feat(fulfillment): gateway card top-up via 200cards API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `a8a2254b` feat(cards): allow nickname-only post-purchase setup without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `9ee9f503` feat(fulfillment): gateway transaction packages via purchase-settlement  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `8eb12d52` feat(transactions): sync issuer auth/settlements to DB and expose GET /v1/transactions  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `8c131b9f` feat(cards): proxy query-card-info for full PAN and CVV on GET /cards/{id}  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `11cceca1` feat(cards): return transactionQuotaRemaining from issuer settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `ca9b3866` feat(cards): wire post-purchase setup and change-pin to gateway PIN APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `49f47e22` feat(gateway): add Neivan gateway client and gatewayprobe CLI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `e5be9b94` feat(admin): add user, config, kyc, limits and finance admin APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `dbcbefe5` feat(otp): add per-flow ttl config and resend timer metadata  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c95b23ca` feat(card-limits): add global and per-user max cards resolution  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8d077003` feat(admin): add admin auth login and admin management cli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `563d5525` feat(otp): include expiry time in sms and email content  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `549daf2a` feat(cli): add cardlimitcli and document docker compose usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `f0b927d6` feat: authenticated change-password and transaction-package fulfillment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `d6f70168` feat(cards): add PUT /cards/{id}/label and POST /cards/{id}/change-pin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `6d31f91e` feat(kyc): Tier 1 verification, SMS/email OTP, and ops hardening  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `5ef8b0ce` feat(transaction-packages): payment methods on pricing and POST quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `56db61c1` feat(cards): issuance pricing methods and quote endpoint  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `391d4a35` feat(pricing): transaction packages from KV with GET /transaction-packages/pricing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `ce7ca513` feat(recharge): add pricing, quote, and rates endpoints  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1199231b` feat(topup): balance credit on fulfillment, invoice metadata in API, result columns  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f73ed0f2` feat(cards): create fulfilled cards as pending_setup  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `b48d7e17` feat(cards): POST complete-setup to activate pending_setup cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `97d12362` feat: implement async fulfillment worker and expand backend coverage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `7a0e36f1` feat: invoices and Zibal payment intents API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d44acb48` feat(smtp): submission TLS, optional cleartext auth, and mail headers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c2018d99` feat: GET /v1/cards — list user cards from Postgres  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `a1edf502` feat: app_kv, issuance pricing API, kvcatalog, kvcli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `583a1fb7` feat(auth): add backend-driven device challenge flow and CORS support  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `792f152d` feat: log Redis/Postgres startup connectivity state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-05` `8b3f17e5` Add route delivery doc §6.3, Kavenegar SMS and SMTP email OTP  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `be218cae` feat(phase1): observability, logging, recover, timeouts, CI; close Phase 0  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `b2d476a3` feat(auth): JWT (HS256), migrations, password login, profile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `9d60a7a9` docs: add PRD, technical spec, and canonical database schema  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `99d3d8cd` feat(auth): B2C /v1/auth/* API, OTP tables, dual-session, rate limits  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `89aa9b4a` feat(auth): per-mobile OTP resend cooldown via Redis  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `58075232` feat: Phase 0 API contract (Postman) and Go skeleton with GET /v1/health  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `501ae1c2` feat: config, Postgres/Redis wiring, GET /v1/ready  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `35493574` feat(docker): add PostgreSQL and Redis to compose stack  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (18)

- `2026-06-02` `4a7ba4cd` fix(card-cap): exclude open invoices from slot ceiling  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `1bb1b2c0` fix(card-cap): count active card-purchase requests as used slots  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-01` `b336eafb` fix(kyc): do not re-require channels already verified after policy bump  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `cdc095a2` fix: Neivan Pay return sync and webhook signature diagnostics  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `edee4796` fix(cards): sync masked PAN and expiry on list from issuer query-card-info  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `b56e6a0f` fix(fulfillment): increment quota on package purchase instead of SET from settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `63b3d8ec` fix(fulfillment): sync transaction quota from issuer settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `51ce183a` fix(fulfillment): complete transaction packages without request-status poll  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `56134d6e` feat(fulfillment): gateway issuance, admin restart, and payment path fixes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `fc4c6b57` fix(issuance): return IRR pricing and use configured USD base quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `d7ec27a7` fix(invoices): normalize legacy IRT amounts to IRR in API DTOs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `9eda3535` fix(auth): remove national id from signup flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `5c39a41e` fix(packages): return IRR display currency in quote response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `1af18d33` fix(kyc): mark signup email verified in tier1  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `b51b69e7` fix(kyc): persist tier1 verification for users missing kyc row  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `59f7a6b1` fix(fx): treat Tetherland price as Toman and convert to IRR (Rials)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `bb9d40d6` fix: expose payment envs and idempotency header in CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `df16f1a6` fix(auth): device fingerprint hash, login SQL casts, SMS/Kavenegar docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (2)

- `2026-04-11` `4baf2350` docs and ops: Postman auth flows, SMTP env examples, compose SMTP passthrough  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `3c3d53a2` docs: .env.example hints for local DATABASE_URL/REDIS_ADDR  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (5)

- `2026-05-16` `888bb5e1` docker images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `e6268b8d` chore: expand .gitignore for build artifacts and tooling  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `9d4c9c6a` chore: updates gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `717e6a00` chore: stop tracking vendor/ (keep local copy ignored)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `334ab50d` chore: Go 1.26.0 toolchain, Dockerfile (Alpine), Docker Compose  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-05-26` `1057c821` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `cdb246a3` Dockerfile: pull builder and runtime images from hub.hamdocker.ir mirrors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-05` `f4c0dd12` Auth send-otp: intent, email lookup, signup email OTP / login SMS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (76)

#### Features (48)

- `2026-06-02` `e202966f` feat(onboarding): provide invoice entrypoint for no-card users  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `a8d1a1ae` feat(invoices): embed assignment summary in list response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-01` `b218b716` feat(kyc): make Tier 1 required channels configurable via app_kv  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `6192f7fd` Add imageManager.sh for stage/prod image publish.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `fd756926` feat: add payment delegation, payer auth, and contact payer linking  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `520cdfd4` feat: expose Neivan Pay provider discovery on checkout BFF  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `a6a75e34` feat: improve Neivan Pay invoicing integration and HTTP debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `48f0f096` feat: integrate invoicing with Neivan Pay orchestration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `bdd70285` feat(fulfillment): gateway card top-up via 200cards API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `a8a2254b` feat(cards): allow nickname-only post-purchase setup without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `9ee9f503` feat(fulfillment): gateway transaction packages via purchase-settlement  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `8eb12d52` feat(transactions): sync issuer auth/settlements to DB and expose GET /v1/transactions  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `8c131b9f` feat(cards): proxy query-card-info for full PAN and CVV on GET /cards/{id}  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `11cceca1` feat(cards): return transactionQuotaRemaining from issuer settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `ca9b3866` feat(cards): wire post-purchase setup and change-pin to gateway PIN APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `49f47e22` feat(gateway): add Neivan gateway client and gatewayprobe CLI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `e5be9b94` feat(admin): add user, config, kyc, limits and finance admin APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `dbcbefe5` feat(otp): add per-flow ttl config and resend timer metadata  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c95b23ca` feat(card-limits): add global and per-user max cards resolution  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8d077003` feat(admin): add admin auth login and admin management cli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `563d5525` feat(otp): include expiry time in sms and email content  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `549daf2a` feat(cli): add cardlimitcli and document docker compose usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `f0b927d6` feat: authenticated change-password and transaction-package fulfillment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `d6f70168` feat(cards): add PUT /cards/{id}/label and POST /cards/{id}/change-pin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `6d31f91e` feat(kyc): Tier 1 verification, SMS/email OTP, and ops hardening  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `5ef8b0ce` feat(transaction-packages): payment methods on pricing and POST quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `56db61c1` feat(cards): issuance pricing methods and quote endpoint  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `391d4a35` feat(pricing): transaction packages from KV with GET /transaction-packages/pricing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `ce7ca513` feat(recharge): add pricing, quote, and rates endpoints  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1199231b` feat(topup): balance credit on fulfillment, invoice metadata in API, result columns  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f73ed0f2` feat(cards): create fulfilled cards as pending_setup  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `b48d7e17` feat(cards): POST complete-setup to activate pending_setup cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `97d12362` feat: implement async fulfillment worker and expand backend coverage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `7a0e36f1` feat: invoices and Zibal payment intents API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d44acb48` feat(smtp): submission TLS, optional cleartext auth, and mail headers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c2018d99` feat: GET /v1/cards — list user cards from Postgres  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `a1edf502` feat: app_kv, issuance pricing API, kvcatalog, kvcli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `583a1fb7` feat(auth): add backend-driven device challenge flow and CORS support  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `792f152d` feat: log Redis/Postgres startup connectivity state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-05` `8b3f17e5` Add route delivery doc §6.3, Kavenegar SMS and SMTP email OTP  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `be218cae` feat(phase1): observability, logging, recover, timeouts, CI; close Phase 0  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `b2d476a3` feat(auth): JWT (HS256), migrations, password login, profile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `9d60a7a9` docs: add PRD, technical spec, and canonical database schema  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `99d3d8cd` feat(auth): B2C /v1/auth/* API, OTP tables, dual-session, rate limits  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `89aa9b4a` feat(auth): per-mobile OTP resend cooldown via Redis  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `58075232` feat: Phase 0 API contract (Postman) and Go skeleton with GET /v1/health  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `501ae1c2` feat: config, Postgres/Redis wiring, GET /v1/ready  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `35493574` feat(docker): add PostgreSQL and Redis to compose stack  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (18)

- `2026-06-02` `4a7ba4cd` fix(card-cap): exclude open invoices from slot ceiling  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `1bb1b2c0` fix(card-cap): count active card-purchase requests as used slots  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-01` `b336eafb` fix(kyc): do not re-require channels already verified after policy bump  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `cdc095a2` fix: Neivan Pay return sync and webhook signature diagnostics  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `edee4796` fix(cards): sync masked PAN and expiry on list from issuer query-card-info  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `b56e6a0f` fix(fulfillment): increment quota on package purchase instead of SET from settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `63b3d8ec` fix(fulfillment): sync transaction quota from issuer settlement_counter  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `51ce183a` fix(fulfillment): complete transaction packages without request-status poll  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `56134d6e` feat(fulfillment): gateway issuance, admin restart, and payment path fixes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `fc4c6b57` fix(issuance): return IRR pricing and use configured USD base quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `d7ec27a7` fix(invoices): normalize legacy IRT amounts to IRR in API DTOs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `9eda3535` fix(auth): remove national id from signup flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `5c39a41e` fix(packages): return IRR display currency in quote response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `1af18d33` fix(kyc): mark signup email verified in tier1  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `b51b69e7` fix(kyc): persist tier1 verification for users missing kyc row  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `59f7a6b1` fix(fx): treat Tetherland price as Toman and convert to IRR (Rials)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `bb9d40d6` fix: expose payment envs and idempotency header in CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `df16f1a6` fix(auth): device fingerprint hash, login SQL casts, SMS/Kavenegar docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (2)

- `2026-04-11` `4baf2350` docs and ops: Postman auth flows, SMTP env examples, compose SMTP passthrough  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `3c3d53a2` docs: .env.example hints for local DATABASE_URL/REDIS_ADDR  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (5)

- `2026-05-16` `888bb5e1` docker images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `e6268b8d` chore: expand .gitignore for build artifacts and tooling  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `9d4c9c6a` chore: updates gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `717e6a00` chore: stop tracking vendor/ (keep local copy ignored)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-04` `334ab50d` chore: Go 1.26.0 toolchain, Dockerfile (Alpine), Docker Compose  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-05-26` `1057c821` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `cdb246a3` Dockerfile: pull builder and runtime images from hub.hamdocker.ir mirrors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-05` `f4c0dd12` Auth send-otp: intent, email lookup, signup email OTP / login SMS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## Liravirtualmastercardwebapp

- Branches with matches: 7
- Commits listed in this repo section: 372

### Branch `develop` (76)

#### Features (27)

- `2026-06-01` `bb2d3c36` feat(auth): default phone country to United States (+1) on login and signup  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-01` `b488e1b3` feat(kyc): respect server Tier 1 requiredChannels in profile UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `27137953` Add imageManager.sh for stage/prod Docker builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `85fe2168` feat: payment delegation UI, payer routes, and invoice management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `84641f29` feat: support staging deploy under /virtual/ path prefix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `400641f6` feat: Pay checkout discovery with currency and gateway selection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `eb34e22c` feat(post-purchase): nickname-only setup activates card without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `ab1bc1d9` feat(top-up): show IRR amounts and refresh expired quotes on pay  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `7ec902b8` feat(top-up): hide fees and load min/max from pricing API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `58116f6f` feat(cards): hide block and PIN actions from cards page toolbar  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `53e9bc56` feat(packages): hide fee row and include fee in IRR equivalent on package cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `3909eec1` feat(cards): load sensitive card details in modal via backend proxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `e3f5b46c` feat(cards): gateway PIN setup UX and fulfillment restart polish  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `b5fee756` feat(otp-ui): render resend countdown from backend timing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `e0aa746b` feat(cards): wire My Cards rename and PIN flows to API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `dfbf5693` feat(packages): payment method selection and live quote on confirm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `de5dc8ba` feat(kyc): Tier 1 gate, profile OTP, and resilient API loading  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `8e7dcec6` feat: buy-card USD/crypto, invoice crypto display, Iran phone validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67d30c23` feat: change-password API, transaction packages, and invoices  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `33d4169f` feat(packages): load pricing from API and restrict picker to active cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `f0189c9c` feat(topup): crypto invoice USD display, auto-refresh, cards reload after top-up  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8502861c` feat(top-up): dynamic pricing/quote API and clearer API errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1b8bfb5c` feat(web): load top-up pricing and quotes from backend  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d9b76b97` Docker and API client: env-aware builds, add image-manager script  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `4a4bad59` feat(auth): wire login/signup/reset flows to backend and env-configurable API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `2001b2c9` Add Docker and Nginx setup for web app deployment.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `f9a24b52` Update asset imports and add project gitignore.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (29)

- `2026-06-02` `dc99aa55` fix: redirect no-card users to active invoice fulfillment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `b4a66408` fix(onboarding-nav): prevent buy-card redirect loop on manual entry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `b3b210f9` fix(onboarding): route no-card users to status-aware destinations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `a9ad5574` fix(invoice): allow retry flow when canPay is only root-level  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `3fb4826c` fix(card-cap-ui): hide buy-card entry and block checkout at limit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `2454619c` fix: honor /virtual/panel base path for redirects and favicon  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `f98522fa` fix(transactions): map API fields for list tabs and refetch on transactions page  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `aafbf5c8` fix: stop transactions API loop and simplify help support tab  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `259774ff` fix(cards): show quota total at least as high as remaining from API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `ef388503` fix(buy-card): align issuance checkout with IRR and fixed USD quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c68ec553` fix(otp-ui): show expiry countdown and isolate resend state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c14cca62` fix(cards-ui): use profile maxCards instead of hardcoded cap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `98b8ddfc` fix(signup): remove national id step from registration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8f33137b` fix: sets default en langaufe  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `51efc346` fix(buy-card): remove redundant payment method subtitles  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `4967b531` fix(otp-ui): unify resend timer to MM:SS countdown  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `3ab7b957` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `263853b0` fix(invoices-ui): show IRR values and simplify top-up invoice lines  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34d8e3ad` fix(pwa): enforce network-only service worker and disable HTTP caching  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67c57b7f` fix(signup): clarify terms modal CTA copy in Persian  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `976efc58` fix: navigares to login pag e  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8ac3c9d6` fix(top-up): remove live USD/IRR rate line from card header  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `41c2afc1` fix(web): self-host Vazirmatn font for offline usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f17686f3` fix: align buy-card invoice flow with backend contracts  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `12f7e03c` fix(web): dedupe completeCardSetup and align develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `0214530a` fix: render invoice line items in invoice detail  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `9fb19808` fix(auth): clear session on public login/signup routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `44889604` fix: stop API error page reload loop (/app/*/error)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3ef774c0` Fix Persian font loading and RTL font application.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Refactors (1)

- `2026-06-02` `04a81f33` refine(invoice-ux): simplify status language and remove technical labels  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (2)

- `2026-04-18` `1691b7ff` chore: remove GET /exchange-rate client usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3134d075` Update lockfile peer dependency metadata.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Merges (8)

- `2026-04-13` `fa88f895` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `83f48fc8` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `6a552b73` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `1acf7e62` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c237b7b6` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `ae705320` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `407b9d31` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `79af6117` Merge branch 'main' of https://github.com/liracards/Liravirtualmastercardwebapp into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (9)

- `2026-06-02` `89149fc3` alll  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `4071de8d` perf(invoices): consume assignment data from list payload  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `e56cecc3` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `6815fae2` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `24c4aabb` rebranding  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `0a360889` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `c678b2ff` Update Vite base path for stg.niwan.net/virtual/panel deploy.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `b50baa64` Dockerfile: use node:alpine and nginx:alpine base images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `7e7f056f` Disable app mock mode for auth and cards flows.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `feat/topup-dynamic-pricing-quote` (50)

#### Features (18)

- `2026-05-17` `eb34e22c` feat(post-purchase): nickname-only setup activates card without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `58116f6f` feat(cards): hide block and PIN actions from cards page toolbar  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `3909eec1` feat(cards): load sensitive card details in modal via backend proxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `e3f5b46c` feat(cards): gateway PIN setup UX and fulfillment restart polish  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `b5fee756` feat(otp-ui): render resend countdown from backend timing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `e0aa746b` feat(cards): wire My Cards rename and PIN flows to API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `dfbf5693` feat(packages): payment method selection and live quote on confirm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `de5dc8ba` feat(kyc): Tier 1 gate, profile OTP, and resilient API loading  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `8e7dcec6` feat: buy-card USD/crypto, invoice crypto display, Iran phone validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67d30c23` feat: change-password API, transaction packages, and invoices  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `33d4169f` feat(packages): load pricing from API and restrict picker to active cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `f0189c9c` feat(topup): crypto invoice USD display, auto-refresh, cards reload after top-up  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8502861c` feat(top-up): dynamic pricing/quote API and clearer API errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1b8bfb5c` feat(web): load top-up pricing and quotes from backend  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d9b76b97` Docker and API client: env-aware builds, add image-manager script  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `4a4bad59` feat(auth): wire login/signup/reset flows to backend and env-configurable API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `2001b2c9` Add Docker and Nginx setup for web app deployment.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `f9a24b52` Update asset imports and add project gitignore.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (20)

- `2026-04-25` `ef388503` fix(buy-card): align issuance checkout with IRR and fixed USD quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c68ec553` fix(otp-ui): show expiry countdown and isolate resend state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c14cca62` fix(cards-ui): use profile maxCards instead of hardcoded cap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `98b8ddfc` fix(signup): remove national id step from registration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8f33137b` fix: sets default en langaufe  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `51efc346` fix(buy-card): remove redundant payment method subtitles  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `4967b531` fix(otp-ui): unify resend timer to MM:SS countdown  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `3ab7b957` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `263853b0` fix(invoices-ui): show IRR values and simplify top-up invoice lines  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34d8e3ad` fix(pwa): enforce network-only service worker and disable HTTP caching  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67c57b7f` fix(signup): clarify terms modal CTA copy in Persian  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `976efc58` fix: navigares to login pag e  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8ac3c9d6` fix(top-up): remove live USD/IRR rate line from card header  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `41c2afc1` fix(web): self-host Vazirmatn font for offline usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f17686f3` fix: align buy-card invoice flow with backend contracts  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `12f7e03c` fix(web): dedupe completeCardSetup and align develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `0214530a` fix: render invoice line items in invoice detail  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `9fb19808` fix(auth): clear session on public login/signup routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `44889604` fix: stop API error page reload loop (/app/*/error)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3ef774c0` Fix Persian font loading and RTL font application.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (2)

- `2026-04-18` `1691b7ff` chore: remove GET /exchange-rate client usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3134d075` Update lockfile peer dependency metadata.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Merges (8)

- `2026-04-13` `fa88f895` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `83f48fc8` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `6a552b73` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `1acf7e62` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c237b7b6` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `ae705320` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `407b9d31` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `79af6117` Merge branch 'main' of https://github.com/liracards/Liravirtualmastercardwebapp into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (2)

- `2026-04-11` `b50baa64` Dockerfile: use node:alpine and nginx:alpine base images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `7e7f056f` Disable app mock mode for auth and cards flows.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `newgit/develop` (68)

#### Features (27)

- `2026-06-01` `bb2d3c36` feat(auth): default phone country to United States (+1) on login and signup  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-01` `b488e1b3` feat(kyc): respect server Tier 1 requiredChannels in profile UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `27137953` Add imageManager.sh for stage/prod Docker builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `85fe2168` feat: payment delegation UI, payer routes, and invoice management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `84641f29` feat: support staging deploy under /virtual/ path prefix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `400641f6` feat: Pay checkout discovery with currency and gateway selection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `eb34e22c` feat(post-purchase): nickname-only setup activates card without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `ab1bc1d9` feat(top-up): show IRR amounts and refresh expired quotes on pay  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `7ec902b8` feat(top-up): hide fees and load min/max from pricing API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `58116f6f` feat(cards): hide block and PIN actions from cards page toolbar  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `53e9bc56` feat(packages): hide fee row and include fee in IRR equivalent on package cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `3909eec1` feat(cards): load sensitive card details in modal via backend proxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `e3f5b46c` feat(cards): gateway PIN setup UX and fulfillment restart polish  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `b5fee756` feat(otp-ui): render resend countdown from backend timing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `e0aa746b` feat(cards): wire My Cards rename and PIN flows to API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `dfbf5693` feat(packages): payment method selection and live quote on confirm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `de5dc8ba` feat(kyc): Tier 1 gate, profile OTP, and resilient API loading  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `8e7dcec6` feat: buy-card USD/crypto, invoice crypto display, Iran phone validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67d30c23` feat: change-password API, transaction packages, and invoices  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `33d4169f` feat(packages): load pricing from API and restrict picker to active cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `f0189c9c` feat(topup): crypto invoice USD display, auto-refresh, cards reload after top-up  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8502861c` feat(top-up): dynamic pricing/quote API and clearer API errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1b8bfb5c` feat(web): load top-up pricing and quotes from backend  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d9b76b97` Docker and API client: env-aware builds, add image-manager script  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `4a4bad59` feat(auth): wire login/signup/reset flows to backend and env-configurable API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `2001b2c9` Add Docker and Nginx setup for web app deployment.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `f9a24b52` Update asset imports and add project gitignore.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (24)

- `2026-05-24` `2454619c` fix: honor /virtual/panel base path for redirects and favicon  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `f98522fa` fix(transactions): map API fields for list tabs and refetch on transactions page  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `aafbf5c8` fix: stop transactions API loop and simplify help support tab  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `259774ff` fix(cards): show quota total at least as high as remaining from API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `ef388503` fix(buy-card): align issuance checkout with IRR and fixed USD quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c68ec553` fix(otp-ui): show expiry countdown and isolate resend state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c14cca62` fix(cards-ui): use profile maxCards instead of hardcoded cap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `98b8ddfc` fix(signup): remove national id step from registration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8f33137b` fix: sets default en langaufe  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `51efc346` fix(buy-card): remove redundant payment method subtitles  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `4967b531` fix(otp-ui): unify resend timer to MM:SS countdown  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `3ab7b957` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `263853b0` fix(invoices-ui): show IRR values and simplify top-up invoice lines  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34d8e3ad` fix(pwa): enforce network-only service worker and disable HTTP caching  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67c57b7f` fix(signup): clarify terms modal CTA copy in Persian  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `976efc58` fix: navigares to login pag e  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8ac3c9d6` fix(top-up): remove live USD/IRR rate line from card header  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `41c2afc1` fix(web): self-host Vazirmatn font for offline usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f17686f3` fix: align buy-card invoice flow with backend contracts  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `12f7e03c` fix(web): dedupe completeCardSetup and align develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `0214530a` fix: render invoice line items in invoice detail  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `9fb19808` fix(auth): clear session on public login/signup routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `44889604` fix: stop API error page reload loop (/app/*/error)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3ef774c0` Fix Persian font loading and RTL font application.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (2)

- `2026-04-18` `1691b7ff` chore: remove GET /exchange-rate client usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3134d075` Update lockfile peer dependency metadata.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Merges (8)

- `2026-04-13` `fa88f895` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `83f48fc8` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `6a552b73` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `1acf7e62` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c237b7b6` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `ae705320` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `407b9d31` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `79af6117` Merge branch 'main' of https://github.com/liracards/Liravirtualmastercardwebapp into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (7)

- `2026-05-31` `e56cecc3` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `6815fae2` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `24c4aabb` rebranding  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `0a360889` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `c678b2ff` Update Vite base path for stg.niwan.net/virtual/panel deploy.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `b50baa64` Dockerfile: use node:alpine and nginx:alpine base images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `7e7f056f` Disable app mock mode for auth and cards flows.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `newgit/feat/topup-dynamic-pricing-quote` (50)

#### Features (18)

- `2026-05-17` `eb34e22c` feat(post-purchase): nickname-only setup activates card without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `58116f6f` feat(cards): hide block and PIN actions from cards page toolbar  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `3909eec1` feat(cards): load sensitive card details in modal via backend proxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `e3f5b46c` feat(cards): gateway PIN setup UX and fulfillment restart polish  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `b5fee756` feat(otp-ui): render resend countdown from backend timing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `e0aa746b` feat(cards): wire My Cards rename and PIN flows to API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `dfbf5693` feat(packages): payment method selection and live quote on confirm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `de5dc8ba` feat(kyc): Tier 1 gate, profile OTP, and resilient API loading  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `8e7dcec6` feat: buy-card USD/crypto, invoice crypto display, Iran phone validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67d30c23` feat: change-password API, transaction packages, and invoices  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `33d4169f` feat(packages): load pricing from API and restrict picker to active cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `f0189c9c` feat(topup): crypto invoice USD display, auto-refresh, cards reload after top-up  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8502861c` feat(top-up): dynamic pricing/quote API and clearer API errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1b8bfb5c` feat(web): load top-up pricing and quotes from backend  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d9b76b97` Docker and API client: env-aware builds, add image-manager script  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `4a4bad59` feat(auth): wire login/signup/reset flows to backend and env-configurable API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `2001b2c9` Add Docker and Nginx setup for web app deployment.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `f9a24b52` Update asset imports and add project gitignore.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (20)

- `2026-04-25` `ef388503` fix(buy-card): align issuance checkout with IRR and fixed USD quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c68ec553` fix(otp-ui): show expiry countdown and isolate resend state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c14cca62` fix(cards-ui): use profile maxCards instead of hardcoded cap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `98b8ddfc` fix(signup): remove national id step from registration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8f33137b` fix: sets default en langaufe  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `51efc346` fix(buy-card): remove redundant payment method subtitles  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `4967b531` fix(otp-ui): unify resend timer to MM:SS countdown  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `3ab7b957` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `263853b0` fix(invoices-ui): show IRR values and simplify top-up invoice lines  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34d8e3ad` fix(pwa): enforce network-only service worker and disable HTTP caching  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67c57b7f` fix(signup): clarify terms modal CTA copy in Persian  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `976efc58` fix: navigares to login pag e  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8ac3c9d6` fix(top-up): remove live USD/IRR rate line from card header  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `41c2afc1` fix(web): self-host Vazirmatn font for offline usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f17686f3` fix: align buy-card invoice flow with backend contracts  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `12f7e03c` fix(web): dedupe completeCardSetup and align develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `0214530a` fix: render invoice line items in invoice detail  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `9fb19808` fix(auth): clear session on public login/signup routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `44889604` fix: stop API error page reload loop (/app/*/error)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3ef774c0` Fix Persian font loading and RTL font application.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (2)

- `2026-04-18` `1691b7ff` chore: remove GET /exchange-rate client usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3134d075` Update lockfile peer dependency metadata.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Merges (8)

- `2026-04-13` `fa88f895` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `83f48fc8` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `6a552b73` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `1acf7e62` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c237b7b6` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `ae705320` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `407b9d31` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `79af6117` Merge branch 'main' of https://github.com/liracards/Liravirtualmastercardwebapp into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (2)

- `2026-04-11` `b50baa64` Dockerfile: use node:alpine and nginx:alpine base images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `7e7f056f` Disable app mock mode for auth and cards flows.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/develop` (76)

#### Features (27)

- `2026-06-01` `bb2d3c36` feat(auth): default phone country to United States (+1) on login and signup  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-01` `b488e1b3` feat(kyc): respect server Tier 1 requiredChannels in profile UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `27137953` Add imageManager.sh for stage/prod Docker builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `85fe2168` feat: payment delegation UI, payer routes, and invoice management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `84641f29` feat: support staging deploy under /virtual/ path prefix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `400641f6` feat: Pay checkout discovery with currency and gateway selection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `eb34e22c` feat(post-purchase): nickname-only setup activates card without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `ab1bc1d9` feat(top-up): show IRR amounts and refresh expired quotes on pay  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `7ec902b8` feat(top-up): hide fees and load min/max from pricing API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `58116f6f` feat(cards): hide block and PIN actions from cards page toolbar  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `53e9bc56` feat(packages): hide fee row and include fee in IRR equivalent on package cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `3909eec1` feat(cards): load sensitive card details in modal via backend proxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `e3f5b46c` feat(cards): gateway PIN setup UX and fulfillment restart polish  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `b5fee756` feat(otp-ui): render resend countdown from backend timing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `e0aa746b` feat(cards): wire My Cards rename and PIN flows to API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `dfbf5693` feat(packages): payment method selection and live quote on confirm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `de5dc8ba` feat(kyc): Tier 1 gate, profile OTP, and resilient API loading  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `8e7dcec6` feat: buy-card USD/crypto, invoice crypto display, Iran phone validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67d30c23` feat: change-password API, transaction packages, and invoices  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `33d4169f` feat(packages): load pricing from API and restrict picker to active cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `f0189c9c` feat(topup): crypto invoice USD display, auto-refresh, cards reload after top-up  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8502861c` feat(top-up): dynamic pricing/quote API and clearer API errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1b8bfb5c` feat(web): load top-up pricing and quotes from backend  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d9b76b97` Docker and API client: env-aware builds, add image-manager script  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `4a4bad59` feat(auth): wire login/signup/reset flows to backend and env-configurable API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `2001b2c9` Add Docker and Nginx setup for web app deployment.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `f9a24b52` Update asset imports and add project gitignore.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (29)

- `2026-06-02` `dc99aa55` fix: redirect no-card users to active invoice fulfillment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `b4a66408` fix(onboarding-nav): prevent buy-card redirect loop on manual entry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `b3b210f9` fix(onboarding): route no-card users to status-aware destinations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `a9ad5574` fix(invoice): allow retry flow when canPay is only root-level  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `3fb4826c` fix(card-cap-ui): hide buy-card entry and block checkout at limit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `2454619c` fix: honor /virtual/panel base path for redirects and favicon  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `f98522fa` fix(transactions): map API fields for list tabs and refetch on transactions page  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `aafbf5c8` fix: stop transactions API loop and simplify help support tab  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `259774ff` fix(cards): show quota total at least as high as remaining from API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `ef388503` fix(buy-card): align issuance checkout with IRR and fixed USD quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c68ec553` fix(otp-ui): show expiry countdown and isolate resend state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c14cca62` fix(cards-ui): use profile maxCards instead of hardcoded cap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `98b8ddfc` fix(signup): remove national id step from registration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8f33137b` fix: sets default en langaufe  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `51efc346` fix(buy-card): remove redundant payment method subtitles  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `4967b531` fix(otp-ui): unify resend timer to MM:SS countdown  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `3ab7b957` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `263853b0` fix(invoices-ui): show IRR values and simplify top-up invoice lines  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34d8e3ad` fix(pwa): enforce network-only service worker and disable HTTP caching  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67c57b7f` fix(signup): clarify terms modal CTA copy in Persian  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `976efc58` fix: navigares to login pag e  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8ac3c9d6` fix(top-up): remove live USD/IRR rate line from card header  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `41c2afc1` fix(web): self-host Vazirmatn font for offline usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f17686f3` fix: align buy-card invoice flow with backend contracts  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `12f7e03c` fix(web): dedupe completeCardSetup and align develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `0214530a` fix: render invoice line items in invoice detail  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `9fb19808` fix(auth): clear session on public login/signup routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `44889604` fix: stop API error page reload loop (/app/*/error)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3ef774c0` Fix Persian font loading and RTL font application.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Refactors (1)

- `2026-06-02` `04a81f33` refine(invoice-ux): simplify status language and remove technical labels  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (2)

- `2026-04-18` `1691b7ff` chore: remove GET /exchange-rate client usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3134d075` Update lockfile peer dependency metadata.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Merges (8)

- `2026-04-13` `fa88f895` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `83f48fc8` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `6a552b73` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `1acf7e62` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c237b7b6` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `ae705320` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `407b9d31` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `79af6117` Merge branch 'main' of https://github.com/liracards/Liravirtualmastercardwebapp into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (9)

- `2026-06-02` `89149fc3` alll  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-06-02` `4071de8d` perf(invoices): consume assignment data from list payload  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `e56cecc3` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `6815fae2` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `24c4aabb` rebranding  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `0a360889` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `c678b2ff` Update Vite base path for stg.niwan.net/virtual/panel deploy.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `b50baa64` Dockerfile: use node:alpine and nginx:alpine base images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `7e7f056f` Disable app mock mode for auth and cards flows.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/docs/backend-clean-architecture` (2)

#### Features (1)

- `2026-03-31` `e0dae56d` Add backend clean architecture blueprint and baseline gitignore.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (1)

- `2026-03-31` `4733a8c2` Expand blueprint with delivery roadmap, team-based estimates, and scenario timelines.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/feat/topup-dynamic-pricing-quote` (50)

#### Features (18)

- `2026-05-17` `eb34e22c` feat(post-purchase): nickname-only setup activates card without PIN  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `58116f6f` feat(cards): hide block and PIN actions from cards page toolbar  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `3909eec1` feat(cards): load sensitive card details in modal via backend proxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `e3f5b46c` feat(cards): gateway PIN setup UX and fulfillment restart polish  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `b5fee756` feat(otp-ui): render resend countdown from backend timing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `e0aa746b` feat(cards): wire My Cards rename and PIN flows to API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `dfbf5693` feat(packages): payment method selection and live quote on confirm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `de5dc8ba` feat(kyc): Tier 1 gate, profile OTP, and resilient API loading  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `8e7dcec6` feat: buy-card USD/crypto, invoice crypto display, Iran phone validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67d30c23` feat: change-password API, transaction packages, and invoices  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `33d4169f` feat(packages): load pricing from API and restrict picker to active cards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `f0189c9c` feat(topup): crypto invoice USD display, auto-refresh, cards reload after top-up  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8502861c` feat(top-up): dynamic pricing/quote API and clearer API errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `1b8bfb5c` feat(web): load top-up pricing and quotes from backend  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `d9b76b97` Docker and API client: env-aware builds, add image-manager script  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `4a4bad59` feat(auth): wire login/signup/reset flows to backend and env-configurable API  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `2001b2c9` Add Docker and Nginx setup for web app deployment.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `f9a24b52` Update asset imports and add project gitignore.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (20)

- `2026-04-25` `ef388503` fix(buy-card): align issuance checkout with IRR and fixed USD quote  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c68ec553` fix(otp-ui): show expiry countdown and isolate resend state  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `c14cca62` fix(cards-ui): use profile maxCards instead of hardcoded cap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `98b8ddfc` fix(signup): remove national id step from registration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `8f33137b` fix: sets default en langaufe  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `51efc346` fix(buy-card): remove redundant payment method subtitles  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `4967b531` fix(otp-ui): unify resend timer to MM:SS countdown  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `3ab7b957` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `263853b0` fix(invoices-ui): show IRR values and simplify top-up invoice lines  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34d8e3ad` fix(pwa): enforce network-only service worker and disable HTTP caching  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-18` `67c57b7f` fix(signup): clarify terms modal CTA copy in Persian  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `976efc58` fix: navigares to login pag e  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `8ac3c9d6` fix(top-up): remove live USD/IRR rate line from card header  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `41c2afc1` fix(web): self-host Vazirmatn font for offline usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `f17686f3` fix: align buy-card invoice flow with backend contracts  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `12f7e03c` fix(web): dedupe completeCardSetup and align develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `0214530a` fix: render invoice line items in invoice detail  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `9fb19808` fix(auth): clear session on public login/signup routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `44889604` fix: stop API error page reload loop (/app/*/error)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3ef774c0` Fix Persian font loading and RTL font application.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (2)

- `2026-04-18` `1691b7ff` chore: remove GET /exchange-rate client usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `3134d075` Update lockfile peer dependency metadata.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Merges (8)

- `2026-04-13` `fa88f895` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `83f48fc8` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-13` `6a552b73` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-12` `1acf7e62` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `c237b7b6` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `ae705320` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-11` `407b9d31` Merge branch 'main' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-10` `79af6117` Merge branch 'main' of https://github.com/liracards/Liravirtualmastercardwebapp into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (2)

- `2026-04-11` `b50baa64` Dockerfile: use node:alpine and nginx:alpine base images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-09` `7e7f056f` Disable app mock mode for auth and cards flows.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## neivan-api-gateway

- Branches with matches: 4
- Commits listed in this repo section: 191

### Branch `main` (48)

#### Features (30)

- `2026-05-26` `556f6f2c` Add imageManager.sh for stage/prod API image publish.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `8986cb1d` feat(routes): allow full route updates for admin API set editing.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46f04e60` docs: add CORS example for panel-stg path-based gateway UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `a74bfc24` feat(usage): enrich usage API with display names for admin and tenant  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `90370d73` feat(routes): optional upstream path mapping for masked gateway paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `8bab35dc` feat(gateway): prefix route matching, query merge, upstream header controls  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `84b99c60` feat(gateway): structured trace logs and optional GATEWAY_DEBUG  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `aaa238b1` feat: tenant IP whitelist per API set, API set requirements, composed Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `1b5eeb66` feat: leacky bucket ratelimitng algorithm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `de4de9d3` feat: record and expose client ip in usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `cbbae0d0` feat: add admin and tenant ip whitelist management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `c662b171` feat: add admin replay revoke and tenant token self-service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `741f4f0d` feat: expose tenant ip whitelist read endpoint  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `35a9c547` feat: add route documentation backend and postman preview  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `f1745a58` docs: add API reference and Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `dde87817` feat: make API set tenant assignment replace existing mappings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `d441afd2` feat: add admin API set update and delete  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `93bfb8e0` feat: replay protection requires nonce + timestamp + signature  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `696ad692` feat: add CORS middleware for browser clients  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3faa6d4d` feat: generate replay secret route  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `35c2f33d` feat: add admin API set route update and delete  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `2c8bf138` feat: add migrate CLI and schema migrations for admin username and tenant password  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `0d63ab98` feat: support multi-tenant API set assignment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `f057d8c5` chore: introduce db-agnostic repo factory  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `ac544b5e` feat: add admin management and seed cli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `91e9219a` feat: add admin and tenant panel auth and harden gateway security  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `7ba5c901` feat: add gateway logging, metrics, and k8s health  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `4e233500` feat: pushing all changes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `4687e892` test: add usecase and repository coverage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `43307c52` test: add http delivery tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (7)

- `2026-05-13` `b16d87b4` fix(admin): normalize Postman prefix paths before validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `5fdd889c` fix(gateway): append path pattern to exact routes when backend base ends with /  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `48712bcb` docs: fix rate limiting mermaid diagram  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `a37a36fc` docs: add comprehensive README with diagrams and fix Dockerfile build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `d1d6386f` fix: fixes the /route problem  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `5fec4a36` fix: applies the gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `49aeb18c` fix: applies the gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (2)

- `2026-03-14` `fa2e22b3` Update docs and admin API components  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `f445e7a1` docs: summarize backend storyline features  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (9)

- `2026-03-19` `85984f3e` chore: update dockerfile and compose fil  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `1c3b350f` chore: updates dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `df94069c` chore: polish tenant routes and gateway cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `ec962125` chore: refactors main.go and adds redis health check to health api  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `df98e0bd` chore: harden config and security headers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `0a54d884` test: cover infra services, config, and app wiring  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `2030c373` chore: setups tool-agnostic and clean-architecure basic setups  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `bfb0e7ae` chore: creates base project structure  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `6c426cab` Stop tracking vendor/; keep deps via go.mod/go.sum  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `newgit/main` (47)

#### Features (29)

- `2026-05-24` `8986cb1d` feat(routes): allow full route updates for admin API set editing.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46f04e60` docs: add CORS example for panel-stg path-based gateway UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `a74bfc24` feat(usage): enrich usage API with display names for admin and tenant  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `90370d73` feat(routes): optional upstream path mapping for masked gateway paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `8bab35dc` feat(gateway): prefix route matching, query merge, upstream header controls  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `84b99c60` feat(gateway): structured trace logs and optional GATEWAY_DEBUG  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `aaa238b1` feat: tenant IP whitelist per API set, API set requirements, composed Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `1b5eeb66` feat: leacky bucket ratelimitng algorithm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `de4de9d3` feat: record and expose client ip in usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `cbbae0d0` feat: add admin and tenant ip whitelist management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `c662b171` feat: add admin replay revoke and tenant token self-service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `741f4f0d` feat: expose tenant ip whitelist read endpoint  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `35a9c547` feat: add route documentation backend and postman preview  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `f1745a58` docs: add API reference and Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `dde87817` feat: make API set tenant assignment replace existing mappings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `d441afd2` feat: add admin API set update and delete  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `93bfb8e0` feat: replay protection requires nonce + timestamp + signature  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `696ad692` feat: add CORS middleware for browser clients  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3faa6d4d` feat: generate replay secret route  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `35c2f33d` feat: add admin API set route update and delete  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `2c8bf138` feat: add migrate CLI and schema migrations for admin username and tenant password  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `0d63ab98` feat: support multi-tenant API set assignment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `f057d8c5` chore: introduce db-agnostic repo factory  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `ac544b5e` feat: add admin management and seed cli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `91e9219a` feat: add admin and tenant panel auth and harden gateway security  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `7ba5c901` feat: add gateway logging, metrics, and k8s health  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `4e233500` feat: pushing all changes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `4687e892` test: add usecase and repository coverage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `43307c52` test: add http delivery tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (7)

- `2026-05-13` `b16d87b4` fix(admin): normalize Postman prefix paths before validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `5fdd889c` fix(gateway): append path pattern to exact routes when backend base ends with /  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `48712bcb` docs: fix rate limiting mermaid diagram  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `a37a36fc` docs: add comprehensive README with diagrams and fix Dockerfile build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `d1d6386f` fix: fixes the /route problem  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `5fec4a36` fix: applies the gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `49aeb18c` fix: applies the gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (2)

- `2026-03-14` `fa2e22b3` Update docs and admin API components  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `f445e7a1` docs: summarize backend storyline features  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (9)

- `2026-03-19` `85984f3e` chore: update dockerfile and compose fil  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `1c3b350f` chore: updates dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `df94069c` chore: polish tenant routes and gateway cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `ec962125` chore: refactors main.go and adds redis health check to health api  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `df98e0bd` chore: harden config and security headers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `0a54d884` test: cover infra services, config, and app wiring  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `2030c373` chore: setups tool-agnostic and clean-architecure basic setups  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `bfb0e7ae` chore: creates base project structure  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `6c426cab` Stop tracking vendor/; keep deps via go.mod/go.sum  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/HEAD` (48)

#### Features (30)

- `2026-05-26` `556f6f2c` Add imageManager.sh for stage/prod API image publish.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `8986cb1d` feat(routes): allow full route updates for admin API set editing.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46f04e60` docs: add CORS example for panel-stg path-based gateway UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `a74bfc24` feat(usage): enrich usage API with display names for admin and tenant  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `90370d73` feat(routes): optional upstream path mapping for masked gateway paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `8bab35dc` feat(gateway): prefix route matching, query merge, upstream header controls  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `84b99c60` feat(gateway): structured trace logs and optional GATEWAY_DEBUG  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `aaa238b1` feat: tenant IP whitelist per API set, API set requirements, composed Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `1b5eeb66` feat: leacky bucket ratelimitng algorithm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `de4de9d3` feat: record and expose client ip in usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `cbbae0d0` feat: add admin and tenant ip whitelist management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `c662b171` feat: add admin replay revoke and tenant token self-service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `741f4f0d` feat: expose tenant ip whitelist read endpoint  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `35a9c547` feat: add route documentation backend and postman preview  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `f1745a58` docs: add API reference and Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `dde87817` feat: make API set tenant assignment replace existing mappings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `d441afd2` feat: add admin API set update and delete  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `93bfb8e0` feat: replay protection requires nonce + timestamp + signature  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `696ad692` feat: add CORS middleware for browser clients  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3faa6d4d` feat: generate replay secret route  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `35c2f33d` feat: add admin API set route update and delete  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `2c8bf138` feat: add migrate CLI and schema migrations for admin username and tenant password  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `0d63ab98` feat: support multi-tenant API set assignment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `f057d8c5` chore: introduce db-agnostic repo factory  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `ac544b5e` feat: add admin management and seed cli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `91e9219a` feat: add admin and tenant panel auth and harden gateway security  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `7ba5c901` feat: add gateway logging, metrics, and k8s health  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `4e233500` feat: pushing all changes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `4687e892` test: add usecase and repository coverage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `43307c52` test: add http delivery tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (7)

- `2026-05-13` `b16d87b4` fix(admin): normalize Postman prefix paths before validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `5fdd889c` fix(gateway): append path pattern to exact routes when backend base ends with /  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `48712bcb` docs: fix rate limiting mermaid diagram  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `a37a36fc` docs: add comprehensive README with diagrams and fix Dockerfile build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `d1d6386f` fix: fixes the /route problem  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `5fec4a36` fix: applies the gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `49aeb18c` fix: applies the gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (2)

- `2026-03-14` `fa2e22b3` Update docs and admin API components  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `f445e7a1` docs: summarize backend storyline features  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (9)

- `2026-03-19` `85984f3e` chore: update dockerfile and compose fil  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `1c3b350f` chore: updates dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `df94069c` chore: polish tenant routes and gateway cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `ec962125` chore: refactors main.go and adds redis health check to health api  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `df98e0bd` chore: harden config and security headers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `0a54d884` test: cover infra services, config, and app wiring  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `2030c373` chore: setups tool-agnostic and clean-architecure basic setups  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `bfb0e7ae` chore: creates base project structure  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `6c426cab` Stop tracking vendor/; keep deps via go.mod/go.sum  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (48)

#### Features (30)

- `2026-05-26` `556f6f2c` Add imageManager.sh for stage/prod API image publish.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `8986cb1d` feat(routes): allow full route updates for admin API set editing.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46f04e60` docs: add CORS example for panel-stg path-based gateway UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `a74bfc24` feat(usage): enrich usage API with display names for admin and tenant  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `90370d73` feat(routes): optional upstream path mapping for masked gateway paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `8bab35dc` feat(gateway): prefix route matching, query merge, upstream header controls  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `84b99c60` feat(gateway): structured trace logs and optional GATEWAY_DEBUG  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `aaa238b1` feat: tenant IP whitelist per API set, API set requirements, composed Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `1b5eeb66` feat: leacky bucket ratelimitng algorithm  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `de4de9d3` feat: record and expose client ip in usage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `cbbae0d0` feat: add admin and tenant ip whitelist management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `c662b171` feat: add admin replay revoke and tenant token self-service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `741f4f0d` feat: expose tenant ip whitelist read endpoint  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `35a9c547` feat: add route documentation backend and postman preview  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `f1745a58` docs: add API reference and Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `dde87817` feat: make API set tenant assignment replace existing mappings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `d441afd2` feat: add admin API set update and delete  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `93bfb8e0` feat: replay protection requires nonce + timestamp + signature  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `696ad692` feat: add CORS middleware for browser clients  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3faa6d4d` feat: generate replay secret route  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `35c2f33d` feat: add admin API set route update and delete  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `2c8bf138` feat: add migrate CLI and schema migrations for admin username and tenant password  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `0d63ab98` feat: support multi-tenant API set assignment  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `f057d8c5` chore: introduce db-agnostic repo factory  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `ac544b5e` feat: add admin management and seed cli  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `91e9219a` feat: add admin and tenant panel auth and harden gateway security  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `7ba5c901` feat: add gateway logging, metrics, and k8s health  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `4e233500` feat: pushing all changes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `4687e892` test: add usecase and repository coverage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `43307c52` test: add http delivery tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (7)

- `2026-05-13` `b16d87b4` fix(admin): normalize Postman prefix paths before validation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `5fdd889c` fix(gateway): append path pattern to exact routes when backend base ends with /  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `48712bcb` docs: fix rate limiting mermaid diagram  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `a37a36fc` docs: add comprehensive README with diagrams and fix Dockerfile build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `d1d6386f` fix: fixes the /route problem  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `5fec4a36` fix: applies the gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `49aeb18c` fix: applies the gitignore  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (2)

- `2026-03-14` `fa2e22b3` Update docs and admin API components  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `f445e7a1` docs: summarize backend storyline features  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (9)

- `2026-03-19` `85984f3e` chore: update dockerfile and compose fil  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `1c3b350f` chore: updates dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `df94069c` chore: polish tenant routes and gateway cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `ec962125` chore: refactors main.go and adds redis health check to health api  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `df98e0bd` chore: harden config and security headers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-09` `0a54d884` test: cover infra services, config, and app wiring  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `2030c373` chore: setups tool-agnostic and clean-architecure basic setups  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `bfb0e7ae` chore: creates base project structure  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-23` `6c426cab` Stop tracking vendor/; keep deps via go.mod/go.sum  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## neivan-api-gateway-interface

- Branches with matches: 4
- Commits listed in this repo section: 195

### Branch `main` (49)

#### Features (26)

- `2026-05-26` `e0138e11` Add imageManager.sh for stage/prod Next.js Docker builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `3af44dda` feat(admin): pre-populate and edit API set routes in edit modal.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `cff66789` feat: support path-based deploy under /gateway/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `933dd328` docs: add user journey guide with admin and tenant flow diagrams  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `aaea8998` feat(ui): surface path match type for gateway routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `7dea17fb` feat(postman-import): origin path mapping when gateway path differs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `9fa977de` feat: tenant IP whitelist per API set, client IP in usage, API set requirements, Postman download  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `093bb02e` feat: import routes from Postman (admin API set)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-13` `eead807b` feat: redirect to login on 401  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `e1536ddf` feat: add route documentation editor and viewer  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `de68b41f` docs: add project-specific readme  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `d7070b2b` feat: add replay secret management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `bed28246` feat: add admin and tenant ip whitelist management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `b9fc1f33` feat: compute replay signature in quick token  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `af77ec70` feat: upgrade quick token modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `7d614bd6` feat: add admin usage analytics tables  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `75d9ba50` feat: add usage date filters and docs coverage badges  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `70ee54c4` feat: add tenant api set routes modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `3475fa9b` feat: add tenant usage table  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `2c76dceb` feat: add api explorer, admin usage policies, and replay secret revoke  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `e6d1780e` feat: add edit/delete api-sets modals  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `6faa0b38` feat: add admin tenant creation flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `6885215e` feat: improve admin tenant modals and list  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `4cdbebec` feat: add api-set tenant assignment ui  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3768fd13` feat: add initial admin and tenant portals  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3133a673` feat: update routing and modal behavior  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (13)

- `2026-05-24` `845b635c` fix(admin): prefill and apply default backend URL on API set edit.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4566446a` fix: set trailingSlash when basePath is set for path deploy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `f86df57c` fix(admin): Postman import UX and create flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `8975fb89` fix(tenant-tokens): handle PascalCase create-token API response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `0a402170` fix(usage): map PascalCase API fields and show enriched usage columns  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `55cfc20a` fix: standalone build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `80b8f383` feat: Postman import on create/edit API set; usage policy scope selects; fix usage-policy reload loop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `feee1b61` fix: lock background scroll when modal open  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `ab22e5b8` fix: tenant usage filter button syntax  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `88838e6d` fix: quick token modal refactor  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `56c18a63` fix: tenant select selection logic and enabled replay-secret submit button  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `44db7d89` fix: correct modal loadin upon page refresh  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `339dec96` fix: surface backend error messages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (7)

- `2026-05-20` `9dec6eb9` chore(docker): use Docker Hub Node base image  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `dba68f40` chore: docker build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `8aacbfcc` chore: improve usage pagination and error ux  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `1a8b592d` chore: refresh tenant tokens after changes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `ebbd118a` chore: initial Next.js project scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `bb7b7003` chore: use select for route method  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `4b996254` chore: tweak api-set tenant assign modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-05-24` `a5d5b91f` Update staging basePath and API URL for stg.niwan.net gateway paths.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `cf1acd39` commit all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `b666801c` commit all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `newgit/main` (48)

#### Features (25)

- `2026-05-24` `3af44dda` feat(admin): pre-populate and edit API set routes in edit modal.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `cff66789` feat: support path-based deploy under /gateway/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `933dd328` docs: add user journey guide with admin and tenant flow diagrams  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `aaea8998` feat(ui): surface path match type for gateway routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `7dea17fb` feat(postman-import): origin path mapping when gateway path differs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `9fa977de` feat: tenant IP whitelist per API set, client IP in usage, API set requirements, Postman download  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `093bb02e` feat: import routes from Postman (admin API set)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-13` `eead807b` feat: redirect to login on 401  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `e1536ddf` feat: add route documentation editor and viewer  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `de68b41f` docs: add project-specific readme  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `d7070b2b` feat: add replay secret management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `bed28246` feat: add admin and tenant ip whitelist management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `b9fc1f33` feat: compute replay signature in quick token  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `af77ec70` feat: upgrade quick token modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `7d614bd6` feat: add admin usage analytics tables  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `75d9ba50` feat: add usage date filters and docs coverage badges  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `70ee54c4` feat: add tenant api set routes modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `3475fa9b` feat: add tenant usage table  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `2c76dceb` feat: add api explorer, admin usage policies, and replay secret revoke  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `e6d1780e` feat: add edit/delete api-sets modals  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `6faa0b38` feat: add admin tenant creation flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `6885215e` feat: improve admin tenant modals and list  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `4cdbebec` feat: add api-set tenant assignment ui  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3768fd13` feat: add initial admin and tenant portals  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3133a673` feat: update routing and modal behavior  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (13)

- `2026-05-24` `845b635c` fix(admin): prefill and apply default backend URL on API set edit.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4566446a` fix: set trailingSlash when basePath is set for path deploy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `f86df57c` fix(admin): Postman import UX and create flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `8975fb89` fix(tenant-tokens): handle PascalCase create-token API response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `0a402170` fix(usage): map PascalCase API fields and show enriched usage columns  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `55cfc20a` fix: standalone build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `80b8f383` feat: Postman import on create/edit API set; usage policy scope selects; fix usage-policy reload loop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `feee1b61` fix: lock background scroll when modal open  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `ab22e5b8` fix: tenant usage filter button syntax  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `88838e6d` fix: quick token modal refactor  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `56c18a63` fix: tenant select selection logic and enabled replay-secret submit button  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `44db7d89` fix: correct modal loadin upon page refresh  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `339dec96` fix: surface backend error messages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (7)

- `2026-05-20` `9dec6eb9` chore(docker): use Docker Hub Node base image  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `dba68f40` chore: docker build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `8aacbfcc` chore: improve usage pagination and error ux  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `1a8b592d` chore: refresh tenant tokens after changes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `ebbd118a` chore: initial Next.js project scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `bb7b7003` chore: use select for route method  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `4b996254` chore: tweak api-set tenant assign modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-05-24` `a5d5b91f` Update staging basePath and API URL for stg.niwan.net gateway paths.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `cf1acd39` commit all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `b666801c` commit all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/HEAD` (49)

#### Features (26)

- `2026-05-26` `e0138e11` Add imageManager.sh for stage/prod Next.js Docker builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `3af44dda` feat(admin): pre-populate and edit API set routes in edit modal.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `cff66789` feat: support path-based deploy under /gateway/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `933dd328` docs: add user journey guide with admin and tenant flow diagrams  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `aaea8998` feat(ui): surface path match type for gateway routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `7dea17fb` feat(postman-import): origin path mapping when gateway path differs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `9fa977de` feat: tenant IP whitelist per API set, client IP in usage, API set requirements, Postman download  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `093bb02e` feat: import routes from Postman (admin API set)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-13` `eead807b` feat: redirect to login on 401  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `e1536ddf` feat: add route documentation editor and viewer  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `de68b41f` docs: add project-specific readme  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `d7070b2b` feat: add replay secret management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `bed28246` feat: add admin and tenant ip whitelist management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `b9fc1f33` feat: compute replay signature in quick token  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `af77ec70` feat: upgrade quick token modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `7d614bd6` feat: add admin usage analytics tables  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `75d9ba50` feat: add usage date filters and docs coverage badges  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `70ee54c4` feat: add tenant api set routes modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `3475fa9b` feat: add tenant usage table  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `2c76dceb` feat: add api explorer, admin usage policies, and replay secret revoke  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `e6d1780e` feat: add edit/delete api-sets modals  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `6faa0b38` feat: add admin tenant creation flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `6885215e` feat: improve admin tenant modals and list  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `4cdbebec` feat: add api-set tenant assignment ui  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3768fd13` feat: add initial admin and tenant portals  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3133a673` feat: update routing and modal behavior  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (13)

- `2026-05-24` `845b635c` fix(admin): prefill and apply default backend URL on API set edit.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4566446a` fix: set trailingSlash when basePath is set for path deploy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `f86df57c` fix(admin): Postman import UX and create flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `8975fb89` fix(tenant-tokens): handle PascalCase create-token API response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `0a402170` fix(usage): map PascalCase API fields and show enriched usage columns  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `55cfc20a` fix: standalone build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `80b8f383` feat: Postman import on create/edit API set; usage policy scope selects; fix usage-policy reload loop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `feee1b61` fix: lock background scroll when modal open  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `ab22e5b8` fix: tenant usage filter button syntax  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `88838e6d` fix: quick token modal refactor  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `56c18a63` fix: tenant select selection logic and enabled replay-secret submit button  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `44db7d89` fix: correct modal loadin upon page refresh  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `339dec96` fix: surface backend error messages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (7)

- `2026-05-20` `9dec6eb9` chore(docker): use Docker Hub Node base image  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `dba68f40` chore: docker build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `8aacbfcc` chore: improve usage pagination and error ux  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `1a8b592d` chore: refresh tenant tokens after changes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `ebbd118a` chore: initial Next.js project scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `bb7b7003` chore: use select for route method  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `4b996254` chore: tweak api-set tenant assign modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-05-24` `a5d5b91f` Update staging basePath and API URL for stg.niwan.net gateway paths.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `cf1acd39` commit all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `b666801c` commit all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (49)

#### Features (26)

- `2026-05-26` `e0138e11` Add imageManager.sh for stage/prod Next.js Docker builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `3af44dda` feat(admin): pre-populate and edit API set routes in edit modal.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `cff66789` feat: support path-based deploy under /gateway/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-16` `933dd328` docs: add user journey guide with admin and tenant flow diagrams  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `aaea8998` feat(ui): surface path match type for gateway routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `7dea17fb` feat(postman-import): origin path mapping when gateway path differs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `9fa977de` feat: tenant IP whitelist per API set, client IP in usage, API set requirements, Postman download  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `093bb02e` feat: import routes from Postman (admin API set)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-13` `eead807b` feat: redirect to login on 401  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `e1536ddf` feat: add route documentation editor and viewer  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `de68b41f` docs: add project-specific readme  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `d7070b2b` feat: add replay secret management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `bed28246` feat: add admin and tenant ip whitelist management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `b9fc1f33` feat: compute replay signature in quick token  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `af77ec70` feat: upgrade quick token modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `7d614bd6` feat: add admin usage analytics tables  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `75d9ba50` feat: add usage date filters and docs coverage badges  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `70ee54c4` feat: add tenant api set routes modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `3475fa9b` feat: add tenant usage table  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `2c76dceb` feat: add api explorer, admin usage policies, and replay secret revoke  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `e6d1780e` feat: add edit/delete api-sets modals  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `6faa0b38` feat: add admin tenant creation flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `6885215e` feat: improve admin tenant modals and list  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `4cdbebec` feat: add api-set tenant assignment ui  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3768fd13` feat: add initial admin and tenant portals  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `3133a673` feat: update routing and modal behavior  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (13)

- `2026-05-24` `845b635c` fix(admin): prefill and apply default backend URL on API set edit.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4566446a` fix: set trailingSlash when basePath is set for path deploy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `f86df57c` fix(admin): Postman import UX and create flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `8975fb89` fix(tenant-tokens): handle PascalCase create-token API response  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-13` `0a402170` fix(usage): map PascalCase API fields and show enriched usage columns  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `55cfc20a` fix: standalone build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `80b8f383` feat: Postman import on create/edit API set; usage policy scope selects; fix usage-policy reload loop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `feee1b61` fix: lock background scroll when modal open  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `ab22e5b8` fix: tenant usage filter button syntax  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `88838e6d` fix: quick token modal refactor  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `56c18a63` fix: tenant select selection logic and enabled replay-secret submit button  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `44db7d89` fix: correct modal loadin upon page refresh  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `339dec96` fix: surface backend error messages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (7)

- `2026-05-20` `9dec6eb9` chore(docker): use Docker Hub Node base image  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `dba68f40` chore: docker build  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `8aacbfcc` chore: improve usage pagination and error ux  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-11` `1a8b592d` chore: refresh tenant tokens after changes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `ebbd118a` chore: initial Next.js project scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `bb7b7003` chore: use select for route method  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `4b996254` chore: tweak api-set tenant assign modal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-05-24` `a5d5b91f` Update staging basePath and API URL for stg.niwan.net gateway paths.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `cf1acd39` commit all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-10` `b666801c` commit all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## ingress-manifest

- Branches with matches: 2
- Commits listed in this repo section: 4

### Branch `main` (2)

#### Features (2)

- `2026-05-03` `b2384d52` Add modular HAProxy layouts: assembler, option-a, option-b  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-03` `93038956` Add .gitignore and clarify Git root for haproxy in README  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (2)

#### Features (2)

- `2026-05-03` `b2384d52` Add modular HAProxy layouts: assembler, option-a, option-b  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-03` `93038956` Add .gitignore and clarify Git root for haproxy in README  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## neivan-pay

- Branches with matches: 3
- Commits listed in this repo section: 112

### Branch `main` (38)

#### Features (24)

- `2026-06-02` `970f252f` docs: add merchant integration walkthrough  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `64134c5b` feat(admin): paginate payment intents and improve provider health checks  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `0c659dc9` Add imageManager.sh for core and swagger images.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `c89b451c` feat: polish Zibal return UX and auto-redirect on failure  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `50ab62b3` feat: Zibal browser return page and safer retry flows  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `f3d35049` feat: improve zibal hop page UX with payment context  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `834c21a0` docs: add staging path examples for CORS and API_PUBLIC_BASE_URL  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `fc0bae05` feat: add payment links with public redeem and polished amount form  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `c4a24f24` feat: multi-provider discovery, Trawili adapters, and faster health checks  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `83d27643` feat: per-app payment return URL and Zibal browser return handler  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `2d6a86fc` feat: per-app provider routes, IRR→Zibal migration, and payment debug logs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `fc2b9503` feat: expand pay API auth, reliability, and observability  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `efe97779` feat: add build metadata and detailed API request logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ad05895d` feat: add tenant and app admin CRUD APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `a5e70cc6` feat: add multi-admin management and persistent admin auth  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7c80ae21` feat: add webhook operations and subscription management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `5c412670` feat: add admin tenant and app creation endpoints  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `59c57741` feat: enrich admin provider health and simplify create payloads  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `58392fd8` feat: add in-container migration CLI for core service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `4b01ffb1` feat: separate admin auth from app integration tokens  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `38c3881c` feat: restrict issued app token access to payment flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `23599b84` feat: seed admin auth prerequisites in migrations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ee2eb9cf` Implement payment intent processing foundation and clean HTTP delivery structure.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `2cc7788c` Implement token management core with persistent idempotency and TDD coverage.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (9)

- `2026-06-02` `29e6ed2f` airwallex fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `437cd028` fix(worker): remove unused net/http import  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `ed3a69c3` fix: re-sign webhook payloads after JSONB storage round-trip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `c19758d4` fix: self-host Vazirmatn on Zibal hop page instead of Google Fonts  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `52ebae02` fix: global admin webhook deliveries and signature debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `44a1858b` fix: Trawili parsing, provider persistence, and admin intent listing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `16a5358c` fix: list all admin webhook subscriptions across tenants  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7b884d4c` fix: switch OpenAPI server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `30d2807a` fix: set explicit production server for OpenAPI docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (1)

- `2026-04-26` `5d353397` Initialize neivan-pay baseline docs and runtime assets.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-04-26` `a9effbe4` chore: update and push  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-06-02` `5a1ee50e` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `04393032` all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `b8f7dacb` Bootstrap neivan-pay runtime skeleton and contract artifacts.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `newgit/main` (36)

#### Features (23)

- `2026-05-31` `64134c5b` feat(admin): paginate payment intents and improve provider health checks  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `0c659dc9` Add imageManager.sh for core and swagger images.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `c89b451c` feat: polish Zibal return UX and auto-redirect on failure  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `50ab62b3` feat: Zibal browser return page and safer retry flows  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `f3d35049` feat: improve zibal hop page UX with payment context  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `834c21a0` docs: add staging path examples for CORS and API_PUBLIC_BASE_URL  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `fc0bae05` feat: add payment links with public redeem and polished amount form  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `c4a24f24` feat: multi-provider discovery, Trawili adapters, and faster health checks  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `83d27643` feat: per-app payment return URL and Zibal browser return handler  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `2d6a86fc` feat: per-app provider routes, IRR→Zibal migration, and payment debug logs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `fc2b9503` feat: expand pay API auth, reliability, and observability  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `efe97779` feat: add build metadata and detailed API request logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ad05895d` feat: add tenant and app admin CRUD APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `a5e70cc6` feat: add multi-admin management and persistent admin auth  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7c80ae21` feat: add webhook operations and subscription management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `5c412670` feat: add admin tenant and app creation endpoints  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `59c57741` feat: enrich admin provider health and simplify create payloads  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `58392fd8` feat: add in-container migration CLI for core service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `4b01ffb1` feat: separate admin auth from app integration tokens  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `38c3881c` feat: restrict issued app token access to payment flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `23599b84` feat: seed admin auth prerequisites in migrations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ee2eb9cf` Implement payment intent processing foundation and clean HTTP delivery structure.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `2cc7788c` Implement token management core with persistent idempotency and TDD coverage.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (8)

- `2026-05-31` `437cd028` fix(worker): remove unused net/http import  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `ed3a69c3` fix: re-sign webhook payloads after JSONB storage round-trip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `c19758d4` fix: self-host Vazirmatn on Zibal hop page instead of Google Fonts  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `52ebae02` fix: global admin webhook deliveries and signature debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `44a1858b` fix: Trawili parsing, provider persistence, and admin intent listing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `16a5358c` fix: list all admin webhook subscriptions across tenants  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7b884d4c` fix: switch OpenAPI server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `30d2807a` fix: set explicit production server for OpenAPI docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (1)

- `2026-04-26` `5d353397` Initialize neivan-pay baseline docs and runtime assets.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-04-26` `a9effbe4` chore: update and push  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-06-02` `5a1ee50e` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `04393032` all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `b8f7dacb` Bootstrap neivan-pay runtime skeleton and contract artifacts.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (38)

#### Features (24)

- `2026-06-02` `970f252f` docs: add merchant integration walkthrough  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `64134c5b` feat(admin): paginate payment intents and improve provider health checks  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `0c659dc9` Add imageManager.sh for core and swagger images.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `c89b451c` feat: polish Zibal return UX and auto-redirect on failure  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `50ab62b3` feat: Zibal browser return page and safer retry flows  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `f3d35049` feat: improve zibal hop page UX with payment context  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `834c21a0` docs: add staging path examples for CORS and API_PUBLIC_BASE_URL  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `fc0bae05` feat: add payment links with public redeem and polished amount form  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `c4a24f24` feat: multi-provider discovery, Trawili adapters, and faster health checks  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `83d27643` feat: per-app payment return URL and Zibal browser return handler  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `2d6a86fc` feat: per-app provider routes, IRR→Zibal migration, and payment debug logs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `fc2b9503` feat: expand pay API auth, reliability, and observability  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `efe97779` feat: add build metadata and detailed API request logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ad05895d` feat: add tenant and app admin CRUD APIs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `a5e70cc6` feat: add multi-admin management and persistent admin auth  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7c80ae21` feat: add webhook operations and subscription management  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `5c412670` feat: add admin tenant and app creation endpoints  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `59c57741` feat: enrich admin provider health and simplify create payloads  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `58392fd8` feat: add in-container migration CLI for core service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `4b01ffb1` feat: separate admin auth from app integration tokens  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `38c3881c` feat: restrict issued app token access to payment flow  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `23599b84` feat: seed admin auth prerequisites in migrations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ee2eb9cf` Implement payment intent processing foundation and clean HTTP delivery structure.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `2cc7788c` Implement token management core with persistent idempotency and TDD coverage.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (9)

- `2026-06-02` `29e6ed2f` airwallex fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `437cd028` fix(worker): remove unused net/http import  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `ed3a69c3` fix: re-sign webhook payloads after JSONB storage round-trip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `c19758d4` fix: self-host Vazirmatn on Zibal hop page instead of Google Fonts  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `52ebae02` fix: global admin webhook deliveries and signature debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `44a1858b` fix: Trawili parsing, provider persistence, and admin intent listing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `16a5358c` fix: list all admin webhook subscriptions across tenants  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7b884d4c` fix: switch OpenAPI server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `30d2807a` fix: set explicit production server for OpenAPI docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (1)

- `2026-04-26` `5d353397` Initialize neivan-pay baseline docs and runtime assets.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-04-26` `a9effbe4` chore: update and push  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (3)

- `2026-06-02` `5a1ee50e` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `04393032` all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `b8f7dacb` Bootstrap neivan-pay runtime skeleton and contract artifacts.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## neivan-pay-admin

- Branches with matches: 2
- Commits listed in this repo section: 58

### Branch `main` (29)

#### Features (15)

- `2026-05-31` `2803c293` feat: paginate payment intents list and refresh provider health UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `0b01f7cc` feat: optional Vite base path for Pay Admin path deploy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `eb1f4317` feat: improve payment intents list readability in Pay Admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `9b78a80e` feat: catalog-aware provider routes editor and local dev API proxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f19a2ada` feat: configure payment return URL per app in admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `ee740dc4` feat: manage per-app provider routes in Pay Admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ff6f74f8` feat: migrate admin console auth to X-Admin-Token routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ee4021e9` feat: add admin auth flow, i18n dates, and payment ops views  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ecd4a3a4` feat: add admin user management in admin panel  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `bf6ec6b1` feat: wire full admin route coverage in panel  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `a1287e79` feat: clarify issued token usage in admin token UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9fcc83b9` feat: show backend build id in admin footer  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9b430215` feat: add webhook deliveries and subscriptions admin pages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `884f5542` feat: add tenant and app CRUD management in admin UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `71555d5c` feat: dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (8)

- `2026-05-26` `61adc80e` Fix prod admin base path for respect.plus and harden Docker builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `c9f71b8c` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `b6674f02` fix(build): ship path-deploy Vite env via .env.production in Docker  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `76a1171d` feat: add payment links admin UI and fix provider catalog hook  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9d9e7b98` fix: allows .env file to be in docker build proccess  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7387d39b` fix: prevent webhook subscriptions page refetch loop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `3d74ac4f` fix: use tenant/app selects for webhook subscriptions  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `0d78db62` fix: align admin UI mappings and provider health display  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (2)

- `2026-05-20` `54e0de11` chore(docker): use Docker Hub for Node and nginx base images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `bc0919be` Build admin module shell with routed tenant/app/token views and API actions.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (4)

- `2026-05-31` `6d38712f` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `869210d1` Improve token issuance UX with selectable scopes and localized feedback.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `8498f1a5` Initialize neivan-pay-admin product and engineering specifications.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `51572c33` Bootstrap neivan-pay-admin architecture shell and UI foundations.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (29)

#### Features (15)

- `2026-05-31` `2803c293` feat: paginate payment intents list and refresh provider health UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `0b01f7cc` feat: optional Vite base path for Pay Admin path deploy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `eb1f4317` feat: improve payment intents list readability in Pay Admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `9b78a80e` feat: catalog-aware provider routes editor and local dev API proxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f19a2ada` feat: configure payment return URL per app in admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `ee740dc4` feat: manage per-app provider routes in Pay Admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ff6f74f8` feat: migrate admin console auth to X-Admin-Token routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ee4021e9` feat: add admin auth flow, i18n dates, and payment ops views  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ecd4a3a4` feat: add admin user management in admin panel  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `bf6ec6b1` feat: wire full admin route coverage in panel  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `a1287e79` feat: clarify issued token usage in admin token UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9fcc83b9` feat: show backend build id in admin footer  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9b430215` feat: add webhook deliveries and subscriptions admin pages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `884f5542` feat: add tenant and app CRUD management in admin UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `71555d5c` feat: dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (8)

- `2026-05-26` `61adc80e` Fix prod admin base path for respect.plus and harden Docker builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `c9f71b8c` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `b6674f02` fix(build): ship path-deploy Vite env via .env.production in Docker  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-19` `76a1171d` feat: add payment links admin UI and fix provider catalog hook  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9d9e7b98` fix: allows .env file to be in docker build proccess  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7387d39b` fix: prevent webhook subscriptions page refetch loop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `3d74ac4f` fix: use tenant/app selects for webhook subscriptions  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `0d78db62` fix: align admin UI mappings and provider health display  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (2)

- `2026-05-20` `54e0de11` chore(docker): use Docker Hub for Node and nginx base images  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `bc0919be` Build admin module shell with routed tenant/app/token views and API actions.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (4)

- `2026-05-31` `6d38712f` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `869210d1` Improve token issuance UX with selectable scopes and localized feedback.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `8498f1a5` Initialize neivan-pay-admin product and engineering specifications.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `51572c33` Bootstrap neivan-pay-admin architecture shell and UI foundations.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## neivan-pay-integrations

- Branches with matches: 2
- Commits listed in this repo section: 19

### Branch `main` (10)

#### Features (3)

- `2026-05-21` `bc035781` docs: add implementation plan with discovery in WooCommerce v1  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `b8ab23cd` docs: add implementation rules, testing policy, and engineering standards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `8dcdd076` feat: add PHP merchant SDK and WooCommerce gateway with discovery  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (4)

- `2026-05-31` `ad6b9259` fix(sdk): normalize money amounts and decode API envelopes safely  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-23` `55e15ec6` fix(woocommerce): make gateway available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `41dc26a1` fix(woocommerce): <your message>  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `0b520e47` fix(woocommerce): register Neivan Pay for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (1)

- `2026-05-21` `6d0889b6` docs: adopt supported PHP, WordPress, WooCommerce, and Joomla versions  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-05-21` `66e08ef2` chore: initial monorepo layout and SEP reference samples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (1)

- `2026-05-26` `27449036` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (9)

#### Features (3)

- `2026-05-21` `bc035781` docs: add implementation plan with discovery in WooCommerce v1  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `b8ab23cd` docs: add implementation rules, testing policy, and engineering standards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `8dcdd076` feat: add PHP merchant SDK and WooCommerce gateway with discovery  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (3)

- `2026-05-23` `55e15ec6` fix(woocommerce): make gateway available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `41dc26a1` fix(woocommerce): <your message>  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `0b520e47` fix(woocommerce): register Neivan Pay for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (1)

- `2026-05-21` `6d0889b6` docs: adopt supported PHP, WordPress, WooCommerce, and Joomla versions  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-05-21` `66e08ef2` chore: initial monorepo layout and SEP reference samples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (1)

- `2026-05-26` `27449036` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## neivan-production

- Branches with matches: 2
- Commits listed in this repo section: 10

### Branch `main` (5)

#### Other (5)

- `2026-06-02` `c92d9556` ssalam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `e7fd2fd6` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `b0a60060` update  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `e65baaf2` Initial production deployment layout from staging.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `32e5dbe0` Configure production for respect.plus behind Cloudflare.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (5)

#### Other (5)

- `2026-06-02` `c92d9556` ssalam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `e7fd2fd6` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `b0a60060` update  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `e65baaf2` Initial production deployment layout from staging.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `32e5dbe0` Configure production for respect.plus behind Cloudflare.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## neivan-stageing

- Branches with matches: 9
- Commits listed in this repo section: 671

### Branch `feat/pay-pgm-https-acme` (63)

#### Features (12)

- `2026-05-24` `457e9040` Add HTTPS for Pay API on ipg-stg.liracards.com (ACME / Let's Encrypt).  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `57c6aec7` feat(staging): add WooCommerce shop on panel-stg /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7ae07dba` feat(haproxy): route Neivan API Gateway on /gateway/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `48f2ccb1` feat(haproxy): route Lira virtual card on /virtual/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46c5050b` feat(haproxy): route Neivan Pay on /pay/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `336d0e0c` feat(haproxy): route docs-stg.niwan.net to Pay Swagger UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `fa741dde` feat(haproxy): route ipg.liracards.com to neivan-pay core  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `29a4eb30` chore: add pay swagger docs service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `04ca4e26` chore: add container-safe log file path to pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ef72e1aa` chore: add pay service stack to staging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `7ccebe98` chore: add virtual card admin service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `ed66249e` Add remote sync automation for staging workspace.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (21)

- `2026-05-21` `d47acc33` fix(wc-shop): trust HTTPS behind CDN (stop SSL redirect loop)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `804b9487` fix(wc-shop): WP 6.8, mount plugin on wpcli, harden bootstrap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `596fc630` fix(wc-shop): join wordpress to internal-shared for DB access  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `43054343` fix(wc-shop): stop HAProxy path strip; use Apache Alias /wc  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3dd00e3a` fix(wc-shop): Neivan Pay available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3d9d15f8` fix(wc-shop): stop redirect loop on /wc/wp-admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3823dd2e` fix(wc-shop): keep /wc prefix in WP admin redirects  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `febb0f86` fix(haproxy): keep /gateway prefix for Next.js panel on panel-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `c97f606c` fix(staging): serve Sunrate admin UI on admin-stg /sunrate/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `972b544e` fix(haproxy): serve Pay Swagger at docs-stg.niwan.net/pay/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `90e8a581` fix(haproxy): avoid /gateway redirect loop with Next basePath  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `859f6fdd` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `5150f919` fix: new ipg address  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `7fec8def` haproxy: route full panel-stg/api-stg host to 200cardwrapper (fix /assets 403)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ce958a59` fix: point pay swagger spec to API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9992ab21` fix: switch pay swagger server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `6d7bd855` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `32cce136` fix: adds docs to cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `f4058f84` fix 200cardwrapper env example db and server port  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4e48bef0` fixes 200cards sevice env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `180a72d8` Add two-step image sync and fix service image mappings.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (6)

- `2026-05-20` `7e385935` docs: clarify Pay Admin uses VITE_APP_BASE_PATH for /pay/ builds  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4f8ae807` docs(pay): align staging .env.example with path deploy and CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f1795d56` docs: document per-app payment return URL in Pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `1bac2fbd` docs: clarify Pay Zibal and Virtual Cards Neivan Pay staging env examples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `15339ace` docs(200cardwrapper): clarify CORS_ORIGINS for panel-stg vs api-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `13ef3a9e` docs(200cardwrapper): CORS_ORIGINS entries must not include URL paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (10)

- `2026-05-21` `bccd7252` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `9882fc07` chore(wc-shop): refresh vendored plugin for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `1ea536de` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `e3c15493` chore: sync pay OpenAPI contract updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `977f86c1` chore: sync staging pay OpenAPI with CRUD updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7ba25c59` chore: align staging pay spec with payment-only app token surface  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `53b5536a` chore: expand pay env example with auth and cors settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `2fcf2847` chore: sync staging OpenAPI for webhook operations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `ca53c77c` chore: updates virtual card service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34413c76` chore: regitsers niwan.net in haproxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (14)

- `2026-05-24` `487409d5` Rename Pay API host from ipg-stg to pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `25ce0f6a` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `e51b8e87` updates envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `478ce38b` commita  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-10` `c0229c99` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `9c514352` haproxy: 301 /sunrate to /sunrate/ on stg hosts for SPA basename  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `6db52801` haproxy: route api-stg/panel-stg /sunrate to 200cardwrapper with path strip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `544e2c91` reads images from registry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `90652728` updates ha proxy config  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4a53afc1` updates the virtual card service envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `69eae504` Initialize secure single-host staging deployment scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `5d5a7ad8` Improve HAProxy behind CDN, image sync, and origin logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `53f7b3f2` Keep environment files local and enforce env sync parity.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `228c7ac1` Set explicit API entrypoint for virtual-card core service.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `feat/pay-pgm-https-selfsigned` (63)

#### Features (12)

- `2026-05-24` `a9c9b498` Add HTTPS for Pay API on ipg-stg.liracards.com (self-signed).  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `57c6aec7` feat(staging): add WooCommerce shop on panel-stg /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7ae07dba` feat(haproxy): route Neivan API Gateway on /gateway/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `48f2ccb1` feat(haproxy): route Lira virtual card on /virtual/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46c5050b` feat(haproxy): route Neivan Pay on /pay/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `336d0e0c` feat(haproxy): route docs-stg.niwan.net to Pay Swagger UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `fa741dde` feat(haproxy): route ipg.liracards.com to neivan-pay core  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `29a4eb30` chore: add pay swagger docs service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `04ca4e26` chore: add container-safe log file path to pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ef72e1aa` chore: add pay service stack to staging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `7ccebe98` chore: add virtual card admin service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `ed66249e` Add remote sync automation for staging workspace.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (21)

- `2026-05-21` `d47acc33` fix(wc-shop): trust HTTPS behind CDN (stop SSL redirect loop)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `804b9487` fix(wc-shop): WP 6.8, mount plugin on wpcli, harden bootstrap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `596fc630` fix(wc-shop): join wordpress to internal-shared for DB access  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `43054343` fix(wc-shop): stop HAProxy path strip; use Apache Alias /wc  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3dd00e3a` fix(wc-shop): Neivan Pay available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3d9d15f8` fix(wc-shop): stop redirect loop on /wc/wp-admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3823dd2e` fix(wc-shop): keep /wc prefix in WP admin redirects  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `febb0f86` fix(haproxy): keep /gateway prefix for Next.js panel on panel-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `c97f606c` fix(staging): serve Sunrate admin UI on admin-stg /sunrate/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `972b544e` fix(haproxy): serve Pay Swagger at docs-stg.niwan.net/pay/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `90e8a581` fix(haproxy): avoid /gateway redirect loop with Next basePath  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `859f6fdd` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `5150f919` fix: new ipg address  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `7fec8def` haproxy: route full panel-stg/api-stg host to 200cardwrapper (fix /assets 403)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ce958a59` fix: point pay swagger spec to API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9992ab21` fix: switch pay swagger server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `6d7bd855` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `32cce136` fix: adds docs to cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `f4058f84` fix 200cardwrapper env example db and server port  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4e48bef0` fixes 200cards sevice env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `180a72d8` Add two-step image sync and fix service image mappings.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (6)

- `2026-05-20` `7e385935` docs: clarify Pay Admin uses VITE_APP_BASE_PATH for /pay/ builds  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4f8ae807` docs(pay): align staging .env.example with path deploy and CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f1795d56` docs: document per-app payment return URL in Pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `1bac2fbd` docs: clarify Pay Zibal and Virtual Cards Neivan Pay staging env examples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `15339ace` docs(200cardwrapper): clarify CORS_ORIGINS for panel-stg vs api-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `13ef3a9e` docs(200cardwrapper): CORS_ORIGINS entries must not include URL paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (10)

- `2026-05-21` `bccd7252` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `9882fc07` chore(wc-shop): refresh vendored plugin for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `1ea536de` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `e3c15493` chore: sync pay OpenAPI contract updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `977f86c1` chore: sync staging pay OpenAPI with CRUD updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7ba25c59` chore: align staging pay spec with payment-only app token surface  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `53b5536a` chore: expand pay env example with auth and cors settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `2fcf2847` chore: sync staging OpenAPI for webhook operations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `ca53c77c` chore: updates virtual card service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34413c76` chore: regitsers niwan.net in haproxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (14)

- `2026-05-24` `5ddf806f` Rename Pay API host from ipg-stg to pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `25ce0f6a` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `e51b8e87` updates envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `478ce38b` commita  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-10` `c0229c99` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `9c514352` haproxy: 301 /sunrate to /sunrate/ on stg hosts for SPA basename  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `6db52801` haproxy: route api-stg/panel-stg /sunrate to 200cardwrapper with path strip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `544e2c91` reads images from registry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `90652728` updates ha proxy config  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4a53afc1` updates the virtual card service envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `69eae504` Initialize secure single-host staging deployment scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `5d5a7ad8` Improve HAProxy behind CDN, image sync, and origin logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `53f7b3f2` Keep environment files local and enforce env sync parity.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `228c7ac1` Set explicit API entrypoint for virtual-card core service.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `main` (99)

#### Features (15)

- `2026-05-30` `bb23b555` Add prod infrastructure and dual-host HAProxy routing for gateway and wrapper.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `a10fb008` feat(wc-shop): improve Neivan Pay receipt UI and add Persian i18n  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `ba9fa6e9` Merge feat/pay-pgm-https-selfsigned: Pay API HTTPS on pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `a9c9b498` Add HTTPS for Pay API on ipg-stg.liracards.com (self-signed).  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `57c6aec7` feat(staging): add WooCommerce shop on panel-stg /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7ae07dba` feat(haproxy): route Neivan API Gateway on /gateway/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `48f2ccb1` feat(haproxy): route Lira virtual card on /virtual/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46c5050b` feat(haproxy): route Neivan Pay on /pay/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `336d0e0c` feat(haproxy): route docs-stg.niwan.net to Pay Swagger UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `fa741dde` feat(haproxy): route ipg.liracards.com to neivan-pay core  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `29a4eb30` chore: add pay swagger docs service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `04ca4e26` chore: add container-safe log file path to pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ef72e1aa` chore: add pay service stack to staging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `7ccebe98` chore: add virtual card admin service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `ed66249e` Add remote sync automation for staging workspace.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (40)

- `2026-05-30` `c5b81b2c` Fix gateway/sunrate routing when only prod containers run.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `9b4ce0e8` Fix db-copy-stg-to-prod corrupt dumps and pg_restore exit 139.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `8b0d3e1b` Fix WooCommerce redirect to use Zibal hop only for Zibal payments.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `78f5bd0f` Fix staging/prod gateway stacks clobbering each other in Compose.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `1110ebf8` Fix HAProxy gateway/wrapper routing after container rename.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `f7b07eae` fix(wc-shop): load Neivan Pay translations from site language on storefront  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `89184642` fix(wc-shop): simplify Pay Admin URLs in gateway settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `f899124f` fix: send cancelled Pay returns to order pay page, not thank-you  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `d1eeb14d` fix: stop mu-plugin rewriting Pay API redirect URLs to /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `b07d572a` fix: prefer Pay hop URL over misconfigured WC API base  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `a81ca045` fix: use Apache-safe WC return and webhook URLs under /wc alias  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `9d3f8112` fix: harden WC Zibal redirects and add opt-in debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `804165c9` fix: redirect legacy panel paths and favicon on stg.niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `7192b905` fix: send Zibal hop redirects to configured Pay API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `6be35972` fix: stop infinite redirect loop on failed Pay browser return  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `59694cdc` fix: WC Pay checkout retries, URL migration, and clearer errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `4078e066` fix: add WC browser return endpoint and Pay app setup docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `2d224088` fix: escape WORDPRESS_CONFIG_EXTRA so compose does not strip PHP vars  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `24f809cf` fix: always build absolute Zibal hop URL from WC Pay API base  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `d47acc33` fix(wc-shop): trust HTTPS behind CDN (stop SSL redirect loop)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `804b9487` fix(wc-shop): WP 6.8, mount plugin on wpcli, harden bootstrap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `596fc630` fix(wc-shop): join wordpress to internal-shared for DB access  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `43054343` fix(wc-shop): stop HAProxy path strip; use Apache Alias /wc  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3dd00e3a` fix(wc-shop): Neivan Pay available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3d9d15f8` fix(wc-shop): stop redirect loop on /wc/wp-admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3823dd2e` fix(wc-shop): keep /wc prefix in WP admin redirects  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `febb0f86` fix(haproxy): keep /gateway prefix for Next.js panel on panel-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `c97f606c` fix(staging): serve Sunrate admin UI on admin-stg /sunrate/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `972b544e` fix(haproxy): serve Pay Swagger at docs-stg.niwan.net/pay/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `90e8a581` fix(haproxy): avoid /gateway redirect loop with Next basePath  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `859f6fdd` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `5150f919` fix: new ipg address  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `7fec8def` haproxy: route full panel-stg/api-stg host to 200cardwrapper (fix /assets 403)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ce958a59` fix: point pay swagger spec to API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9992ab21` fix: switch pay swagger server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `6d7bd855` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `32cce136` fix: adds docs to cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `f4058f84` fix 200cardwrapper env example db and server port  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4e48bef0` fixes 200cards sevice env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `180a72d8` Add two-step image sync and fix service image mappings.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Refactors (1)

- `2026-05-24` `97aef035` Migrate staging to stg.niwan.net path routing and simplify HAProxy.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (8)

- `2026-05-24` `edb45e94` Expose Pay Swagger UI at pgm.liracards.com/docs/.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `3ca2ea2d` docs: document Neivan Pay webhook secret and debug env vars  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7e385935` docs: clarify Pay Admin uses VITE_APP_BASE_PATH for /pay/ builds  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4f8ae807` docs(pay): align staging .env.example with path deploy and CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f1795d56` docs: document per-app payment return URL in Pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `1bac2fbd` docs: clarify Pay Zibal and Virtual Cards Neivan Pay staging env examples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `15339ace` docs(200cardwrapper): clarify CORS_ORIGINS for panel-stg vs api-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `13ef3a9e` docs(200cardwrapper): CORS_ORIGINS entries must not include URL paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (10)

- `2026-05-21` `bccd7252` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `9882fc07` chore(wc-shop): refresh vendored plugin for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `1ea536de` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `e3c15493` chore: sync pay OpenAPI contract updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `977f86c1` chore: sync staging pay OpenAPI with CRUD updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7ba25c59` chore: align staging pay spec with payment-only app token surface  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `53b5536a` chore: expand pay env example with auth and cors settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `2fcf2847` chore: sync staging OpenAPI for webhook operations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `ca53c77c` chore: updates virtual card service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34413c76` chore: regitsers niwan.net in haproxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (25)

- `2026-05-31` `e2b14d5c` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `55865884` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `ad51da91` Set X-Forwarded-Proto on prod sunrate backends unconditionally.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `42c0879d` all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `a4bc5fe1` sss'  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `515ab9ff` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `8e0a4e91` sakam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `d2735c67` Document pgm HTTPS deploy without make on staging servers.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `bf57e3b2` all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `a0329609` Use pgm.liracards.com for dedicated Pay API host ACL on main.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `5ddf806f` Rename Pay API host from ipg-stg to pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `5d2bc509` Route pgm.liracards.com by path for Pay API and admin.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `25ce0f6a` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `e51b8e87` updates envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `478ce38b` commita  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-10` `c0229c99` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `9c514352` haproxy: 301 /sunrate to /sunrate/ on stg hosts for SPA basename  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `6db52801` haproxy: route api-stg/panel-stg /sunrate to 200cardwrapper with path strip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `544e2c91` reads images from registry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `90652728` updates ha proxy config  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4a53afc1` updates the virtual card service envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `69eae504` Initialize secure single-host staging deployment scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `5d5a7ad8` Improve HAProxy behind CDN, image sync, and origin logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `53f7b3f2` Keep environment files local and enforce env sync parity.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `228c7ac1` Set explicit API entrypoint for virtual-card core service.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `newgit/main` (97)

#### Features (15)

- `2026-05-30` `bb23b555` Add prod infrastructure and dual-host HAProxy routing for gateway and wrapper.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `a10fb008` feat(wc-shop): improve Neivan Pay receipt UI and add Persian i18n  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `ba9fa6e9` Merge feat/pay-pgm-https-selfsigned: Pay API HTTPS on pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `a9c9b498` Add HTTPS for Pay API on ipg-stg.liracards.com (self-signed).  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `57c6aec7` feat(staging): add WooCommerce shop on panel-stg /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7ae07dba` feat(haproxy): route Neivan API Gateway on /gateway/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `48f2ccb1` feat(haproxy): route Lira virtual card on /virtual/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46c5050b` feat(haproxy): route Neivan Pay on /pay/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `336d0e0c` feat(haproxy): route docs-stg.niwan.net to Pay Swagger UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `fa741dde` feat(haproxy): route ipg.liracards.com to neivan-pay core  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `29a4eb30` chore: add pay swagger docs service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `04ca4e26` chore: add container-safe log file path to pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ef72e1aa` chore: add pay service stack to staging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `7ccebe98` chore: add virtual card admin service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `ed66249e` Add remote sync automation for staging workspace.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (40)

- `2026-05-30` `c5b81b2c` Fix gateway/sunrate routing when only prod containers run.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `9b4ce0e8` Fix db-copy-stg-to-prod corrupt dumps and pg_restore exit 139.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `8b0d3e1b` Fix WooCommerce redirect to use Zibal hop only for Zibal payments.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `78f5bd0f` Fix staging/prod gateway stacks clobbering each other in Compose.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `1110ebf8` Fix HAProxy gateway/wrapper routing after container rename.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `f7b07eae` fix(wc-shop): load Neivan Pay translations from site language on storefront  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `89184642` fix(wc-shop): simplify Pay Admin URLs in gateway settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `f899124f` fix: send cancelled Pay returns to order pay page, not thank-you  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `d1eeb14d` fix: stop mu-plugin rewriting Pay API redirect URLs to /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `b07d572a` fix: prefer Pay hop URL over misconfigured WC API base  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `a81ca045` fix: use Apache-safe WC return and webhook URLs under /wc alias  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `9d3f8112` fix: harden WC Zibal redirects and add opt-in debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `804165c9` fix: redirect legacy panel paths and favicon on stg.niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `7192b905` fix: send Zibal hop redirects to configured Pay API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `6be35972` fix: stop infinite redirect loop on failed Pay browser return  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `59694cdc` fix: WC Pay checkout retries, URL migration, and clearer errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `4078e066` fix: add WC browser return endpoint and Pay app setup docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `2d224088` fix: escape WORDPRESS_CONFIG_EXTRA so compose does not strip PHP vars  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `24f809cf` fix: always build absolute Zibal hop URL from WC Pay API base  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `d47acc33` fix(wc-shop): trust HTTPS behind CDN (stop SSL redirect loop)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `804b9487` fix(wc-shop): WP 6.8, mount plugin on wpcli, harden bootstrap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `596fc630` fix(wc-shop): join wordpress to internal-shared for DB access  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `43054343` fix(wc-shop): stop HAProxy path strip; use Apache Alias /wc  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3dd00e3a` fix(wc-shop): Neivan Pay available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3d9d15f8` fix(wc-shop): stop redirect loop on /wc/wp-admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3823dd2e` fix(wc-shop): keep /wc prefix in WP admin redirects  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `febb0f86` fix(haproxy): keep /gateway prefix for Next.js panel on panel-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `c97f606c` fix(staging): serve Sunrate admin UI on admin-stg /sunrate/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `972b544e` fix(haproxy): serve Pay Swagger at docs-stg.niwan.net/pay/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `90e8a581` fix(haproxy): avoid /gateway redirect loop with Next basePath  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `859f6fdd` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `5150f919` fix: new ipg address  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `7fec8def` haproxy: route full panel-stg/api-stg host to 200cardwrapper (fix /assets 403)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ce958a59` fix: point pay swagger spec to API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9992ab21` fix: switch pay swagger server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `6d7bd855` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `32cce136` fix: adds docs to cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `f4058f84` fix 200cardwrapper env example db and server port  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4e48bef0` fixes 200cards sevice env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `180a72d8` Add two-step image sync and fix service image mappings.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Refactors (1)

- `2026-05-24` `97aef035` Migrate staging to stg.niwan.net path routing and simplify HAProxy.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (8)

- `2026-05-24` `edb45e94` Expose Pay Swagger UI at pgm.liracards.com/docs/.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `3ca2ea2d` docs: document Neivan Pay webhook secret and debug env vars  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7e385935` docs: clarify Pay Admin uses VITE_APP_BASE_PATH for /pay/ builds  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4f8ae807` docs(pay): align staging .env.example with path deploy and CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f1795d56` docs: document per-app payment return URL in Pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `1bac2fbd` docs: clarify Pay Zibal and Virtual Cards Neivan Pay staging env examples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `15339ace` docs(200cardwrapper): clarify CORS_ORIGINS for panel-stg vs api-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `13ef3a9e` docs(200cardwrapper): CORS_ORIGINS entries must not include URL paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (10)

- `2026-05-21` `bccd7252` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `9882fc07` chore(wc-shop): refresh vendored plugin for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `1ea536de` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `e3c15493` chore: sync pay OpenAPI contract updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `977f86c1` chore: sync staging pay OpenAPI with CRUD updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7ba25c59` chore: align staging pay spec with payment-only app token surface  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `53b5536a` chore: expand pay env example with auth and cors settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `2fcf2847` chore: sync staging OpenAPI for webhook operations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `ca53c77c` chore: updates virtual card service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34413c76` chore: regitsers niwan.net in haproxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (23)

- `2026-05-30` `ad51da91` Set X-Forwarded-Proto on prod sunrate backends unconditionally.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `42c0879d` all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `a4bc5fe1` sss'  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `515ab9ff` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `8e0a4e91` sakam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `d2735c67` Document pgm HTTPS deploy without make on staging servers.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `bf57e3b2` all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `a0329609` Use pgm.liracards.com for dedicated Pay API host ACL on main.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `5ddf806f` Rename Pay API host from ipg-stg to pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `5d2bc509` Route pgm.liracards.com by path for Pay API and admin.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `25ce0f6a` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `e51b8e87` updates envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `478ce38b` commita  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-10` `c0229c99` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `9c514352` haproxy: 301 /sunrate to /sunrate/ on stg hosts for SPA basename  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `6db52801` haproxy: route api-stg/panel-stg /sunrate to 200cardwrapper with path strip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `544e2c91` reads images from registry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `90652728` updates ha proxy config  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4a53afc1` updates the virtual card service envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `69eae504` Initialize secure single-host staging deployment scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `5d5a7ad8` Improve HAProxy behind CDN, image sync, and origin logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `53f7b3f2` Keep environment files local and enforce env sync parity.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `228c7ac1` Set explicit API entrypoint for virtual-card core service.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/feat/pay-ipg-stg-https-acme` (62)

#### Features (12)

- `2026-05-24` `457e9040` Add HTTPS for Pay API on ipg-stg.liracards.com (ACME / Let's Encrypt).  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `57c6aec7` feat(staging): add WooCommerce shop on panel-stg /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7ae07dba` feat(haproxy): route Neivan API Gateway on /gateway/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `48f2ccb1` feat(haproxy): route Lira virtual card on /virtual/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46c5050b` feat(haproxy): route Neivan Pay on /pay/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `336d0e0c` feat(haproxy): route docs-stg.niwan.net to Pay Swagger UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `fa741dde` feat(haproxy): route ipg.liracards.com to neivan-pay core  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `29a4eb30` chore: add pay swagger docs service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `04ca4e26` chore: add container-safe log file path to pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ef72e1aa` chore: add pay service stack to staging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `7ccebe98` chore: add virtual card admin service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `ed66249e` Add remote sync automation for staging workspace.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (21)

- `2026-05-21` `d47acc33` fix(wc-shop): trust HTTPS behind CDN (stop SSL redirect loop)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `804b9487` fix(wc-shop): WP 6.8, mount plugin on wpcli, harden bootstrap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `596fc630` fix(wc-shop): join wordpress to internal-shared for DB access  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `43054343` fix(wc-shop): stop HAProxy path strip; use Apache Alias /wc  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3dd00e3a` fix(wc-shop): Neivan Pay available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3d9d15f8` fix(wc-shop): stop redirect loop on /wc/wp-admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3823dd2e` fix(wc-shop): keep /wc prefix in WP admin redirects  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `febb0f86` fix(haproxy): keep /gateway prefix for Next.js panel on panel-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `c97f606c` fix(staging): serve Sunrate admin UI on admin-stg /sunrate/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `972b544e` fix(haproxy): serve Pay Swagger at docs-stg.niwan.net/pay/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `90e8a581` fix(haproxy): avoid /gateway redirect loop with Next basePath  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `859f6fdd` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `5150f919` fix: new ipg address  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `7fec8def` haproxy: route full panel-stg/api-stg host to 200cardwrapper (fix /assets 403)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ce958a59` fix: point pay swagger spec to API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9992ab21` fix: switch pay swagger server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `6d7bd855` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `32cce136` fix: adds docs to cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `f4058f84` fix 200cardwrapper env example db and server port  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4e48bef0` fixes 200cards sevice env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `180a72d8` Add two-step image sync and fix service image mappings.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (6)

- `2026-05-20` `7e385935` docs: clarify Pay Admin uses VITE_APP_BASE_PATH for /pay/ builds  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4f8ae807` docs(pay): align staging .env.example with path deploy and CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f1795d56` docs: document per-app payment return URL in Pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `1bac2fbd` docs: clarify Pay Zibal and Virtual Cards Neivan Pay staging env examples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `15339ace` docs(200cardwrapper): clarify CORS_ORIGINS for panel-stg vs api-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `13ef3a9e` docs(200cardwrapper): CORS_ORIGINS entries must not include URL paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (10)

- `2026-05-21` `bccd7252` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `9882fc07` chore(wc-shop): refresh vendored plugin for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `1ea536de` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `e3c15493` chore: sync pay OpenAPI contract updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `977f86c1` chore: sync staging pay OpenAPI with CRUD updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7ba25c59` chore: align staging pay spec with payment-only app token surface  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `53b5536a` chore: expand pay env example with auth and cors settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `2fcf2847` chore: sync staging OpenAPI for webhook operations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `ca53c77c` chore: updates virtual card service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34413c76` chore: regitsers niwan.net in haproxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (13)

- `2026-05-21` `25ce0f6a` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `e51b8e87` updates envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `478ce38b` commita  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-10` `c0229c99` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `9c514352` haproxy: 301 /sunrate to /sunrate/ on stg hosts for SPA basename  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `6db52801` haproxy: route api-stg/panel-stg /sunrate to 200cardwrapper with path strip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `544e2c91` reads images from registry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `90652728` updates ha proxy config  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4a53afc1` updates the virtual card service envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `69eae504` Initialize secure single-host staging deployment scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `5d5a7ad8` Improve HAProxy behind CDN, image sync, and origin logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `53f7b3f2` Keep environment files local and enforce env sync parity.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `228c7ac1` Set explicit API entrypoint for virtual-card core service.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/feat/pay-ipg-stg-https-selfsigned` (62)

#### Features (12)

- `2026-05-24` `a9c9b498` Add HTTPS for Pay API on ipg-stg.liracards.com (self-signed).  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `57c6aec7` feat(staging): add WooCommerce shop on panel-stg /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7ae07dba` feat(haproxy): route Neivan API Gateway on /gateway/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `48f2ccb1` feat(haproxy): route Lira virtual card on /virtual/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46c5050b` feat(haproxy): route Neivan Pay on /pay/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `336d0e0c` feat(haproxy): route docs-stg.niwan.net to Pay Swagger UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `fa741dde` feat(haproxy): route ipg.liracards.com to neivan-pay core  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `29a4eb30` chore: add pay swagger docs service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `04ca4e26` chore: add container-safe log file path to pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ef72e1aa` chore: add pay service stack to staging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `7ccebe98` chore: add virtual card admin service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `ed66249e` Add remote sync automation for staging workspace.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (21)

- `2026-05-21` `d47acc33` fix(wc-shop): trust HTTPS behind CDN (stop SSL redirect loop)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `804b9487` fix(wc-shop): WP 6.8, mount plugin on wpcli, harden bootstrap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `596fc630` fix(wc-shop): join wordpress to internal-shared for DB access  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `43054343` fix(wc-shop): stop HAProxy path strip; use Apache Alias /wc  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3dd00e3a` fix(wc-shop): Neivan Pay available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3d9d15f8` fix(wc-shop): stop redirect loop on /wc/wp-admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3823dd2e` fix(wc-shop): keep /wc prefix in WP admin redirects  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `febb0f86` fix(haproxy): keep /gateway prefix for Next.js panel on panel-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `c97f606c` fix(staging): serve Sunrate admin UI on admin-stg /sunrate/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `972b544e` fix(haproxy): serve Pay Swagger at docs-stg.niwan.net/pay/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `90e8a581` fix(haproxy): avoid /gateway redirect loop with Next basePath  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `859f6fdd` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `5150f919` fix: new ipg address  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `7fec8def` haproxy: route full panel-stg/api-stg host to 200cardwrapper (fix /assets 403)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ce958a59` fix: point pay swagger spec to API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9992ab21` fix: switch pay swagger server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `6d7bd855` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `32cce136` fix: adds docs to cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `f4058f84` fix 200cardwrapper env example db and server port  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4e48bef0` fixes 200cards sevice env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `180a72d8` Add two-step image sync and fix service image mappings.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (6)

- `2026-05-20` `7e385935` docs: clarify Pay Admin uses VITE_APP_BASE_PATH for /pay/ builds  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4f8ae807` docs(pay): align staging .env.example with path deploy and CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f1795d56` docs: document per-app payment return URL in Pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `1bac2fbd` docs: clarify Pay Zibal and Virtual Cards Neivan Pay staging env examples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `15339ace` docs(200cardwrapper): clarify CORS_ORIGINS for panel-stg vs api-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `13ef3a9e` docs(200cardwrapper): CORS_ORIGINS entries must not include URL paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (10)

- `2026-05-21` `bccd7252` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `9882fc07` chore(wc-shop): refresh vendored plugin for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `1ea536de` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `e3c15493` chore: sync pay OpenAPI contract updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `977f86c1` chore: sync staging pay OpenAPI with CRUD updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7ba25c59` chore: align staging pay spec with payment-only app token surface  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `53b5536a` chore: expand pay env example with auth and cors settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `2fcf2847` chore: sync staging OpenAPI for webhook operations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `ca53c77c` chore: updates virtual card service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34413c76` chore: regitsers niwan.net in haproxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (13)

- `2026-05-21` `25ce0f6a` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `e51b8e87` updates envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `478ce38b` commita  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-10` `c0229c99` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `9c514352` haproxy: 301 /sunrate to /sunrate/ on stg hosts for SPA basename  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `6db52801` haproxy: route api-stg/panel-stg /sunrate to 200cardwrapper with path strip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `544e2c91` reads images from registry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `90652728` updates ha proxy config  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4a53afc1` updates the virtual card service envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `69eae504` Initialize secure single-host staging deployment scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `5d5a7ad8` Improve HAProxy behind CDN, image sync, and origin logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `53f7b3f2` Keep environment files local and enforce env sync parity.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `228c7ac1` Set explicit API entrypoint for virtual-card core service.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/feat/pay-pgm-https-acme` (63)

#### Features (12)

- `2026-05-24` `457e9040` Add HTTPS for Pay API on ipg-stg.liracards.com (ACME / Let's Encrypt).  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `57c6aec7` feat(staging): add WooCommerce shop on panel-stg /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7ae07dba` feat(haproxy): route Neivan API Gateway on /gateway/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `48f2ccb1` feat(haproxy): route Lira virtual card on /virtual/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46c5050b` feat(haproxy): route Neivan Pay on /pay/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `336d0e0c` feat(haproxy): route docs-stg.niwan.net to Pay Swagger UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `fa741dde` feat(haproxy): route ipg.liracards.com to neivan-pay core  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `29a4eb30` chore: add pay swagger docs service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `04ca4e26` chore: add container-safe log file path to pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ef72e1aa` chore: add pay service stack to staging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `7ccebe98` chore: add virtual card admin service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `ed66249e` Add remote sync automation for staging workspace.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (21)

- `2026-05-21` `d47acc33` fix(wc-shop): trust HTTPS behind CDN (stop SSL redirect loop)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `804b9487` fix(wc-shop): WP 6.8, mount plugin on wpcli, harden bootstrap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `596fc630` fix(wc-shop): join wordpress to internal-shared for DB access  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `43054343` fix(wc-shop): stop HAProxy path strip; use Apache Alias /wc  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3dd00e3a` fix(wc-shop): Neivan Pay available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3d9d15f8` fix(wc-shop): stop redirect loop on /wc/wp-admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3823dd2e` fix(wc-shop): keep /wc prefix in WP admin redirects  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `febb0f86` fix(haproxy): keep /gateway prefix for Next.js panel on panel-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `c97f606c` fix(staging): serve Sunrate admin UI on admin-stg /sunrate/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `972b544e` fix(haproxy): serve Pay Swagger at docs-stg.niwan.net/pay/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `90e8a581` fix(haproxy): avoid /gateway redirect loop with Next basePath  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `859f6fdd` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `5150f919` fix: new ipg address  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `7fec8def` haproxy: route full panel-stg/api-stg host to 200cardwrapper (fix /assets 403)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ce958a59` fix: point pay swagger spec to API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9992ab21` fix: switch pay swagger server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `6d7bd855` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `32cce136` fix: adds docs to cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `f4058f84` fix 200cardwrapper env example db and server port  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4e48bef0` fixes 200cards sevice env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `180a72d8` Add two-step image sync and fix service image mappings.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (6)

- `2026-05-20` `7e385935` docs: clarify Pay Admin uses VITE_APP_BASE_PATH for /pay/ builds  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4f8ae807` docs(pay): align staging .env.example with path deploy and CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f1795d56` docs: document per-app payment return URL in Pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `1bac2fbd` docs: clarify Pay Zibal and Virtual Cards Neivan Pay staging env examples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `15339ace` docs(200cardwrapper): clarify CORS_ORIGINS for panel-stg vs api-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `13ef3a9e` docs(200cardwrapper): CORS_ORIGINS entries must not include URL paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (10)

- `2026-05-21` `bccd7252` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `9882fc07` chore(wc-shop): refresh vendored plugin for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `1ea536de` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `e3c15493` chore: sync pay OpenAPI contract updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `977f86c1` chore: sync staging pay OpenAPI with CRUD updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7ba25c59` chore: align staging pay spec with payment-only app token surface  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `53b5536a` chore: expand pay env example with auth and cors settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `2fcf2847` chore: sync staging OpenAPI for webhook operations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `ca53c77c` chore: updates virtual card service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34413c76` chore: regitsers niwan.net in haproxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (14)

- `2026-05-24` `487409d5` Rename Pay API host from ipg-stg to pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `25ce0f6a` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `e51b8e87` updates envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `478ce38b` commita  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-10` `c0229c99` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `9c514352` haproxy: 301 /sunrate to /sunrate/ on stg hosts for SPA basename  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `6db52801` haproxy: route api-stg/panel-stg /sunrate to 200cardwrapper with path strip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `544e2c91` reads images from registry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `90652728` updates ha proxy config  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4a53afc1` updates the virtual card service envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `69eae504` Initialize secure single-host staging deployment scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `5d5a7ad8` Improve HAProxy behind CDN, image sync, and origin logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `53f7b3f2` Keep environment files local and enforce env sync parity.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `228c7ac1` Set explicit API entrypoint for virtual-card core service.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/feat/pay-pgm-https-selfsigned` (63)

#### Features (12)

- `2026-05-24` `a9c9b498` Add HTTPS for Pay API on ipg-stg.liracards.com (self-signed).  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `57c6aec7` feat(staging): add WooCommerce shop on panel-stg /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7ae07dba` feat(haproxy): route Neivan API Gateway on /gateway/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `48f2ccb1` feat(haproxy): route Lira virtual card on /virtual/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46c5050b` feat(haproxy): route Neivan Pay on /pay/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `336d0e0c` feat(haproxy): route docs-stg.niwan.net to Pay Swagger UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `fa741dde` feat(haproxy): route ipg.liracards.com to neivan-pay core  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `29a4eb30` chore: add pay swagger docs service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `04ca4e26` chore: add container-safe log file path to pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ef72e1aa` chore: add pay service stack to staging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `7ccebe98` chore: add virtual card admin service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `ed66249e` Add remote sync automation for staging workspace.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (21)

- `2026-05-21` `d47acc33` fix(wc-shop): trust HTTPS behind CDN (stop SSL redirect loop)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `804b9487` fix(wc-shop): WP 6.8, mount plugin on wpcli, harden bootstrap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `596fc630` fix(wc-shop): join wordpress to internal-shared for DB access  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `43054343` fix(wc-shop): stop HAProxy path strip; use Apache Alias /wc  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3dd00e3a` fix(wc-shop): Neivan Pay available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3d9d15f8` fix(wc-shop): stop redirect loop on /wc/wp-admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3823dd2e` fix(wc-shop): keep /wc prefix in WP admin redirects  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `febb0f86` fix(haproxy): keep /gateway prefix for Next.js panel on panel-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `c97f606c` fix(staging): serve Sunrate admin UI on admin-stg /sunrate/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `972b544e` fix(haproxy): serve Pay Swagger at docs-stg.niwan.net/pay/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `90e8a581` fix(haproxy): avoid /gateway redirect loop with Next basePath  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `859f6fdd` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `5150f919` fix: new ipg address  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `7fec8def` haproxy: route full panel-stg/api-stg host to 200cardwrapper (fix /assets 403)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ce958a59` fix: point pay swagger spec to API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9992ab21` fix: switch pay swagger server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `6d7bd855` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `32cce136` fix: adds docs to cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `f4058f84` fix 200cardwrapper env example db and server port  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4e48bef0` fixes 200cards sevice env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `180a72d8` Add two-step image sync and fix service image mappings.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (6)

- `2026-05-20` `7e385935` docs: clarify Pay Admin uses VITE_APP_BASE_PATH for /pay/ builds  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4f8ae807` docs(pay): align staging .env.example with path deploy and CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f1795d56` docs: document per-app payment return URL in Pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `1bac2fbd` docs: clarify Pay Zibal and Virtual Cards Neivan Pay staging env examples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `15339ace` docs(200cardwrapper): clarify CORS_ORIGINS for panel-stg vs api-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `13ef3a9e` docs(200cardwrapper): CORS_ORIGINS entries must not include URL paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (10)

- `2026-05-21` `bccd7252` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `9882fc07` chore(wc-shop): refresh vendored plugin for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `1ea536de` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `e3c15493` chore: sync pay OpenAPI contract updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `977f86c1` chore: sync staging pay OpenAPI with CRUD updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7ba25c59` chore: align staging pay spec with payment-only app token surface  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `53b5536a` chore: expand pay env example with auth and cors settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `2fcf2847` chore: sync staging OpenAPI for webhook operations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `ca53c77c` chore: updates virtual card service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34413c76` chore: regitsers niwan.net in haproxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (14)

- `2026-05-24` `5ddf806f` Rename Pay API host from ipg-stg to pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `25ce0f6a` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `e51b8e87` updates envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `478ce38b` commita  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-10` `c0229c99` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `9c514352` haproxy: 301 /sunrate to /sunrate/ on stg hosts for SPA basename  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `6db52801` haproxy: route api-stg/panel-stg /sunrate to 200cardwrapper with path strip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `544e2c91` reads images from registry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `90652728` updates ha proxy config  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4a53afc1` updates the virtual card service envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `69eae504` Initialize secure single-host staging deployment scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `5d5a7ad8` Improve HAProxy behind CDN, image sync, and origin logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `53f7b3f2` Keep environment files local and enforce env sync parity.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `228c7ac1` Set explicit API entrypoint for virtual-card core service.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (99)

#### Features (15)

- `2026-05-30` `bb23b555` Add prod infrastructure and dual-host HAProxy routing for gateway and wrapper.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `a10fb008` feat(wc-shop): improve Neivan Pay receipt UI and add Persian i18n  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `ba9fa6e9` Merge feat/pay-pgm-https-selfsigned: Pay API HTTPS on pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `a9c9b498` Add HTTPS for Pay API on ipg-stg.liracards.com (self-signed).  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `57c6aec7` feat(staging): add WooCommerce shop on panel-stg /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7ae07dba` feat(haproxy): route Neivan API Gateway on /gateway/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `48f2ccb1` feat(haproxy): route Lira virtual card on /virtual/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `46c5050b` feat(haproxy): route Neivan Pay on /pay/ stg paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `336d0e0c` feat(haproxy): route docs-stg.niwan.net to Pay Swagger UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `fa741dde` feat(haproxy): route ipg.liracards.com to neivan-pay core  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `29a4eb30` chore: add pay swagger docs service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `04ca4e26` chore: add container-safe log file path to pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `ef72e1aa` chore: add pay service stack to staging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `7ccebe98` chore: add virtual card admin service and routing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `ed66249e` Add remote sync automation for staging workspace.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (40)

- `2026-05-30` `c5b81b2c` Fix gateway/sunrate routing when only prod containers run.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `9b4ce0e8` Fix db-copy-stg-to-prod corrupt dumps and pg_restore exit 139.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `8b0d3e1b` Fix WooCommerce redirect to use Zibal hop only for Zibal payments.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `78f5bd0f` Fix staging/prod gateway stacks clobbering each other in Compose.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `1110ebf8` Fix HAProxy gateway/wrapper routing after container rename.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `f7b07eae` fix(wc-shop): load Neivan Pay translations from site language on storefront  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `89184642` fix(wc-shop): simplify Pay Admin URLs in gateway settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `f899124f` fix: send cancelled Pay returns to order pay page, not thank-you  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `d1eeb14d` fix: stop mu-plugin rewriting Pay API redirect URLs to /wc/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `b07d572a` fix: prefer Pay hop URL over misconfigured WC API base  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `a81ca045` fix: use Apache-safe WC return and webhook URLs under /wc alias  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `9d3f8112` fix: harden WC Zibal redirects and add opt-in debug logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `804165c9` fix: redirect legacy panel paths and favicon on stg.niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `7192b905` fix: send Zibal hop redirects to configured Pay API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `6be35972` fix: stop infinite redirect loop on failed Pay browser return  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `59694cdc` fix: WC Pay checkout retries, URL migration, and clearer errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `4078e066` fix: add WC browser return endpoint and Pay app setup docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `2d224088` fix: escape WORDPRESS_CONFIG_EXTRA so compose does not strip PHP vars  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `24f809cf` fix: always build absolute Zibal hop URL from WC Pay API base  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `d47acc33` fix(wc-shop): trust HTTPS behind CDN (stop SSL redirect loop)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `804b9487` fix(wc-shop): WP 6.8, mount plugin on wpcli, harden bootstrap  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `596fc630` fix(wc-shop): join wordpress to internal-shared for DB access  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `43054343` fix(wc-shop): stop HAProxy path strip; use Apache Alias /wc  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3dd00e3a` fix(wc-shop): Neivan Pay available on Blocks Store API checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3d9d15f8` fix(wc-shop): stop redirect loop on /wc/wp-admin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `3823dd2e` fix(wc-shop): keep /wc prefix in WP admin redirects  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `febb0f86` fix(haproxy): keep /gateway prefix for Next.js panel on panel-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `c97f606c` fix(staging): serve Sunrate admin UI on admin-stg /sunrate/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `972b544e` fix(haproxy): serve Pay Swagger at docs-stg.niwan.net/pay/  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `90e8a581` fix(haproxy): avoid /gateway redirect loop with Next basePath  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `859f6fdd` fix  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-17` `5150f919` fix: new ipg address  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `7fec8def` haproxy: route full panel-stg/api-stg host to 200cardwrapper (fix /assets 403)  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `ce958a59` fix: point pay swagger spec to API host  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `9992ab21` fix: switch pay swagger server host to niwan.net  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `6d7bd855` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `32cce136` fix: adds docs to cors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `f4058f84` fix 200cardwrapper env example db and server port  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4e48bef0` fixes 200cards sevice env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `180a72d8` Add two-step image sync and fix service image mappings.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Refactors (1)

- `2026-05-24` `97aef035` Migrate staging to stg.niwan.net path routing and simplify HAProxy.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (8)

- `2026-05-24` `edb45e94` Expose Pay Swagger UI at pgm.liracards.com/docs/.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `3ca2ea2d` docs: document Neivan Pay webhook secret and debug env vars  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `7e385935` docs: clarify Pay Admin uses VITE_APP_BASE_PATH for /pay/ builds  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-20` `4f8ae807` docs(pay): align staging .env.example with path deploy and CORS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `f1795d56` docs: document per-app payment return URL in Pay env example  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `1bac2fbd` docs: clarify Pay Zibal and Virtual Cards Neivan Pay staging env examples  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `15339ace` docs(200cardwrapper): clarify CORS_ORIGINS for panel-stg vs api-stg  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `13ef3a9e` docs(200cardwrapper): CORS_ORIGINS entries must not include URL paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (10)

- `2026-05-21` `bccd7252` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `9882fc07` chore(wc-shop): refresh vendored plugin for Blocks checkout  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `1ea536de` chore(wc-shop): refresh vendored Neivan Pay plugin  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `e3c15493` chore: sync pay OpenAPI contract updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `977f86c1` chore: sync staging pay OpenAPI with CRUD updates  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `7ba25c59` chore: align staging pay spec with payment-only app token surface  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `53b5536a` chore: expand pay env example with auth and cors settings  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-27` `2fcf2847` chore: sync staging OpenAPI for webhook operations  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `ca53c77c` chore: updates virtual card service  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-20` `34413c76` chore: regitsers niwan.net in haproxy  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (25)

- `2026-05-31` `e2b14d5c` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-31` `55865884` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `ad51da91` Set X-Forwarded-Proto on prod sunrate backends unconditionally.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-30` `42c0879d` all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `a4bc5fe1` sss'  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-26` `515ab9ff` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-25` `8e0a4e91` sakam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `d2735c67` Document pgm HTTPS deploy without make on staging servers.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `bf57e3b2` all  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `a0329609` Use pgm.liracards.com for dedicated Pay API host ACL on main.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `5ddf806f` Rename Pay API host from ipg-stg to pgm.liracards.com.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-24` `5d2bc509` Route pgm.liracards.com by path for Pay API and admin.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-21` `25ce0f6a` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-18` `e51b8e87` updates envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `478ce38b` commita  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-10` `c0229c99` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `9c514352` haproxy: 301 /sunrate to /sunrate/ on stg hosts for SPA basename  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `6db52801` haproxy: route api-stg/panel-stg /sunrate to 200cardwrapper with path strip  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-17` `544e2c91` reads images from registry  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `90652728` updates ha proxy config  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `4a53afc1` updates the virtual card service envs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `69eae504` Initialize secure single-host staging deployment scaffold  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `5d5a7ad8` Improve HAProxy behind CDN, image sync, and origin logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `53f7b3f2` Keep environment files local and enforce env sync parity.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-14` `228c7ac1` Set explicit API entrypoint for virtual-card core service.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## new-ui

- Branches with matches: 7
- Commits listed in this repo section: 33

### Branch `feat/reset-password-activeDatetime-timezone` (3)

#### Features (1)

- `2026-05-19` `cd73a2f5` chore: add package-lock.json for reproducible npm installs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (1)

- `2026-05-19` `ebca1a92` Fix reset password set-new-password request payload.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-05-20` `08c54056` chore(git): ignore .env and release tarballs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/develop` (13)

#### Features (3)

- `2026-04-26` `eae11953` add env files for API base url  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `d23d9500` Merge branch 'feature/login-email-phone-tabs' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `9da43468` Merge branch 'chore/add-api-base-url-env' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (8)

- `2026-05-12` `d51b1013` fix: correct backend url  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-02` `fd2a5c8c` fix: display card PAN left-to-right in RTL locales  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-02` `bde0b208` fix: revert changes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-02` `0b99d2ea` fix: handles card number presentation on fa lanugage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-29` `f9876a2d` fix: enforce required fields and correct signup payload  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-29` `afa9229e` fix: align login mobile field names  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-29` `39ba4ffd` fix: send normalized phone fields for login  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `379e4ac4` fix: signup page revert back to email and phone selection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (2)

- `2026-04-26` `4cf81b19` update gitignore env file rules  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `edb166d9` enable email and phone login tabs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/feat/reset-password-activeDatetime-timezone` (3)

#### Features (1)

- `2026-05-19` `cd73a2f5` chore: add package-lock.json for reproducible npm installs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (1)

- `2026-05-19` `ebca1a92` Fix reset password set-new-password request payload.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-05-20` `08c54056` chore(git): ignore .env and release tarballs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/feature/login-email-phone-tabs` (1)

#### Other (1)

- `2026-04-25` `edb166d9` enable email and phone login tabs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/fix-card-number-presentation-on-fa-langauage` (1)

#### Bug Fixes (1)

- `2026-05-02` `c4199e2f` fix: handles card number presentation on fa lanugage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/fix/cards-rtl-card-number` (11)

#### Features (3)

- `2026-04-26` `eae11953` add env files for API base url  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `d23d9500` Merge branch 'feature/login-email-phone-tabs' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `9da43468` Merge branch 'chore/add-api-base-url-env' into develop  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (6)

- `2026-05-02` `fd2a5c8c` fix: display card PAN left-to-right in RTL locales  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-02` `06ca55dd` fix: handles card number presentation on fa lanugage  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-29` `f9876a2d` fix: enforce required fields and correct signup payload  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-29` `afa9229e` fix: align login mobile field names  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-29` `39ba4ffd` fix: send normalized phone fields for login  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-26` `379e4ac4` fix: signup page revert back to email and phone selection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (2)

- `2026-04-26` `4cf81b19` update gitignore env file rules  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-25` `edb166d9` enable email and phone login tabs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/hotfix/remove-set-password-datetime-fields` (1)

#### Features (1)

- `2026-05-15` `29c9ea63` Remove activeDatetime and timezone from set-new-password request.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## observability-stack

- Branches with matches: 2
- Commits listed in this repo section: 24

### Branch `main` (12)

#### Features (3)

- `2026-05-09` `cdf54622` feat: expand dashboard filters for fleet log exploration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `87d386ff` feat: add docker-based fleet log management and dashboards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `58b8d0ae` feat: improve service naming and add log level filtering  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (6)

- `2026-05-09` `fca33bff` fix: correct alloy static label map syntax  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `f5383aa9` fix: use custom level variable for dashboard filtering  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `d9c07fbc` fix: correct deploy bind mount paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `b4f57e6d` fix: harden dashboard loki selectors for all-values  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `5d3a469e` fix: add local alloy static labels for dashboard filters  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `5943f1b8` fix: align stack logs dashboard with service_name labels  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-05-04` `efc0b9f6` chore: updates repo  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (2)

- `2026-05-10` `af41251d` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `a13eb8b5` observability: Lira file logs to Loki, fleet files renderer, Grafana multi-tenant  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (12)

#### Features (3)

- `2026-05-09` `cdf54622` feat: expand dashboard filters for fleet log exploration  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `87d386ff` feat: add docker-based fleet log management and dashboards  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `58b8d0ae` feat: improve service naming and add log level filtering  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (6)

- `2026-05-09` `fca33bff` fix: correct alloy static label map syntax  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `f5383aa9` fix: use custom level variable for dashboard filtering  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `d9c07fbc` fix: correct deploy bind mount paths  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `b4f57e6d` fix: harden dashboard loki selectors for all-values  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `5d3a469e` fix: add local alloy static labels for dashboard filters  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `5943f1b8` fix: align stack logs dashboard with service_name labels  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-05-04` `efc0b9f6` chore: updates repo  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (2)

- `2026-05-10` `af41251d` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-09` `a13eb8b5` observability: Lira file logs to Loki, fleet files renderer, Grafana multi-tenant  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## sunrate-proxy

- Branches with matches: 4
- Commits listed in this repo section: 166

### Branch `main` (43)

#### Features (11)

- `2026-05-26` `ff93cb6f` Add imageManager.sh for stage/prod surate-proxy images.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `356996ab` chore: add detailed CORS and USD proxy debug logs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `788ebb7f` Add DevOps and maintenance diagrams  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `614979eb` feat: per-tenant upstream credentials, tenant manager, and tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `5c693fd5` Add 200cards upstream Postman collection reference  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `235f9423` feat(admin): one-time password reveal for tenants  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `1e83d56a` feat(admin): tenant create, credential sync, and JWT cache invalidation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-13` `7d4f92fa` docs: add Sunrate proxy API docs and Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `b1e1ba18` Add tests: proxy, auth, config, system handler, repositories  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `f65699b8` Add bootstrap login debug logging and app restart policy in docker-compose  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b4000fc3` Add admin API and CORS: /admin/api-keys, user-identifiers, issued-cards; CORS_ORIGINS in .env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (12)

- `2026-05-11` `f5fef9d1` fix(cors): apply Allow-Origin on first WriteHeader/Write, not at request start  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `844a7d23` fix(proxy): stop forwarding browser headers to 200cards upstream  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `75776708` fix(cors): do not send mismatched Allow-Origin for unknown browsers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `20a0b95b` fix(usdcards): sanitize upstream response headers for proxied body  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `a2f5c08b` Fix Mermaid diagram rendering in GitHub rich display  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `f4beb2a6` fix: PIN routes use card_id/card_pin and card_id/old_pin/new_pin; sanitize payload for jsonb; doc and Postman  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `dbf11c61` fix: allow User-Identifier header in CORS for automation tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `154d61f7` Add server logging, issued-card storage fixes, and user-identifier upsert  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `50d06236` fix: quote Mermaid node labels to fix GitHub render parse error  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `b81a92a8` fix: diagram  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `23861669` Fix Mermaid diagram for GitHub rendering  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `1d605aef` Fix Mermaid request flow diagram for GitHub  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (4)

- `2026-03-29` `78a42913` Align USD proxy with 200cards; log upstream bodies; automation docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `1103f028` docs: automation tests – require request-status polling and client_request_id formats for async steps  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `926d519d` Document architecture, PRD, and request flows in README  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `223e0976` README: token TTL/renewal/retry, camelCase admin API, config table, run note  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (5)

- `2026-03-19` `958a7606` chore: updates compose file  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `3cf47fc4` chore: updates dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b1120bee` Bump Go version to 1.24 in go.mod  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `5b651925` Initial commit: Go proxy for 200cards API with health, USD card routes, API key auth, user-identifier tracking, create-card audit, Postgres/GORM, Docker  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `410b3cb5` Go 1.26: bump go.mod and Dockerfile; use 1.22+ method/path routing and PathValue  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (11)

- `2026-04-15` `30d51189` Include gen-apikey binary in runtime image  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `11399ad2` proxy over tcp nd ipv4  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `b80cd911` check  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `9a23f202` salam 2  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `4c0fdb09` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `450628dd` salam22  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `2ab813ae` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `557c7af7` log login response body only on non-2xx status  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `b2c5d1e2` Token TTL from env, renewal before expiry, retry login with backoff  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `40b00d25` Parse JWT exp claim for token expiry; fallback to LOGIN_TOKEN_TTL when missing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b5f755e0` Go 1.21 routes: path-only patterns + RequireMethod; admin responses camelCase, no KeyHash; bootstrap login non-fatal; CORS on all routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `newgit/main` (37)

#### Features (9)

- `2026-03-30` `788ebb7f` Add DevOps and maintenance diagrams  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `614979eb` feat: per-tenant upstream credentials, tenant manager, and tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `5c693fd5` Add 200cards upstream Postman collection reference  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `235f9423` feat(admin): one-time password reveal for tenants  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `1e83d56a` feat(admin): tenant create, credential sync, and JWT cache invalidation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-13` `7d4f92fa` docs: add Sunrate proxy API docs and Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `b1e1ba18` Add tests: proxy, auth, config, system handler, repositories  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `f65699b8` Add bootstrap login debug logging and app restart policy in docker-compose  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b4000fc3` Add admin API and CORS: /admin/api-keys, user-identifiers, issued-cards; CORS_ORIGINS in .env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (8)

- `2026-03-30` `a2f5c08b` Fix Mermaid diagram rendering in GitHub rich display  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `f4beb2a6` fix: PIN routes use card_id/card_pin and card_id/old_pin/new_pin; sanitize payload for jsonb; doc and Postman  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `dbf11c61` fix: allow User-Identifier header in CORS for automation tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `154d61f7` Add server logging, issued-card storage fixes, and user-identifier upsert  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `50d06236` fix: quote Mermaid node labels to fix GitHub render parse error  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `b81a92a8` fix: diagram  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `23861669` Fix Mermaid diagram for GitHub rendering  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `1d605aef` Fix Mermaid request flow diagram for GitHub  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (4)

- `2026-03-29` `78a42913` Align USD proxy with 200cards; log upstream bodies; automation docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `1103f028` docs: automation tests – require request-status polling and client_request_id formats for async steps  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `926d519d` Document architecture, PRD, and request flows in README  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `223e0976` README: token TTL/renewal/retry, camelCase admin API, config table, run note  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (5)

- `2026-03-19` `958a7606` chore: updates compose file  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `3cf47fc4` chore: updates dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b1120bee` Bump Go version to 1.24 in go.mod  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `5b651925` Initial commit: Go proxy for 200cards API with health, USD card routes, API key auth, user-identifier tracking, create-card audit, Postgres/GORM, Docker  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `410b3cb5` Go 1.26: bump go.mod and Dockerfile; use 1.22+ method/path routing and PathValue  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (11)

- `2026-04-15` `30d51189` Include gen-apikey binary in runtime image  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `11399ad2` proxy over tcp nd ipv4  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `b80cd911` check  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `9a23f202` salam 2  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `4c0fdb09` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `450628dd` salam22  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `2ab813ae` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `557c7af7` log login response body only on non-2xx status  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `b2c5d1e2` Token TTL from env, renewal before expiry, retry login with backoff  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `40b00d25` Parse JWT exp claim for token expiry; fallback to LOGIN_TOKEN_TTL when missing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b5f755e0` Go 1.21 routes: path-only patterns + RequireMethod; admin responses camelCase, no KeyHash; bootstrap login non-fatal; CORS on all routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/HEAD` (43)

#### Features (11)

- `2026-05-26` `ff93cb6f` Add imageManager.sh for stage/prod surate-proxy images.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `356996ab` chore: add detailed CORS and USD proxy debug logs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `788ebb7f` Add DevOps and maintenance diagrams  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `614979eb` feat: per-tenant upstream credentials, tenant manager, and tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `5c693fd5` Add 200cards upstream Postman collection reference  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `235f9423` feat(admin): one-time password reveal for tenants  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `1e83d56a` feat(admin): tenant create, credential sync, and JWT cache invalidation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-13` `7d4f92fa` docs: add Sunrate proxy API docs and Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `b1e1ba18` Add tests: proxy, auth, config, system handler, repositories  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `f65699b8` Add bootstrap login debug logging and app restart policy in docker-compose  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b4000fc3` Add admin API and CORS: /admin/api-keys, user-identifiers, issued-cards; CORS_ORIGINS in .env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (12)

- `2026-05-11` `f5fef9d1` fix(cors): apply Allow-Origin on first WriteHeader/Write, not at request start  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `844a7d23` fix(proxy): stop forwarding browser headers to 200cards upstream  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `75776708` fix(cors): do not send mismatched Allow-Origin for unknown browsers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `20a0b95b` fix(usdcards): sanitize upstream response headers for proxied body  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `a2f5c08b` Fix Mermaid diagram rendering in GitHub rich display  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `f4beb2a6` fix: PIN routes use card_id/card_pin and card_id/old_pin/new_pin; sanitize payload for jsonb; doc and Postman  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `dbf11c61` fix: allow User-Identifier header in CORS for automation tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `154d61f7` Add server logging, issued-card storage fixes, and user-identifier upsert  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `50d06236` fix: quote Mermaid node labels to fix GitHub render parse error  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `b81a92a8` fix: diagram  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `23861669` Fix Mermaid diagram for GitHub rendering  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `1d605aef` Fix Mermaid request flow diagram for GitHub  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (4)

- `2026-03-29` `78a42913` Align USD proxy with 200cards; log upstream bodies; automation docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `1103f028` docs: automation tests – require request-status polling and client_request_id formats for async steps  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `926d519d` Document architecture, PRD, and request flows in README  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `223e0976` README: token TTL/renewal/retry, camelCase admin API, config table, run note  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (5)

- `2026-03-19` `958a7606` chore: updates compose file  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `3cf47fc4` chore: updates dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b1120bee` Bump Go version to 1.24 in go.mod  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `5b651925` Initial commit: Go proxy for 200cards API with health, USD card routes, API key auth, user-identifier tracking, create-card audit, Postgres/GORM, Docker  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `410b3cb5` Go 1.26: bump go.mod and Dockerfile; use 1.22+ method/path routing and PathValue  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (11)

- `2026-04-15` `30d51189` Include gen-apikey binary in runtime image  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `11399ad2` proxy over tcp nd ipv4  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `b80cd911` check  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `9a23f202` salam 2  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `4c0fdb09` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `450628dd` salam22  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `2ab813ae` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `557c7af7` log login response body only on non-2xx status  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `b2c5d1e2` Token TTL from env, renewal before expiry, retry login with backoff  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `40b00d25` Parse JWT exp claim for token expiry; fallback to LOGIN_TOKEN_TTL when missing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b5f755e0` Go 1.21 routes: path-only patterns + RequireMethod; admin responses camelCase, no KeyHash; bootstrap login non-fatal; CORS on all routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (43)

#### Features (11)

- `2026-05-26` `ff93cb6f` Add imageManager.sh for stage/prod surate-proxy images.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `356996ab` chore: add detailed CORS and USD proxy debug logs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `788ebb7f` Add DevOps and maintenance diagrams  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `614979eb` feat: per-tenant upstream credentials, tenant manager, and tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `5c693fd5` Add 200cards upstream Postman collection reference  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `235f9423` feat(admin): one-time password reveal for tenants  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `1e83d56a` feat(admin): tenant create, credential sync, and JWT cache invalidation  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-13` `7d4f92fa` docs: add Sunrate proxy API docs and Postman collection  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `b1e1ba18` Add tests: proxy, auth, config, system handler, repositories  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `f65699b8` Add bootstrap login debug logging and app restart policy in docker-compose  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b4000fc3` Add admin API and CORS: /admin/api-keys, user-identifiers, issued-cards; CORS_ORIGINS in .env  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (12)

- `2026-05-11` `f5fef9d1` fix(cors): apply Allow-Origin on first WriteHeader/Write, not at request start  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `844a7d23` fix(proxy): stop forwarding browser headers to 200cards upstream  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `75776708` fix(cors): do not send mismatched Allow-Origin for unknown browsers  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-11` `20a0b95b` fix(usdcards): sanitize upstream response headers for proxied body  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `a2f5c08b` Fix Mermaid diagram rendering in GitHub rich display  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `f4beb2a6` fix: PIN routes use card_id/card_pin and card_id/old_pin/new_pin; sanitize payload for jsonb; doc and Postman  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `dbf11c61` fix: allow User-Identifier header in CORS for automation tests  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `154d61f7` Add server logging, issued-card storage fixes, and user-identifier upsert  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-14` `50d06236` fix: quote Mermaid node labels to fix GitHub render parse error  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `b81a92a8` fix: diagram  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `23861669` Fix Mermaid diagram for GitHub rendering  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `1d605aef` Fix Mermaid request flow diagram for GitHub  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Docs (4)

- `2026-03-29` `78a42913` Align USD proxy with 200cards; log upstream bodies; automation docs  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `1103f028` docs: automation tests – require request-status polling and client_request_id formats for async steps  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-12` `926d519d` Document architecture, PRD, and request flows in README  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `223e0976` README: token TTL/renewal/retry, camelCase admin API, config table, run note  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (5)

- `2026-03-19` `958a7606` chore: updates compose file  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-19` `3cf47fc4` chore: updates dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b1120bee` Bump Go version to 1.24 in go.mod  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `5b651925` Initial commit: Go proxy for 200cards API with health, USD card routes, API key auth, user-identifier tracking, create-card audit, Postgres/GORM, Docker  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `410b3cb5` Go 1.26: bump go.mod and Dockerfile; use 1.22+ method/path routing and PathValue  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (11)

- `2026-04-15` `30d51189` Include gen-apikey binary in runtime image  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `11399ad2` proxy over tcp nd ipv4  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `b80cd911` check  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `9a23f202` salam 2  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `4c0fdb09` commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `450628dd` salam22  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-30` `2ab813ae` salam  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `557c7af7` log login response body only on non-2xx status  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `b2c5d1e2` Token TTL from env, renewal before expiry, retry login with backoff  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-25` `40b00d25` Parse JWT exp claim for token expiry; fallback to LOGIN_TOKEN_TTL when missing  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `b5f755e0` Go 1.21 routes: path-only patterns + RequireMethod; admin responses camelCase, no KeyHash; bootstrap login non-fatal; CORS on all routes  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## sunrate-proxy-ui

- Branches with matches: 4
- Commits listed in this repo section: 57

### Branch `main` (16)

#### Features (2)

- `2026-05-26` `f692b868` Add imageManager.sh for stage/prod admin UI builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-12` `045eade5` feat(automation): config picker pause, resume paths, and create-card body  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (6)

- `2026-05-12` `fd46186c` fix: update  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-12` `56127d3a` fix(automation): cap create-card remark at 32 characters  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-12` `0ef9bc33` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `c723bf9c` fixes ngixn 404 on refresh page problem  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `f2ec1552` Add Automation Tests page and fix API payloads  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `1d7d63ff` Fix app layout: top navbar in flow, improve UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-03-19` `688e59e4` chore: adds dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (7)

- `2026-05-24` `3ee1f2b5` Update Vite base path for stg.niwan.net/sunrate/admin-panel deploy.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `65f8e043` Deploy under /sunrate: Vite base, router basename, image push script  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `f877670e` Automation: env User-Identifier, cards/search, purchase quantity; shared proxy URL  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `5a51bc6f` Tenant admin UI: CRUD, soft-delete, one-time password reveal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `e7765235` Ignore .env in git  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `5fa39b02` Admin UI: login with API key, dashboard, floating navbar, API keys, user identifiers, issued cards pages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `1c33ab7c` Migrate from CSS modules to Tailwind CSS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `newgit/main` (9)

#### Bug Fixes (3)

- `2026-04-15` `c723bf9c` fixes ngixn 404 on refresh page problem  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `f2ec1552` Add Automation Tests page and fix API payloads  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `1d7d63ff` Fix app layout: top navbar in flow, improve UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-03-19` `688e59e4` chore: adds dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (5)

- `2026-03-29` `f877670e` Automation: env User-Identifier, cards/search, purchase quantity; shared proxy URL  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `5a51bc6f` Tenant admin UI: CRUD, soft-delete, one-time password reveal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `e7765235` Ignore .env in git  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `5fa39b02` Admin UI: login with API key, dashboard, floating navbar, API keys, user identifiers, issued cards pages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `1c33ab7c` Migrate from CSS modules to Tailwind CSS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/HEAD` (16)

#### Features (2)

- `2026-05-26` `f692b868` Add imageManager.sh for stage/prod admin UI builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-12` `045eade5` feat(automation): config picker pause, resume paths, and create-card body  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (6)

- `2026-05-12` `fd46186c` fix: update  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-12` `56127d3a` fix(automation): cap create-card remark at 32 characters  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-12` `0ef9bc33` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `c723bf9c` fixes ngixn 404 on refresh page problem  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `f2ec1552` Add Automation Tests page and fix API payloads  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `1d7d63ff` Fix app layout: top navbar in flow, improve UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-03-19` `688e59e4` chore: adds dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (7)

- `2026-05-24` `3ee1f2b5` Update Vite base path for stg.niwan.net/sunrate/admin-panel deploy.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `65f8e043` Deploy under /sunrate: Vite base, router basename, image push script  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `f877670e` Automation: env User-Identifier, cards/search, purchase quantity; shared proxy URL  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `5a51bc6f` Tenant admin UI: CRUD, soft-delete, one-time password reveal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `e7765235` Ignore .env in git  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `5fa39b02` Admin UI: login with API key, dashboard, floating navbar, API keys, user identifiers, issued cards pages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `1c33ab7c` Migrate from CSS modules to Tailwind CSS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/main` (16)

#### Features (2)

- `2026-05-26` `f692b868` Add imageManager.sh for stage/prod admin UI builds.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-12` `045eade5` feat(automation): config picker pause, resume paths, and create-card body  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (6)

- `2026-05-12` `fd46186c` fix: update  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-12` `56127d3a` fix(automation): cap create-card remark at 32 characters  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-12` `0ef9bc33` fix: commit  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-04-15` `c723bf9c` fixes ngixn 404 on refresh page problem  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-15` `f2ec1552` Add Automation Tests page and fix API payloads  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `1d7d63ff` Fix app layout: top navbar in flow, improve UI  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Chores (1)

- `2026-03-19` `688e59e4` chore: adds dockerfile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (7)

- `2026-05-24` `3ee1f2b5` Update Vite base path for stg.niwan.net/sunrate/admin-panel deploy.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-05-04` `65f8e043` Deploy under /sunrate: Vite base, router basename, image push script  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `f877670e` Automation: env User-Identifier, cards/search, purchase quantity; shared proxy URL  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-03-29` `5a51bc6f` Tenant admin UI: CRUD, soft-delete, one-time password reveal  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `e7765235` Ignore .env in git  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `5fa39b02` Admin UI: login with API key, dashboard, floating navbar, API keys, user identifiers, issued cards pages  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)
- `2026-02-24` `1c33ab7c` Migrate from CSS modules to Tailwind CSS  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

## sso

- Branches with matches: 5
- Commits listed in this repo section: 9

### Branch `fix/sand-real-zeepay` (3)

#### Features (1)

- `2026-05-18` `fd6cfa8c` add structured zeepay call logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (1)

- `2026-05-18` `7297b3c4` fix sand zeepay client profile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (1)

- `2026-05-19` `09c98585` Store reset-password Zeepay tokens in Redis and harden set-password flow.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `hotfix/zeepay-error-mapping-503004` (1)

#### Bug Fixes (1)

- `2026-05-12` `a88d606e` fix(sso): surface ZeePay 503004 and preserve codes for Feign errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/development` (1)

#### Bug Fixes (1)

- `2026-05-12` `a88d606e` fix(sso): surface ZeePay 503004 and preserve codes for Feign errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/fix/sand-real-zeepay` (3)

#### Features (1)

- `2026-05-18` `fd6cfa8c` add structured zeepay call logging  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Bug Fixes (1)

- `2026-05-18` `7297b3c4` fix sand zeepay client profile  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

#### Other (1)

- `2026-05-19` `09c98585` Store reset-password Zeepay tokens in Redis and harden set-password flow.  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

### Branch `origin/hotfix/zeepay-error-mapping-503004` (1)

#### Bug Fixes (1)

- `2026-05-12` `a88d606e` fix(sso): surface ZeePay 503004 and preserve codes for Feign errors  (author: Hamid <hamid@hamsaa.ir>; committer: Hamid <hamid@hamsaa.ir>)

