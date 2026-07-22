---
generated: '2026-06-20'
method: generated
name: Retrieve Moody's economic time series
description: Authenticate against the Data Buffet API and pull one or many economic/demographic time series by mnemonic, with frequency conversion and transformations.
api: openapi/moodys-series-api-openapi.yml
operations: [getAccessToken, getSeries, getMultiSeries]
source: >-
  Grounded in openapi/moodys-reference-api-openapi.yml and
  openapi/moodys-series-api-openapi.yml; conventions in
  conventions/moodys-conventions.yml.
---

# Retrieve Moody's economic time series

Use this to pull economic, demographic, or financial time series from Moody's Analytics Data Buffet.

## Auth
- OAuth2 client-credentials: `getAccessToken` (`POST /oauth2/token` on `https://api.economy.com/data/v1`) with your `client_id` and `client_secret` (provisioned with your Moody's Analytics subscription). See `authentication/moodys-authentication.yml`.
- Send the returned access token as `Authorization: Bearer <token>` on every call. There are no OAuth scopes — entitlements are account-based (see `scopes/moodys-scopes.yml`).

## Steps
1. **Get a token** — `getAccessToken`. Cache it and refresh before expiry.
2. **Single series** — `getSeries` (`GET /series`) with `mnemonic` (the Data Buffet series identifier). Optional: `freq` (frequency conversion — enumerate options first with `listFrequencies` in `openapi/moodys-reference-api-openapi.yml`), `trans` (mathematical transformation), `startDate`/`endDate`, and `vintage` for point-in-time data (`listVintages` enumerates them).
3. **Many series in one call** — `getMultiSeries` (`POST /multi-series`) with a body listing the mnemonics and shared retrieval options.

## Errors
- `400` invalid parameters, `401` invalid or expired token, `404` unknown mnemonic — the envelope is a custom `Error {code, message}` object, see `errors/moodys-problem-types.yml`.
- On `429`, honor the `Retry-After` header; limits are contract-negotiated (`rate-limits/moodys-rate-limits.yml`).

## Notes
- No idempotency-key mechanism exists; the retrieval operations are GETs and safe to retry.
- Responses are complete payloads — there is no pagination to follow.
