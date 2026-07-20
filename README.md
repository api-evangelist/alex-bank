# Alex Bank (alex-bank)

Alex Bank (Alex Bank Pty Ltd, ABN 13 627 244 848) is an Australian digital bank headquartered in Brisbane, founded in 2018 by former Suncorp bankers Simon Beitz and Craig Fenwick. It is a shareholder-owned, venture-backed authorised deposit-taking institution (ADI) - not a customer-owned mutual - that received its Restricted ADI licence from APRA in July 2021 and a full banking licence in December 2021. Alex offers consumer lending (personal, green, car and EV loans) and deposit products (term deposits and a savings account). As an active ADI it is a Consumer Data Right (CDR) data holder and exposes a public Product Reference Data API under the DSB Consumer Data Standards.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/apis.yml)

## Tags

- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Digital Bank
- Product Reference Data

## Timestamps

- **Created:** 2026-07-20
- **Modified:** 2026-07-20

## APIs

### Alex Bank CDR Product Reference Data API

Public, unauthenticated Product Reference Data (PRD) API conforming to the DSB Consumer Data Standards (CDR Banking API). Confirmed live at `https://public.cdr.alex.com.au/cds-au/v1/banking/products` (HTTP 200, `x-v: 3`) returning a `data.products` array of Alex Bank's deposit and lending products (term deposits, savings, personal/green/car/EV loans) with rates, fees, features and eligibility. Exposes `GET /banking/products` and `GET /banking/products/{productId}`; no API key or OAuth required.

- **Human URL:** [https://www.alex.bank/legal/open-banking/](https://www.alex.bank/legal/open-banking/)
- **Base URL:** `https://public.cdr.alex.com.au/cds-au/v1`

#### Tags

- CDR
- Open Banking
- Product Reference Data
- Banking
- Public API

#### Properties

- [Documentation](https://www.alex.bank/legal/open-banking/)
- [API Reference](https://consumerdatastandardsaustralia.github.io/standards/#get-products)
- [OpenAPI](openapi/alex-bank-cds-banking-products-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [Website](https://www.alex.bank/)
- [Documentation](https://www.alex.bank/legal/open-banking/)
- [Blog](https://www.alex.bank/blog/)
- [Privacy Policy](https://www.alex.bank/legal/privacy-policy/)
- [Terms of Service](https://www.alex.bank/legal/)
- [Consumer Data Right Policy](https://www.alex.bank/legal/consumer-data-right-cdr-policy/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
