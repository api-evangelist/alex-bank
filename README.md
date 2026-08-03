# Alex Bank (alex-bank)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
