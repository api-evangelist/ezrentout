# EZRentOut (ezrentout)

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

EZRentOut is cloud-based equipment rental management software from EZO (the company behind EZOfficeInventory) for rental businesses to manage orders, fixed and inventory assets, bundles, customers, members, locations, purchase orders, and maintenance. Its REST API is made available to paying customers for custom integrations - each request is authenticated with a per-company access token sent in a `token` header over HTTPS, endpoints are namespaced with a `.api` suffix, and calls are scoped to the customer's own `{subdomain}.ezrentout.com` tenant.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/apis.yml)

## Tags

- Equipment Rental
- Rental Management
- Asset Tracking
- Inventory
- Order Management
- EZO

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## Authentication

The API is disabled by default and must be enabled by the account owner in **Settings**, where a per-company access token is generated. Send the token in a `token` HTTP header on every request over HTTPS. All requests are scoped to your own tenant at `https://{subdomain}.ezrentout.com`. List endpoints are paginated via a `page` query parameter (default 1). Dates use `mm/dd/yyyy` and times use `hh:mm`.

## APIs

### EZRentOut Orders API

Create and manage rental orders (called baskets) end to end - draft an order, add assets, inventory, and stock, reserve and cancel reservations, apply coupons, taxes, and damage charges, check out (rent out), check in (return), and read order details and history.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Orders
- Baskets
- Reservations

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [API Reference](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Fixed Assets API

Manage serialized fixed (rentable) assets - create, list, filter, retrieve, update, retire, and delete equipment, update GPS coordinates for location tracking, read asset history and booked dates, and search the catalog.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Assets
- Equipment
- GPS

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [API Reference](https://ezo.io/ezrentout/blog/location-tracking-assets-api/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Inventory API

Manage inventory (volatile assets) and asset stock - create, list, filter, retrieve, update, and delete items, add and transfer stock across locations, read stock history and booked dates, and inspect location-based quantity thresholds.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Inventory
- Stock
- Volatile Assets

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Bundles API

Create, list, and retrieve bundles - reusable packages (kits) of assets and inventory that can be rented out together as a single line on an order.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Bundles
- Kits
- Packages

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Customers API

Manage the people and organizations that rent - customers, businesses, and business contacts - with full CRUD, activation and deactivation, and shipping and billing address management per customer and per business.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Customers
- Businesses
- Contacts

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Members API

Manage members (staff users) of the rental account - create, list, retrieve, and update members, mark them active or inactive, and read the items a member currently has checked out.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Members
- Users
- Staff

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Locations API

Manage the locations (warehouses / branches) that assets and inventory live in - create, list, retrieve, and update locations, activate and deactivate them, and read item quantity by location.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Locations
- Warehouses
- Multi-location

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Availability API

Check availability for rental scheduling - read booked (reserved) dates for a specific asset, inventory item, or stock asset, and read available quantity by location, so integrations can avoid double-booking before reserving an order.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Availability
- Booked Dates
- Scheduling

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Payments and Invoicing API

Handle order billing - list payment options, charge a pre-payment or a full payment against an order, void a recorded payment, apply taxes (custom and group tax IDs) and pricing coupons, and add damage charges. Invoicing in EZRentOut is expressed through these order-scoped payment and tax endpoints rather than a standalone invoice resource.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Payments
- Invoicing
- Taxes

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Purchase Orders API

Manage procurement - create and update purchase orders, add catalog and non-catalog line items, confirm, receive items against, void, and delete a PO, read PO details, and manage the vendors POs are raised with.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Purchase Orders
- Procurement
- Vendors

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EZRentOut Maintenance and Work Orders API

Keep equipment serviceable - put assets into maintenance, create, schedule, update, and complete service records, and manage work orders (tasks) with start and end, work logs, linked inventory, and checklists.

- **Human URL:** [https://ezo.io/ezrentout/developers/](https://ezo.io/ezrentout/developers/)
- **Base URL:** `https://{subdomain}.ezrentout.com`

#### Tags

- Maintenance
- Services
- Work Orders

#### Properties

- [Documentation](https://ezo.io/ezrentout/developers/)
- [OpenAPI](openapi/ezrentout-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezrentout.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezrentout.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/showcase/ezrentout/)
- [Website](https://ezo.io/ezrentout/)
- [Documentation](https://ezo.io/ezrentout/developers/)
- [Plans](plans/ezrentout-plans-pricing.yml)
- [Rate Limits](rate-limits/ezrentout-rate-limits.yml)
- [Fin Ops](finops/ezrentout-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
