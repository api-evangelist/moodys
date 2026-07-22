---
generated: '2026-06-20'
method: generated
name: Run a Data Buffet basket and download the output
description: Create or reuse a basket of series, execute it as an order, poll for completion, and download the generated file.
api: openapi/moodys-baskets-api-openapi.yml
operations: [getAccessToken, listBaskets, createBasket, createOrder, getOrder, downloadOrder]
source: >-
  Grounded in openapi/moodys-baskets-api-openapi.yml,
  openapi/moodys-orders-api-openapi.yml, and
  openapi/moodys-reference-api-openapi.yml.
---

# Run a Data Buffet basket and download the output

Use this for batch retrieval: a **basket** is a saved collection of series, an **order** is an asynchronous execution of that basket producing a downloadable file.

## Auth
- OAuth2 client-credentials via `getAccessToken`; send `Authorization: Bearer <token>`. See `authentication/moodys-authentication.yml`.

## Steps
1. **Get a token** — `getAccessToken` (`openapi/moodys-reference-api-openapi.yml`).
2. **Find or create the basket** — `listBaskets` (`GET /baskets`) to reuse an existing one, or `createBasket` (`POST /baskets`) with the series mnemonics. Manage it later with `getBasket`, `updateBasket`, `deleteBasket`.
3. **Pick an output format** — `listFileTypes` (`openapi/moodys-reference-api-openapi.yml`) enumerates supported file types.
4. **Execute** — `createOrder` (`openapi/moodys-orders-api-openapi.yml`) referencing the basket id. Capture the order id.
5. **Poll** — `getOrder` until the order reports completion (`listOrders` shows all recent orders).
6. **Download** — `downloadOrder` streams the generated output file.

## Errors
- Custom `Error {code, message}` envelope (`errors/moodys-problem-types.yml`); `401` means the token expired — re-run `getAccessToken`.
- Do not tight-loop `getOrder`; back off between polls and honor `Retry-After` on `429`.

## Notes
- `createOrder` is **not** idempotent-keyed — check `listOrders` before retrying a submission that may have gone through (`conventions/moodys-conventions.yml`).
