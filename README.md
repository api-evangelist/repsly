# Repsly (repsly)

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
