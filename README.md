# Uber Eats (uber-eats)

Uber Eats exposes a family of developer APIs through the Uber Developer Portal that let restaurants, marketplace platforms, POS providers, and logistics partners integrate directly with Uber Eats and Uber Direct. The Uber Eats Marketplace APIs cover store onboarding, store status and hours, menu management, order ingestion and fulfillment, delivery fulfillment (Uber-courier and BYOC), promotions, and reporting. Uber Direct (Deliveries) exposes Uber's courier network for on-demand same-day delivery — quotes, deliveries, courier tracking, proof of delivery, refunds, pick-and-pack, and webhook notifications. All APIs are RESTful, JSON, and gated by OAuth 2.0 client credentials issued from the Uber Developer Portal.

**URL:** [Visit APIs.json URL](https://developer.uber.com/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

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
Onboards merchant stores onto a partner's Uber Eats integration, connecting Uber store identifiers to a partner platform.

**Human URL:** [Integration Activation Suite](https://developer.uber.com/docs/eats/references/api/integration_activation_suite)

### Uber Eats Store API
Manages store status (online/offline), business hours, holiday schedules, and store configuration on Uber Eats.

**Human URL:** [Store Suite](https://developer.uber.com/docs/eats/references/api/store_suite)

#### Properties
- [Documentation](https://developer.uber.com/docs/eats/references/api/store_suite)
- [OpenAPI](openapi/uber-eats-openapi.yml)
- [NaftikoCapability](capabilities/eats-general.yaml)

### Uber Eats Menu API
Retrieve and upsert full menus for a store and update individual items, modifier groups, prices, suspensions, and availability.

**Human URL:** [Menu Suite](https://developer.uber.com/docs/eats/references/api/v2/)

### Uber Eats Order API
Handles inbound Uber Eats orders, including accept/deny, status updates, item-level adjustments, and cancellation flows.

**Human URL:** [Order Suite](https://developer.uber.com/docs/eats/references/api/order_suite)

### Uber Eats Delivery Partner API
Delivery fulfillment by Uber couriers for Uber Eats orders — courier assignment, tracking, and status updates.

**Human URL:** [Delivery Partner Suite](https://developer.uber.com/docs/eats/references/api/delivery_partner_suite)

### Uber Eats Delivery BYOC API
Supports merchants and partners that use their own delivery fleet (Bring Your Own Courier).

**Human URL:** [Delivery BYOC Suite](https://developer.uber.com/docs/eats/references/api/delivery_byoc_suite)

### Uber Eats Promotions API
Creates and manages marketing campaigns and discounts on Uber Eats stores.

**Human URL:** [Promotions Suite](https://developer.uber.com/docs/eats/references/api/promotions_suite)

### Uber Eats Reporting API
Returns transactional, financial, and performance reports for Uber Eats stores.

**Human URL:** [Reporting Suite](https://developer.uber.com/docs/eats/references/api/reporting_suite)

### Uber Direct (Deliveries) API
Uber's courier network as a delivery-as-a-service API — quotes, deliveries, courier tracking, and proof of delivery.

**Human URL:** [Uber Direct Overview](https://developer.uber.com/docs/deliveries/overview)

#### Properties
- [Documentation](https://developer.uber.com/docs/deliveries/overview)
- [APIReference](https://developer.uber.com/docs/deliveries/references/api)
- [OpenAPI](openapi/uber-direct-openapi.yml)
- [SDK — JavaScript/TypeScript](https://www.npmjs.com/package/uber-direct)
- [CodeExamples — Uber Direct SDK Samples](https://github.com/uber/uber-direct-sdk-samples)
- [NaftikoCapability](capabilities/uber-direct-general.yaml)

### Uber Direct Organizations API
Manage parent organizations and child accounts for multi-tenant merchants.

**Human URL:** [Organizations](https://developer.uber.com/docs/deliveries/references/api/organizations)

### Uber Direct Courier Pick & Pack API
Shop-and-pay style deliveries where the courier shops on behalf of the customer.

**Human URL:** [Pick and Pack](https://developer.uber.com/docs/deliveries/references/api/pick-and-pack)

### Uber Direct Refund API
Refund requests on completed Uber Direct deliveries and the corresponding webhook events.

**Human URL:** [Refunds](https://developer.uber.com/docs/deliveries/references/api/refunds)

### Uber Direct Business Location Management API
Administers physical pickup locations associated with Uber Direct accounts.

**Human URL:** [Locations](https://developer.uber.com/docs/deliveries/references/api/locations)

### Uber Eats & Direct Webhooks
Webhook events for order lifecycle, courier updates, refunds, shopping progress, and delivery status.

**Human URL:** [Webhooks](https://developer.uber.com/docs/eats/guides/webhooks)

### Uber OAuth 2.0
OAuth 2.0 authentication — client_credentials for server-to-server and authorization_code with PKCE for user-facing.

**Human URL:** [Authentication](https://developer.uber.com/docs/eats/guides/authentication)

## Common Properties

- [Website](https://www.uber.com/us/en/business/products/eats/)
- [GitHubOrganization](https://github.com/uber)
- [SDK — Uber Direct JavaScript/TypeScript SDK](https://github.com/uber/uber-direct-sdk)
- [DeveloperPortal](https://developer.uber.com/)
- [Documentation](https://developer.uber.com/docs)
- [Dashboard](https://developer.uber.com/dashboard)
- [Status](https://status.uber.com/)
- [SpectralRules](rules/uber-eats-rules.yml)
- [Vocabulary](vocabulary/uber-eats-vocabulary.yml)
- [Plans](plans/uber-eats-plans-pricing.yml)
- [RateLimits](rate-limits/uber-eats-rate-limits.yml)
- [FinOps](finops/uber-eats-finops.yml)

## Features

| Name | Description |
|------|-------------|
| Full Marketplace Coverage | Onboarding, stores, menus, orders, fulfillment, promotions, and reporting all available as APIs. |
| Multiple Fulfillment Models | Supports Uber-courier delivery, partner-courier (BYOC), and merchant-handled pickup flows. |
| Uber Direct Logistics | Same platform exposes Uber's courier network for delivery-as-a-service outside Uber Eats. |
| Webhooks | Real-time event notifications for orders, deliveries, courier updates, and refunds. |
| OAuth 2.0 | Standard OAuth 2.0 client-credentials and authorization-code flows. |
| Partner Portal | Centralized Developer Portal for app creation, credentials, scopes, sandbox keys, and analytics. |

## Use Cases

| Name | Description |
|------|-------------|
| POS Integration | Pipe Uber Eats orders into a restaurant's POS system and stream status updates back to Uber. |
| Menu Management | Sync menu changes from a merchant's master catalog to all Uber Eats stores. |
| Marketplace Aggregation | Multi-brand operators centrally manage many Uber Eats stores via a single integration. |
| Same-Day Delivery | Use Uber Direct to offer on-demand last-mile delivery for ecommerce, grocery, retail, and pharmacy. |
| Multi-Brand Operations | Manage shared kitchens, virtual brands, and cloud kitchens across many storefronts. |
| Financial Reconciliation | Pull reporting data to reconcile Uber Eats settlements with internal financial systems. |

## Integrations

| Name |
|------|
| Toast POS |
| Square |
| Olo |
| Lightspeed |
| NCR |
| Oracle Micros |
| Otter |
| Deliverect |
| Shopify |
| WooCommerce |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Uber Eats Marketplace API](openapi/uber-eats-openapi.yml)
- [Uber Direct (DaaS) API](openapi/uber-direct-openapi.yml)

### JSON Schema

13 schema files extracted from the OpenAPI specs in [json-schema/](json-schema/).

### JSON Structure

13 JSON Structure files in [json-structure/](json-structure/).

### JSON-LD

- [Uber Eats Marketplace Context](json-ld/uber-eats-eats-context.jsonld)
- [Uber Direct Context](json-ld/uber-eats-uber-direct-context.jsonld)

### Examples

13 example payloads in [examples/](examples/).

## Capabilities

Self-contained Naftiko capabilities, one per business surface, each exposing both a REST and an MCP adapter.

| Capability | APIs Combined | MCP Tools | Persona |
|----------|--------------|-------|---------|
| [Eats Marketplace](capabilities/eats-general.yaml) | Uber Eats Marketplace API | 10 | POS Integrator |
| [Uber Direct Delivery](capabilities/uber-direct-general.yaml) | Uber Direct (DaaS) API | 7 | Logistics Partner |

## Vocabulary

- [Uber Eats Vocabulary](vocabulary/uber-eats-vocabulary.yml) — Unified taxonomy mapping 14 resources, 9 actions, 2 workflows, and 4 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Uber Eats Spectral Rules](rules/uber-eats-rules.yml) — 25 rules across metadata, paths, operations, parameters, responses, schemas, security, and HTTP-method categories enforcing Uber Eats / Uber Direct API conventions.

## Commercial

- [Plans & Pricing](plans/uber-eats-plans-pricing.yml) — API access is free to approved partners; revenue via marketplace commission (Lite 20% / Plus 25% / Premium 30%, US effective 2026-03-11) and Uber Direct flat per-delivery fee (from $7.99).
- [Rate Limits](rate-limits/uber-eats-rate-limits.yml)
- [FinOps](finops/uber-eats-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
