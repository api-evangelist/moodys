---
generated: '2026-06-20'
method: generated
name: Discover Data Buffet series and metadata
description: Search the Data Buffet catalog for series mnemonics and enumerate the frequencies, vintages, and file types available for retrieval.
api: openapi/moodys-search-api-openapi.yml
operations: [getAccessToken, searchSeries, listFrequencies, listVintages, listFileTypes, checkHealth]
source: >-
  Grounded in openapi/moodys-search-api-openapi.yml,
  openapi/moodys-reference-api-openapi.yml, and
  openapi/moodys-health-api-openapi.yml.
---

# Discover Data Buffet series and metadata

Use this before any retrieval flow: find the right series mnemonics and learn what retrieval options they support.

## Auth
- OAuth2 client-credentials via `getAccessToken`; send `Authorization: Bearer <token>`. See `authentication/moodys-authentication.yml`.

## Steps
1. **Check availability** — `checkHealth` (`openapi/moodys-health-api-openapi.yml`) verifies the API is up (also see the kompany status page for the KYC surface: https://kycapi-status.kompany.com/).
2. **Get a token** — `getAccessToken`.
3. **Search the catalog** — `searchSeries` (`GET /search`) with your query terms; results carry the series mnemonics used by `getSeries`/`getMultiSeries` and basket contents.
4. **Enumerate options** — `listFrequencies` (frequency conversions), `listVintages` (point-in-time dataset versions), and `listFileTypes` (order output formats), all in `openapi/moodys-reference-api-openapi.yml`.

## Errors
- Custom `Error {code, message}` envelope — see `errors/moodys-problem-types.yml`.

## Notes
- Mnemonics, not URLs, are the currency of the Data Buffet API: every downstream retrieval keys off the mnemonics discovered here (`data-model/moodys-data-model.yml`).
