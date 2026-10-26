# Kintsugi (kintsugi)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Kintsugi is an AI-driven sales tax compliance and automation platform that calculates US sales tax, VAT, and GST in real time, monitors economic and physical nexus, manages exemptions and registrations, and auto-prepares and files returns. Its REST API exposes tax estimation, transactions, products, address validation, nexus, exemptions, registrations, and filings, authenticated with an API key plus organization ID header.

> Disambiguation: this is Kintsugi the sales tax automation company (trykintsugi.com), not the unrelated Kintsugi mental-health / voice-biomarker company.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/kintsugi/refs/heads/main/apis.yml)

## Tags

- Sales Tax
- Tax Compliance
- Tax Automation
- VAT
- GST
- Nexus
- AI

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Kintsugi Tax Calculations API

Calculates sales tax, VAT, and GST for a transaction before payment via POST /tax/estimate, returning jurisdiction-level tax breakdown, taxable amount, effective rate, and active-registration status without persisting a record.

- **Human URL:** [https://docs.trykintsugi.com/docs/api-guides/sales-tax-calculations](https://docs.trykintsugi.com/docs/api-guides/sales-tax-calculations)
- **Base URL:** `https://api.trykintsugi.com/v1`

#### Tags

- Tax Calculation
- Tax Estimate
- Sales Tax

#### Properties

- [Documentation](https://docs.trykintsugi.com/docs/api-guides/sales-tax-calculations)
- [API Reference](https://docs.trykintsugi.com/reference/api/tax-estimation/estimate-tax)
- [OpenAPI](openapi/kintsugi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kintsugi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kintsugi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kintsugi Transactions API

Creates, retrieves, and updates committed sales transactions and credit notes, with lookup by Kintsugi ID, external ID, customer, or filing, to drive accurate liability and return preparation.

- **Human URL:** [https://docs.trykintsugi.com/docs/api-guides/syncing-transaction-records](https://docs.trykintsugi.com/docs/api-guides/syncing-transaction-records)
- **Base URL:** `https://api.trykintsugi.com/v1`

#### Tags

- Transactions
- Credit Notes
- Filings

#### Properties

- [Documentation](https://docs.trykintsugi.com/docs/api-guides/syncing-transaction-records)
- [API Reference](https://docs.trykintsugi.com/reference/api/transactions/create-transaction)
- [OpenAPI](openapi/kintsugi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kintsugi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kintsugi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kintsugi Products and Tax Codes API

Manages product records and their taxability classification, including listing product categories used to map catalog items to the correct tax treatment across jurisdictions.

- **Human URL:** [https://docs.trykintsugi.com/docs/api-guides/product-customer-records](https://docs.trykintsugi.com/docs/api-guides/product-customer-records)
- **Base URL:** `https://api.trykintsugi.com/v1`

#### Tags

- Products
- Tax Codes
- Product Categories

#### Properties

- [Documentation](https://docs.trykintsugi.com/docs/api-guides/product-customer-records)
- [API Reference](https://docs.trykintsugi.com/reference/api/products/create-product)
- [OpenAPI](openapi/kintsugi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kintsugi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kintsugi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kintsugi Addresses and Nexus API

Validates and suggests addresses for accurate jurisdiction assignment, and manages physical nexus and state registrations so liability tracking reflects where the business is obligated to collect tax.

- **Human URL:** [https://docs.trykintsugi.com/reference/api/address-validation/search](https://docs.trykintsugi.com/reference/api/address-validation/search)
- **Base URL:** `https://api.trykintsugi.com/v1`

#### Tags

- Address Validation
- Nexus
- Registrations

#### Properties

- [Documentation](https://docs.trykintsugi.com/reference/api/address-validation/search)
- [API Reference](https://docs.trykintsugi.com/reference/api/nexus/get-nexus-for-org)
- [OpenAPI](openapi/kintsugi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kintsugi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kintsugi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kintsugi Exemptions API

Creates and lists customer tax exemptions and uploads or retrieves exemption certificate attachments, so exempt sales are excluded from calculated liability with documentation on file.

- **Human URL:** [https://docs.trykintsugi.com/reference/api/exemptions/get-exemptions](https://docs.trykintsugi.com/reference/api/exemptions/get-exemptions)
- **Base URL:** `https://api.trykintsugi.com/v1`

#### Tags

- Exemptions
- Certificates
- Compliance

#### Properties

- [Documentation](https://docs.trykintsugi.com/reference/api/exemptions/get-exemptions)
- [API Reference](https://docs.trykintsugi.com/reference/api/exemptions/create-exemption)
- [OpenAPI](openapi/kintsugi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kintsugi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kintsugi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kintsugi Filings API

Retrieves prepared and submitted sales tax returns, including filings by ID and by registration, giving programmatic visibility into the automated filing lifecycle Kintsugi runs on the customer's behalf.

- **Human URL:** [https://docs.trykintsugi.com/reference/api/filings/get-filings](https://docs.trykintsugi.com/reference/api/filings/get-filings)
- **Base URL:** `https://api.trykintsugi.com/v1`

#### Tags

- Filings
- Returns
- Registrations

#### Properties

- [Documentation](https://docs.trykintsugi.com/reference/api/filings/get-filings)
- [API Reference](https://docs.trykintsugi.com/reference/api/filings/get-filing-by-id)
- [OpenAPI](openapi/kintsugi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kintsugi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kintsugi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Kintsugi Webhooks

Event notifications that let integrations react to changes such as nexus thresholds being approached, registrations completing, and filings being prepared or submitted, keeping external systems in sync with compliance state.

- **Human URL:** [https://docs.trykintsugi.com/docs/guides/integrating-kintsugis-api](https://docs.trykintsugi.com/docs/guides/integrating-kintsugis-api)
- **Base URL:** `https://api.trykintsugi.com/v1`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.trykintsugi.com/docs/guides/integrating-kintsugis-api)
- [OpenAPI](openapi/kintsugi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [GitHub Organization](https://github.com/kintsugi-tax)
- [LinkedIn](https://www.linkedin.com/company/trykintsugi)
- [Website](https://www.trykintsugi.com)
- [Documentation](https://docs.trykintsugi.com)
- [Plans](plans/kintsugi-plans-pricing.yml)
- [Rate Limits](rate-limits/kintsugi-rate-limits.yml)
- [Fin Ops](finops/kintsugi-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
