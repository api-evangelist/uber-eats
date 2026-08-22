# Uber Eats (uber-eats)

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

Uber Eats exposes a family of developer APIs through the Uber Developer
Portal that let restaurants, marketplace platforms, POS providers, and
logistics partners integrate directly with Uber Eats and Uber Direct.
The Uber Eats Marketplace APIs cover store onboarding, store status and
hours, menu management, order ingestion and fulfillment, delivery
fulfillment (Uber-courier and BYOC), promotions, and reporting. Uber
Direct (Deliveries) exposes Uber's courier network for on-demand
same-day delivery — quotes, deliveries, courier tracking, proof of
delivery, refunds, pick-and-pack, and webhook notifications. All APIs
are RESTful, JSON, and gated by OAuth 2.0 client credentials issued
from the Uber Developer Portal.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** Partner

## Tags

- Uber Eats
- Uber Direct
- Food Delivery
- Last-Mile Logistics
- Restaurants
- Menus
- Orders
- Fulfillment
- Courier
- OAuth2

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-06-03

## APIs

### Uber Eats Integration Activation API

The Integration Activation API suite onboards merchant stores onto
a partner's Uber Eats integration, connecting Uber store identifiers
to a partner platform and enabling subsequent menu, order, and
store API access.

- **Human URL:** [https://developer.uber.com/docs/eats/references/api/integration_activation_suite](https://developer.uber.com/docs/eats/references/api/integration_activation_suite)
- **Base URL:** `https://api.uber.com`

#### Tags

- Onboarding
- Activation
- Merchant

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/references/api/integration_activation_suite)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Eats Store API

The Store API suite manages store status (online/offline), business
hours, holiday schedules, and store configuration on Uber Eats. It
lets POS and marketplace integrations programmatically pause and
resume locations and update operating hours.

- **Human URL:** [https://developer.uber.com/docs/eats/references/api/store_suite](https://developer.uber.com/docs/eats/references/api/store_suite)
- **Base URL:** `https://api.uber.com`

#### Tags

- Stores
- Hours
- Status
- Location

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/references/api/store_suite)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/openapi/uber-eats-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Eats Menu API

The Menu API suite lets integrations retrieve and upsert full menus
for a store and update individual menu items, modifier groups,
prices, suspensions, and availability windows.

- **Human URL:** [https://developer.uber.com/docs/eats/references/api/v2/](https://developer.uber.com/docs/eats/references/api/v2/)
- **Base URL:** `https://api.uber.com`

#### Tags

- Menus
- Items
- Modifiers
- Pricing

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/references/api/v2/)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Eats Order API

The Order API suite handles inbound Uber Eats orders, including
order accept/deny, status updates, item-level adjustments, and
cancellation flows. Orders are typically delivered to integrations
via webhooks and acknowledged/fulfilled through this API.

- **Human URL:** [https://developer.uber.com/docs/eats/references/api/order_suite](https://developer.uber.com/docs/eats/references/api/order_suite)
- **Base URL:** `https://api.uber.com`

#### Tags

- Orders
- Fulfillment
- Webhooks
- POS

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/references/api/order_suite)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Eats Delivery Partner API

The Delivery Partner API suite handles delivery fulfillment by
Uber couriers for Uber Eats orders, including courier assignment,
tracking, and status updates surfaced back to the merchant
integration.

- **Human URL:** [https://developer.uber.com/docs/eats/references/api/delivery_partner_suite](https://developer.uber.com/docs/eats/references/api/delivery_partner_suite)
- **Base URL:** `https://api.uber.com`

#### Tags

- Delivery
- Couriers
- Tracking

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/references/api/delivery_partner_suite)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Eats Delivery BYOC API

The Delivery BYOC ("Bring Your Own Courier") API suite supports
merchants and marketplace partners that use their own delivery
fleet, exchanging assignment, status, and proof-of-delivery
information with Uber Eats.

- **Human URL:** [https://developer.uber.com/docs/eats/references/api/delivery_byoc_suite](https://developer.uber.com/docs/eats/references/api/delivery_byoc_suite)
- **Base URL:** `https://api.uber.com`

#### Tags

- BYOC
- Own Fleet
- Delivery

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/references/api/delivery_byoc_suite)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Eats Promotions API

The Promotions API suite creates and manages marketing campaigns
and discounts on Uber Eats stores, including campaign lifecycle,
targeting, and reporting.

- **Human URL:** [https://developer.uber.com/docs/eats/references/api/promotions_suite](https://developer.uber.com/docs/eats/references/api/promotions_suite)
- **Base URL:** `https://api.uber.com`

#### Tags

- Promotions
- Campaigns
- Marketing

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/references/api/promotions_suite)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Eats Reporting API

The Reporting API suite returns transactional, financial, and
performance reports for Uber Eats stores, used by merchants and
marketplace partners for reconciliation and analytics.

- **Human URL:** [https://developer.uber.com/docs/eats/references/api/reporting_suite](https://developer.uber.com/docs/eats/references/api/reporting_suite)
- **Base URL:** `https://api.uber.com`

#### Tags

- Reporting
- Analytics
- Financials

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/references/api/reporting_suite)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Direct (Deliveries) API

