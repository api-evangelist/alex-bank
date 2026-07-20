---
name: Look up Alex Bank banking products
description: >-
  Retrieve Alex Bank's publicly available deposit and lending products (rates, fees,
  features, eligibility) via the unauthenticated CDR Product Reference Data API, then
  drill into a single product's full detail. No credentials required.
api: openapi/alex-bank-cds-banking-products-openapi.yml
method: generated
generated: '2026-07-20'
operations:
- listBankingProducts
- getBankingProductDetail
---

# Look up Alex Bank banking products

Alex Bank exposes its product catalogue through the Consumer Data Right (CDR) Product
Reference Data API. This surface is **public and unauthenticated** — send no API key,
OAuth token or client certificate.

Base URL: `https://public.cdr.alex.com.au/cds-au/v1`

## Rules

- Always send the CDR version header `x-v` (use `x-v: 5` for Get Products, the current
  version; `x-v: 4` for Get Product Detail). Optionally send `x-min-v` for the lowest
  acceptable version. A version mismatch returns `406 Unsupported Version`.
- Responses are paginated: use `page` and `page-size` query params (max page-size 1000).
  Read `meta.totalRecords` / `meta.totalPages` and follow `links.next` to page through.
- Errors use the CDR envelope (`errors[]` of `code`/`title`/`detail`), not RFC 9457.
  Correlate with the `x-fapi-interaction-id` response header.

## Steps

1. **List products** — call `listBankingProducts` (`GET /banking/products`) with header
   `x-v: 5`. Optionally filter with `product-category`, `effective`, `updated-since`, or
   `brand`. Read `data.products[]` and page via `links.next` until `links.next` is absent.
2. **Pick a product** — take the `productId` of the product you care about from the list.
3. **Get product detail** — call `getBankingProductDetail`
   (`GET /banking/products/{productId}`) with header `x-v: 4` to retrieve full rates,
   fees, features, constraints, eligibility and additional-information links.

## Notes

Anything beyond product reference data (accounts, balances, transactions, payees) is the
CDR consumer-data-sharing surface and requires ACCC accreditation, FAPI OAuth2/OIDC and
mTLS — it is not reachable with this skill.
