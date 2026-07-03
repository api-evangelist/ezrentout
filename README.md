# EZRentOut (ezrentout)

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