Uber Direct exposes Uber's courier network as a delivery-as-a-service
API. Merchants request a delivery (or quote), Uber dispatches a
courier, and the merchant receives webhook notifications throughout
the lifecycle. The API supports proof of delivery, geocoding,
delivery windows, and pincode validation.

- **Human URL:** [https://developer.uber.com/docs/deliveries/overview](https://developer.uber.com/docs/deliveries/overview)
- **Base URL:** `https://api.uber.com`

#### Tags

- Uber Direct
- Last-Mile
- Couriers
- Deliveries

#### Properties

- [Documentation](https://developer.uber.com/docs/deliveries/overview)
- [API Reference](https://developer.uber.com/docs/deliveries/references/api)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/openapi/uber-direct-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [SDK](https://www.npmjs.com/package/uber-direct)
- [Code Examples](https://github.com/uber/uber-direct-sdk-samples)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Direct Organizations API

The Organizations API lets Uber Direct partners manage parent
organizations and child accounts (e.g. multi-tenant merchants),
including provisioning of API credentials and store-level access.

- **Human URL:** [https://developer.uber.com/docs/deliveries/references/api/organizations](https://developer.uber.com/docs/deliveries/references/api/organizations)
- **Base URL:** `https://api.uber.com`

#### Tags

- Organizations
- Multi-Tenant
- Provisioning

#### Properties

- [Documentation](https://developer.uber.com/docs/deliveries/references/api/organizations)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Direct Courier Pick & Pack API

The Courier Pick & Pack API supports shop-and-pay style deliveries
where the courier shops on behalf of the customer, including item
lists, substitutions, and shopping progress events.

- **Human URL:** [https://developer.uber.com/docs/deliveries/references/api/pick-and-pack](https://developer.uber.com/docs/deliveries/references/api/pick-and-pack)
- **Base URL:** `https://api.uber.com`

#### Tags

- Pick and Pack
- Shopping
- Grocery

#### Properties

- [Documentation](https://developer.uber.com/docs/deliveries/references/api/pick-and-pack)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Direct Refund API

The Refund API supports refund requests on completed Uber Direct
deliveries, including the corresponding webhook events that notify
merchants of refund outcomes.

- **Human URL:** [https://developer.uber.com/docs/deliveries/references/api/refunds](https://developer.uber.com/docs/deliveries/references/api/refunds)
- **Base URL:** `https://api.uber.com`

#### Tags

- Refunds
- Disputes

#### Properties

- [Documentation](https://developer.uber.com/docs/deliveries/references/api/refunds)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Direct Business Location Management API

The Business Location Management API administers physical pickup
locations associated with Uber Direct accounts, used for routing
and dispatch.

- **Human URL:** [https://developer.uber.com/docs/deliveries/references/api/locations](https://developer.uber.com/docs/deliveries/references/api/locations)
- **Base URL:** `https://api.uber.com`

#### Tags

- Locations
- Pickup
- Stores

#### Properties

- [Documentation](https://developer.uber.com/docs/deliveries/references/api/locations)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Eats & Direct Webhooks

Both Uber Eats and Uber Direct send webhook events for order
lifecycle, courier updates, refunds, shopping progress, and
delivery status. Partners register webhook URLs in the Uber
Developer Portal and verify signatures on each delivery.

- **Human URL:** [https://developer.uber.com/docs/eats/guides/webhooks](https://developer.uber.com/docs/eats/guides/webhooks)
- **Base URL:** `https://api.uber.com`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/guides/webhooks)
- [Direct Webhooks](https://developer.uber.com/docs/deliveries/guides/webhooks)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber OAuth 2.0

Uber APIs are authenticated using OAuth 2.0. Server-to-server
integrations use the client_credentials grant; user-facing
integrations use the authorization_code grant with PKCE. Tokens
are obtained from the Uber OAuth token endpoint and scoped per
product (Eats, Direct, Riders, etc.).

- **Human URL:** [https://developer.uber.com/docs/eats/guides/authentication](https://developer.uber.com/docs/eats/guides/authentication)
- **Base URL:** `https://auth.uber.com/oauth/v2`

#### Tags

- OAuth2
- Authentication
- Client Credentials

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/guides/authentication)
- [Token Endpoint](https://auth.uber.com/oauth/v2/token)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.uber.com/us/en/business/products/eats/)
- [GitHub Organization](https://github.com/uber)
- [SDK](https://github.com/uber/uber-direct-sdk)
- [Developer Portal](https://developer.uber.com/)
- [Documentation](https://developer.uber.com/docs)
- [Uber Eats Docs](https://developer.uber.com/docs/eats/introduction)
- [Uber Direct Docs](https://developer.uber.com/docs/deliveries/overview)
- [Authentication](https://developer.uber.com/docs/eats/guides/authentication)
- [Webhooks](https://developer.uber.com/docs/eats/guides/webhooks)
- [Dashboard](https://developer.uber.com/dashboard)
- [Terms of Service](https://developer.uber.com/docs/riders/policies/legal)
- [Blog](https://www.uber.com/newsroom/)
- [Status](https://status.uber.com/)
- [Spectral Rules](rules/uber-eats-rules.yml)
- [Vocabulary](vocabulary/uber-eats-vocabulary.yml)
- [Plans](plans/uber-eats-plans-pricing.yml)
- [Rate Limits](rate-limits/uber-eats-rate-limits.yml)
- [Fin Ops](finops/uber-eats-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
