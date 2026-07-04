# Repsly (repsly)

Repsly is a retail execution and field sales platform for CPG brands and field teams - covering in-store activity, merchandising, retail audits, order taking, and territory management. The Repsly Web API (v3) is a REST interface at `https://api.repsly.com/v3` designed for ERP/CRM integration: it imports (POST) clients and products into Repsly and exports (GET) clients, visits, retail audits, forms, photos, purchase orders, pricelists, representatives, and schedules back out. Requests use HTTP Basic authentication over SSL (with API credentials from the Repsly settings page, distinct from your login), exchange JSON or XML, and paginate export results in batches of up to 50 records using timestamp or last-ID cursors until the response `MetaCollectionResult.TotalCount` reaches zero.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/apis.yml)

## Tags

- Retail Execution
- Field Sales
- Merchandising
- CPG
- Retail Audits
- Sales Force Automation

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

### Repsly Clients API

Export clients and client notes from Repsly and import (insert or update) client master data from an ERP/CRM. Client export uses a timestamp cursor; client notes use a last-note-ID cursor.

- **Human URL:** [https://repsly-dev.readme.io/reference/getting-started-1](https://repsly-dev.readme.io/reference/getting-started-1)
- **Base URL:** `https://api.repsly.com/v3`

#### Tags

- Clients
- Client Notes
- CRM

#### Properties

- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [API Reference](https://knowledge.repsly.com/hc/en-us/sections/4408918344723-API-documentation)
- [OpenAPI](openapi/repsly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/repsly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/repsly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Repsly Representatives API

Export the field representatives (and back-office users) on the account along with their territories and permissions, plus daily working time records that log each representative's tracked hours.

- **Human URL:** [https://repsly-dev.readme.io/reference/getting-started-1](https://repsly-dev.readme.io/reference/getting-started-1)
- **Base URL:** `https://api.repsly.com/v3`

#### Tags

- Representatives
- Users
- Working Time

#### Properties

- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [OpenAPI](openapi/repsly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/repsly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/repsly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Repsly Visits API

Export in-store visits (check-in/check-out, GPS, notes), planned visit schedules over a date range, and visit schedule realizations, and import visit schedules to plan representatives' routes.

- **Human URL:** [https://repsly-dev.readme.io/reference/getting-started-1](https://repsly-dev.readme.io/reference/getting-started-1)
- **Base URL:** `https://api.repsly.com/v3`

#### Tags

- Visits
- Schedules
- Field Activity

#### Properties

- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [OpenAPI](openapi/repsly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/repsly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/repsly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Repsly Products API

Export products, product lists, and document types, and import (insert or update) product catalog and product packaging data from an ERP so mobile reps always work from current SKUs.

- **Human URL:** [https://repsly-dev.readme.io/reference/getting-started-1](https://repsly-dev.readme.io/reference/getting-started-1)
- **Base URL:** `https://api.repsly.com/v3`

#### Tags

- Products
- Product Lists
- Catalog

#### Properties

- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [OpenAPI](openapi/repsly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/repsly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/repsly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Repsly Forms API

Export completed custom forms and retail audit results (including matrix answers) captured by representatives in the field, using last-form-ID and last-retail-audit-ID cursors.

- **Human URL:** [https://repsly-dev.readme.io/reference/getting-started-1](https://repsly-dev.readme.io/reference/getting-started-1)
- **Base URL:** `https://api.repsly.com/v3`

#### Tags

- Forms
- Retail Audits
- Data Collection

#### Properties

- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [OpenAPI](openapi/repsly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/repsly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/repsly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Repsly Photos API

Export photos captured during visits - shelf and display shots, merchandising evidence, and form/audit attachments - with their metadata and URLs, paginated by a last-photo-ID cursor.

- **Human URL:** [https://repsly-dev.readme.io/reference/getting-started-1](https://repsly-dev.readme.io/reference/getting-started-1)
- **Base URL:** `https://api.repsly.com/v3`

#### Tags

- Photos
- Merchandising
- Media

#### Properties

- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [OpenAPI](openapi/repsly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/repsly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/repsly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Repsly Pricelists API

Export the list of pricelists and the items within a specific pricelist, and import (insert or update) pricelists and their items so order taking uses the correct per-client pricing.

- **Human URL:** [https://repsly-dev.readme.io/reference/getting-started-1](https://repsly-dev.readme.io/reference/getting-started-1)
- **Base URL:** `https://api.repsly.com/v3`

#### Tags

- Pricelists
- Pricing
- Catalog

#### Properties

- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [OpenAPI](openapi/repsly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/repsly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/repsly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Repsly Purchase Orders API

Export purchase orders (and other sales documents) taken by reps in the field, paginated by a last-document-ID cursor, and post status updates back to a sales document after it is processed in the back office.

- **Human URL:** [https://repsly-dev.readme.io/reference/getting-started-1](https://repsly-dev.readme.io/reference/getting-started-1)
- **Base URL:** `https://api.repsly.com/v3`

#### Tags

- Purchase Orders
- Orders
- Sales Documents

#### Properties

- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [OpenAPI](openapi/repsly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/repsly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/repsly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Repsly Import and Export API

The bulk integration surface. Import (POST) clients, products, packages, pricelists, and schedules where Repsly decides per record whether to insert or update, then poll the import job status endpoint by importJobID to confirm completion.

- **Human URL:** [https://repsly-dev.readme.io/reference/getting-started-1](https://repsly-dev.readme.io/reference/getting-started-1)
- **Base URL:** `https://api.repsly.com/v3`

#### Tags

- Import
- Export
- Integration

#### Properties

- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [OpenAPI](openapi/repsly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/repsly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/repsly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/repsly)
- [Website](https://www.repsly.com)
- [Documentation](https://repsly-dev.readme.io/reference/getting-started-1)
- [Plans](plans/repsly-plans-pricing.yml)
- [Rate Limits](rate-limits/repsly-rate-limits.yml)
- [Fin Ops](finops/repsly-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
