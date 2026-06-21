# Kintsugi (kintsugi)

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
