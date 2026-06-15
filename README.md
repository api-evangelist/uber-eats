# Uber Eats (uber-eats)

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
