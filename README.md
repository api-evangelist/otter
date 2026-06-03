# Otter (otter)
Otter (TryOtter) is a Restaurant Operating System used by hundreds of thousands of restaurants worldwide to aggregate delivery and online orders, consolidate menus, analyze sales, and control third-party delivery services from one place. For developers and integration partners, Otter publishes a Public API (OpenAPI 3.0, OAuth 2.0) and developer guides spanning account pairing, orders, menus, delivery, finance, reports, reviews, storefront, loyalty, organization, and inventory — with HMAC-signed webhooks for event-driven integration. Onboarding begins by registering an application, configuring webhooks, and onboarding stores; authentication and the account-specific base URL are provisioned through an Otter account representative.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Restaurant, Order Management, Delivery, Online Ordering, Menu Management, Analytics

## Timestamps

- **Created:** 2026-06-02
- **Modified:** 2026-06-03

## APIs

### Otter Public API
The Otter Public API enables integrations across the digital food ecosystem, covering account pairing, orders, menus, delivery, finance, reports, reviews, storefront, loyalty, and store management. Integrations combine API endpoints with webhooks and configuration; onboarding starts by registering an application, configuring webhooks, and onboarding stores. Auth and base URL details are provided via an account representative and the OpenAPI reference.

**Human URL:** [https://developer-guides.tryotter.com/docs/](https://developer-guides.tryotter.com/docs/)

**Base URL:** `https://{public-api-url}`

#### Tags:

 - Orders, Menu, Delivery, Webhooks, Reports

#### Properties

- [Documentation](https://developer-guides.tryotter.com/docs/)
- [GettingStarted](https://developer-guides.tryotter.com/docs/)
- [OpenAPI](openapi/otter-public-api-openapi.yml)
- [APIReference](https://developer-guides.tryotter.com/api-reference/)
- [Authentication](https://developer-guides.tryotter.com/api-reference/#operation/requestToken)
- [Webhooks](https://developer-guides.tryotter.com/docs/guides-webhook-authentication/)
- [RateLimits](rate-limits/otter-rate-limits.yml)
- [JSONSchema](json-schema/)
- [JSONStructure](json-structure/)
- [Example](examples/)
- NaftikoCapability — 27 capability files (see Capabilities section below)

## Common Properties

- [Website](https://www.tryotter.com)
- [Documentation](https://developer-guides.tryotter.com/docs/)
- [Support](https://helpdesk.tryotter.com/hc/en-us/articles/22694653065107-API-Documentation)
- [Blog](https://www.tryotter.com/blog)
- [LinkedIn](https://www.linkedin.com/company/try-otter)
- [X](https://twitter.com/try_otter)
- [SpectralRules](rules/otter-public-api-rules.yml)
- [JSONLD](json-ld/otter-public-api-context.jsonld)
- [Vocabulary](vocabulary/otter-vocabulary.yml)
- [Plans](plans/otter-plans-pricing.yml)
- [RateLimits](rate-limits/otter-rate-limits.yml)
- [FinOps](finops/otter-finops.yml)
- [Pricing](https://www.tryotter.com/pricing)
- [GitHubRepository](https://github.com/api-evangelist/otter)

## Features

| Name | Description |
|------|-------------|
| Order Aggregation | Receive, confirm, update, and fulfill orders from multiple delivery and online-ordering channels through a single Public API. |
| Menu Management | Upsert, publish, and synchronize menus, hours, and item availability across connected storefronts and channels. |
| Delivery Orchestration | Request delivery quotes, create and update delivery requests, and track courier status via webhooks. |
| Finance & Payouts | Post financial transactions and invoices and retrieve payout and order-total data. |
| Reports | Generate orders, items, payouts, and ratings/reviews reports for stores over a time period. |
| Reviews & Loyalty | Reply to customer reviews and compute, redeem, accumulate, refund, and simulate loyalty rewards. |
| Storefront Control | Pause and unpause storefronts and report store availability and hours configuration. |
| Account Pairing & Organization | Onboard stores, manage store links, and read organization, brand, and store data via OAuth authorization-code flow. |
| Webhooks | Subscribe to order, menu, delivery, storefront, reports, and account-pairing events signed with HMAC-SHA256. |

## Use Cases

| Name | Description |
|------|-------------|
| POS Integration | Sync orders and menus between a third-party point-of-sale system and Otter-connected channels. |
| Delivery Provider Integration | Provide delivery services by responding to quote and delivery-request webhooks and posting status updates. |
| Menu Aggregator | Centrally manage and publish menus and availability across many stores and storefronts. |
| Financial Reconciliation | Pull payout, order-total, and transaction data to reconcile restaurant finances. |
| Loyalty Program | Power a loyalty program by computing and redeeming rewards against Otter orders. |

## Integrations

| Name | Description |
|------|-------------|
| Delivery Service Providers | Third-party delivery marketplaces and on-demand courier networks. |
| Point of Sale Platforms | Restaurant POS systems exchanging orders and menus with Otter. |
| Online Ordering Channels | Branded and third-party online ordering storefronts aggregated by Otter. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [otter-public-api-openapi.yml](openapi/otter-public-api-openapi.yml)

### JSON Schema

- 319 JSON Schema files in [`json-schema/`](json-schema/) extracted from the OpenAPI component schemas.

### JSON Structure

- 319 JSON Structure files in [`json-structure/`](json-structure/).

### JSON-LD

- [otter-public-api-context.jsonld](json-ld/otter-public-api-context.jsonld)

### Examples

- 319 example payloads in [`examples/`](examples/), one per schema.

## Capabilities

Self-contained Naftiko capabilities — one per Otter Public API business surface (OpenAPI tag), each exposing both a REST and an MCP adapter.

| Capability | Tools | File |
|------------|-------|------|
| Otter Public API — Account Pairing Endpoints | 2 | [public-api-account-pairing-endpoints.yaml](capabilities/public-api-account-pairing-endpoints.yaml) |
| Otter Public API — Account Pairing Webhooks | 3 | [public-api-account-pairing-webhooks.yaml](capabilities/public-api-account-pairing-webhooks.yaml) |
| Otter Public API — Auth Endpoints | 2 | [public-api-auth-endpoints.yaml](capabilities/public-api-auth-endpoints.yaml) |
| Otter Public API — Callback Endpoints | 1 | [public-api-callback-endpoints.yaml](capabilities/public-api-callback-endpoints.yaml) |
| Otter Public API — Delivery Endpoints | 6 | [public-api-delivery-endpoints.yaml](capabilities/public-api-delivery-endpoints.yaml) |
| Otter Public API — Delivery Webhooks | 5 | [public-api-delivery-webhooks.yaml](capabilities/public-api-delivery-webhooks.yaml) |
| Otter Public API — Direct Orders Endpoints | 1 | [public-api-direct-orders-endpoints.yaml](capabilities/public-api-direct-orders-endpoints.yaml) |
| Otter Public API — Finance Endpoints | 2 | [public-api-finance-endpoints.yaml](capabilities/public-api-finance-endpoints.yaml) |
| Otter Public API — Inventory Endpoints | 3 | [public-api-inventory-endpoints.yaml](capabilities/public-api-inventory-endpoints.yaml) |
| Otter Public API — Manager Loyalty Endpoints | 8 | [public-api-manager-loyalty-endpoints.yaml](capabilities/public-api-manager-loyalty-endpoints.yaml) |
| Otter Public API — Manager Menu Endpoints | 8 | [public-api-manager-menu-endpoints.yaml](capabilities/public-api-manager-menu-endpoints.yaml) |
| Otter Public API — Manager Order Endpoints | 11 | [public-api-manager-order-endpoints.yaml](capabilities/public-api-manager-order-endpoints.yaml) |
| Otter Public API — Manager Orders Webhooks | 6 | [public-api-manager-orders-webhooks.yaml](capabilities/public-api-manager-orders-webhooks.yaml) |
| Otter Public API — Manager Storefront Endpoints | 4 | [public-api-manager-storefront-endpoints.yaml](capabilities/public-api-manager-storefront-endpoints.yaml) |
| Otter Public API — Market Intel Endpoints | 1 | [public-api-market-intel-endpoints.yaml](capabilities/public-api-market-intel-endpoints.yaml) |
| Otter Public API — Menus Endpoints | 6 | [public-api-menus-endpoints.yaml](capabilities/public-api-menus-endpoints.yaml) |
| Otter Public API — Menus Webhooks | 4 | [public-api-menus-webhooks.yaml](capabilities/public-api-menus-webhooks.yaml) |
| Otter Public API — Orders Endpoints | 6 | [public-api-orders-endpoints.yaml](capabilities/public-api-orders-endpoints.yaml) |
| Otter Public API — Orders Webhooks | 3 | [public-api-orders-webhooks.yaml](capabilities/public-api-orders-webhooks.yaml) |
| Otter Public API — Organization Endpoints | 8 | [public-api-organization-endpoints.yaml](capabilities/public-api-organization-endpoints.yaml) |
| Otter Public API — Ping Endpoints | 1 | [public-api-ping-endpoints.yaml](capabilities/public-api-ping-endpoints.yaml) |
| Otter Public API — Ping Webhooks | 1 | [public-api-ping-webhooks.yaml](capabilities/public-api-ping-webhooks.yaml) |
| Otter Public API — Reports Endpoints | 2 | [public-api-reports-endpoints.yaml](capabilities/public-api-reports-endpoints.yaml) |
| Otter Public API — Reports Webhooks | 1 | [public-api-reports-webhooks.yaml](capabilities/public-api-reports-webhooks.yaml) |
| Otter Public API — Reviews Endpoints | 1 | [public-api-reviews-endpoints.yaml](capabilities/public-api-reviews-endpoints.yaml) |
| Otter Public API — Storefront Endpoints | 7 | [public-api-storefront-endpoints.yaml](capabilities/public-api-storefront-endpoints.yaml) |
| Otter Public API — Storefront Webhooks | 4 | [public-api-storefront-webhooks.yaml](capabilities/public-api-storefront-webhooks.yaml) |

## Vocabulary

- [Otter Vocabulary](vocabulary/otter-vocabulary.yml) — Unified taxonomy mapping 44 resources, 24 actions, and 27 capability workflows across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Otter Public API Spectral Ruleset](rules/otter-public-api-rules.yml) — 29 rules enforcing Otter Public API conventions.

## Plans & Pricing

- [Plans & Pricing](plans/otter-plans-pricing.yml)

## Rate Limits

- [Rate Limits](rate-limits/otter-rate-limits.yml)

## FinOps

- [FinOps](finops/otter-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
