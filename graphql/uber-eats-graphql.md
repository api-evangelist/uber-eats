# Uber Eats GraphQL Schema

## Overview

This conceptual GraphQL schema represents the Uber Eats platform API domain, covering restaurant and store management, menus, orders, delivery fulfillment, promotions, customer data, and reporting. Uber Eats exposes its services through REST APIs (Uber Eats Marketplace APIs and Uber Direct), but this schema models the underlying domain as a unified GraphQL surface to support integration tooling, federation design, and API documentation.

The schema is derived from the publicly documented Uber Eats API reference at https://developer.uber.com/docs/eats/introduction and the Uber Direct delivery API at https://developer.uber.com/docs/deliveries/overview.

## Schema Source

- **Provider:** Uber Eats
- **Source:** Conceptual — derived from REST API documentation
- **Reference Docs:** https://developer.uber.com/docs/eats/introduction
- **Schema File:** uber-eats-schema.graphql

## Domain Coverage

### Restaurant and Store Management

Types covering store identity, configuration, operating hours, holiday schedules, and status management. The `Restaurant` and `RestaurantDetails` types model merchant locations, while `StoreHours`, `OperatingHours`, and `Holiday` capture scheduling. Store status (online/paused/offline) is represented through `StoreStatus`.

### Menu and Catalog

The menu domain is modeled as a tree: `Menu` contains `MenuCategory` items, each holding `MenuItem` objects. Items have `MenuItemDetails`, `MenuPhoto`, `MenuBadge`, and availability windows (`ItemAvailability`). Modifiers are organized through `ModifierGroup` and `Modifier` types with `ModifierPrice` for price overrides. Nutritional and allergen data are represented by `Nutritional`, `Allergen`, `DietaryInfo`, and `ItemAttribute`.

### Ordering and Cart

Cart and checkout flow types (`Cart`, `CartItem`, `CartModifier`, `CartSummary`, `Checkout`) model the customer order-building experience. The `Order` type captures the full order lifecycle, with `OrderStatus`, `OrderHistory`, and `OrderFulfillment` tracking state transitions. Pricing is encapsulated in `Price`.

### Delivery and Tracking

Delivery estimation and real-time tracking are covered by `DeliveryEstimate`, `DeliveryFee`, `PickupEstimate`, `DeliveryDriver`, `DriverLocation`, `DeliveryTracking`, and `TrackingStatus`. These align with both Uber-courier fulfillment and BYOC (Bring Your Own Courier) flows.

### Refunds and Disputes

`OrderRefund`, `RefundAmount`, and `RefundReason` model the refund lifecycle for both Uber Eats order-level refunds and Uber Direct delivery refunds.

### Customer and Address

Customer identity, address management, and payment are covered by `Customer`, `CustomerAddress`, `DeliveryAddress`, `GeoLocation`, and `PaymentMethod`.

### Promotions and Loyalty

Marketing and incentive types include `Promotion`, `MenuPromotion`, `DiscountOffer`, `Coupon`, `LoyaltyPoint`, and `EatsPass` (Uber Eats subscription program).

### Ratings and Reviews

`Rating`, `Review`, and `ReviewResponse` model the post-order feedback loop between customers and restaurants.

### Discovery and Filtering

`Cuisine`, `FoodCategory`, and `DietaryFilter` support menu search, browse, and filtering experiences.

### Authentication and Webhooks

`APIKey`, `Token`, and `Webhook` represent the authentication and event-notification infrastructure backed by OAuth 2.0 client credentials and webhook signature verification.

## Types Summary

| Domain | Types |
|---|---|
| Restaurant/Store | Restaurant, RestaurantDetails, StoreStatus, StoreHours, OperatingHours, Holiday |
| Menu/Catalog | Menu, MenuCategory, MenuItem, MenuItemDetails, MenuPhoto, MenuBadge, ItemAvailability, ItemAttribute |
| Allergens/Nutrition | Allergen, Nutritional, DietaryInfo |
| Pricing | Price, ModifierPrice |
| Modifiers | MenuItemModifier, ModifierGroup, Modifier |
| Order/Cart | Order, Cart, CartItem, CartModifier, CartSummary, Checkout |
| Delivery | DeliveryEstimate, DeliveryFee, PickupEstimate, OrderFulfillment, DeliveryDriver, DriverLocation, DeliveryTracking, TrackingStatus |
| Order Lifecycle | OrderStatus, OrderHistory |
| Refunds | OrderRefund, RefundAmount, RefundReason |
| Customer | Customer, CustomerAddress, DeliveryAddress, GeoLocation, PaymentMethod |
| Promotions | Promotion, MenuPromotion, DiscountOffer, Coupon, LoyaltyPoint, EatsPass |
| Ratings | Rating, Review, ReviewResponse |
| Discovery | Cuisine, FoodCategory, DietaryFilter |
| Auth/Webhooks | APIKey, Token, Webhook |

## Usage Notes

This schema is intended for design reference and tooling integration. Uber Eats does not publish a public GraphQL API; all production integrations use the REST endpoints documented at https://developer.uber.com/docs/eats/references/api and https://developer.uber.com/docs/deliveries/references/api. Authentication uses OAuth 2.0 client credentials obtained from the Uber Developer Portal at https://developer.uber.com/dashboard.
