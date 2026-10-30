# EZRentOut

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

EZRentOut is cloud-based equipment rental management software from EZO (the company behind EZOfficeInventory) for rental businesses to manage orders, fixed and inventory assets, bundles, customers, members, locations, purchase orders, and maintenance. Its REST API is made available to paying customers for custom integrations - each request is authenticated with a per-company access token sent in a token header over HTTPS, endpoints are namespaced with a .api suffix, and calls are scoped to the customer's own {subdomain}.ezrentout.com tenant. The API covers orders (baskets), assets, inventory and stock assets, bundles, customers and businesses, members, locations, availability, payments and invoicing, purchase orders, and service/work-order maintenance.

**Areas:** Equipment Rental · Rental Management · Asset Tracking · Inventory · Order Management · EZO

## EZRentOut on APIs.io

Everything profiled for EZRentOut is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/ezrentout/](https://apis.io/providers/ezrentout/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [EZRentOut Assets API](https://apis.io/apis/ezrentout/ezrentout-assets-api/) — Serialized fixed (rentable) assets and GPS location tracking.
- [EZRentOut Availability API](https://apis.io/apis/ezrentout/ezrentout-availability-api/) — Booked dates and per-location quantity for scheduling.
- [EZRentOut Bundles API](https://apis.io/apis/ezrentout/ezrentout-bundles-api/) — Reusable kits of assets and inventory rented together.
- [EZRentOut Customers API](https://apis.io/apis/ezrentout/ezrentout-customers-api/) — Customers, businesses, and business contacts, with addresses.
- [EZRentOut Inventory API](https://apis.io/apis/ezrentout/ezrentout-inventory-api/) — Volatile assets (inventory) and asset stock, with per-location stock.
- [EZRentOut Locations API](https://apis.io/apis/ezrentout/ezrentout-locations-api/) — Warehouses / branches that hold assets and inventory.
- [EZRentOut Maintenance API](https://apis.io/apis/ezrentout/ezrentout-maintenance-api/) — Service records and work orders (tasks) to keep equipment serviceable.
- [EZRentOut Members API](https://apis.io/apis/ezrentout/ezrentout-members-api/) — Staff members (users) of the rental account.
- [EZRentOut Orders API](https://apis.io/apis/ezrentout/ezrentout-orders-api/) — Rental orders, called baskets - draft, reserve, check out, and check in.
- [EZRentOut Payments API](https://apis.io/apis/ezrentout/ezrentout-payments-api/) — Order payments, taxes, coupons, and damage charges (invoicing).
- [EZRentOut Purchase Orders API](https://apis.io/apis/ezrentout/ezrentout-purchase-orders-api/) — Procurement - purchase orders and vendors.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Ezrentout Agentic Access](https://apis.io/agentic-access/ezrentout/ezrentout-agentic-access/)

#### Collections (12)

Postman and Open Collection request collections.

- [EZRentOut API](https://apis.io/collections/ezrentout/open-ezrentout/)
- [EZRentOut Assets API](https://apis.io/collections/ezrentout/open-ezrentout-assets-api/)
- [EZRentOut Assets Availability API](https://apis.io/collections/ezrentout/open-ezrentout-availability-api/)
- [EZRentOut Assets Bundles API](https://apis.io/collections/ezrentout/open-ezrentout-bundles-api/)
- [EZRentOut Assets Customers API](https://apis.io/collections/ezrentout/open-ezrentout-customers-api/)
- [EZRentOut Assets Inventory API](https://apis.io/collections/ezrentout/open-ezrentout-inventory-api/)
- [EZRentOut Assets Locations API](https://apis.io/collections/ezrentout/open-ezrentout-locations-api/)
- [EZRentOut Assets Maintenance API](https://apis.io/collections/ezrentout/open-ezrentout-maintenance-api/)
- [EZRentOut Assets Members API](https://apis.io/collections/ezrentout/open-ezrentout-members-api/)
- [EZRentOut Assets Orders API](https://apis.io/collections/ezrentout/open-ezrentout-orders-api/)
- [EZRentOut Assets Payments API](https://apis.io/collections/ezrentout/open-ezrentout-payments-api/)
- [EZRentOut Assets Purchase Orders API](https://apis.io/collections/ezrentout/open-ezrentout-purchase-orders-api/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Ezrentout Authentication](https://apis.io/security/ezrentout/ezrentout-authentication/)
- [Ezrentout Domain Security](https://apis.io/security/ezrentout/ezrentout-domain-security/)
- [Ezrentout Trust Center](https://apis.io/security/ezrentout/ezrentout-trust-center/)

#### Plans and pricing (2)

Published plans, tiers and prices.

- [Ezrentout Plans Pricing](https://apis.io/plans/ezrentout/ezrentout-plans-pricing/)
- [Ezrentout Price Estimates](https://apis.io/plans/ezrentout/ezrentout-price-estimates/)

#### Rate limits (1)

Published request limits.

- [Ezrentout Rate Limits](https://apis.io/rate-limits/ezrentout/ezrentout-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Ezrentout Finops](https://apis.io/finops/ezrentout/ezrentout-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://ezo.io/ezrentout/)
- [Documentation](https://ezo.io/ezrentout/developers/)
- [Pricing](https://ezo.io/ezrentout/pricing/)
- [Blog](https://ezo.io/ezrentout/blog/feed/)

## API Evangelist rating

**Kin Score 36.3** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 44.1 |
| Contract governance | 0.0 |
| Operational transparency | 21.1 |
| Developer ergonomics | 32.1 |
| Access clarity | 50.0 |

**Agent readiness 24.0** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | verified |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/ezrentout/](https://apis.io/providers/ezrentout/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for EZRentOut: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/ezrentout/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
