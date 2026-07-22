---
authorization_urls: []
description: ''
docs: https://developer.shopline.com/docs/apps/api-instructions-for-use/access-scope
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Shopline Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SHOPLINE publishes 63 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SHOPLINE API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SHOPLINE
provider_slug: shopline
schemes:
- flows:
  - flow: authorizationCode
    note: Custom and Public apps request access scopes at install time; the issued accessToken carries the granted scopes. Scopes follow a read_<resource> / write_<resource> naming convention (a write scope generally implies its corresponding read access).
  name: OAuth2
scope_count: 63
scope_names:
- read_products
- write_products
- read_product_listings
- write_product_listings
- read_product_variant_images
- write_product_variant_images
- read_product_sizechart
- write_product_sizechart
- read_inventory
- write_inventory
- read_location
- read_orders
- write_orders
- read_draft_orders
- write_draft_orders
- write_checkouts
- read_returns
- write_return
- read_customers
- write_customers
- read_discounts
- write_discounts
- read_price_rules
- write_price_rules
- read_gift_card
- read_payment
- write_payment_gateways
- read_subscription_contracts
- write_subscription_contracts
- read_selling_plan_group
- write_selling_plan_group
- read_assigned_fulfillment_orders
- write_assigned_fulfillment_orders
- read_fulfillment_service
- write_fulfillment_service
- read_shipping
- write_shipping
- read_markets
- write_markets
- read_marketing_event
- write_marketing_event
- read_content
- write_content
- read_page
- write_page
- read_themes
- write_themes
- read_translation
- write_translation
- write_files
- read_publications
- write_publications
- read_script_tags
- write_script_tags
- read_store_information
- write_store_information
- read_shop_policy
- write_shop_policy
- read_store_staff
- read_store_log
- read_store_metrics
- read_bulkoperation
- write_bulkoperation
scopes:
- description: Read products
  flows: []
  scope: read_products
- description: Read and write products
  flows: []
  scope: write_products
- description: Read product listings
  flows: []
  scope: read_product_listings
- description: Read and write product listings
  flows: []
  scope: write_product_listings
- description: Read product variant images
  flows: []
  scope: read_product_variant_images
- description: Read and write product variant images
  flows: []
  scope: write_product_variant_images
- description: Read product size charts
  flows: []
  scope: read_product_sizechart
- description: Read and write product size charts
  flows: []
  scope: write_product_sizechart
- description: Read inventory
  flows: []
  scope: read_inventory
- description: Read and write inventory
  flows: []
  scope: write_inventory
- description: Read locations
  flows: []
  scope: read_location
- description: Read orders
  flows: []
  scope: read_orders
- description: Read and write orders
  flows: []
  scope: write_orders
- description: Read draft orders
  flows: []
  scope: read_draft_orders
- description: Read and write draft orders
  flows: []
  scope: write_draft_orders
- description: Read and write checkouts
  flows: []
  scope: write_checkouts
- description: Read returns
  flows: []
  scope: read_returns
- description: Read and write returns
  flows: []
  scope: write_return
- description: Read customers
  flows: []
  scope: read_customers
- description: Read and write customers
  flows: []
  scope: write_customers
- description: Read discounts
  flows: []
  scope: read_discounts
- description: Read and write discounts
  flows: []
  scope: write_discounts
- description: Read price rules
  flows: []
  scope: read_price_rules
- description: Read and write price rules
  flows: []
  scope: write_price_rules
- description: Read gift cards
  flows: []
  scope: read_gift_card
- description: Read payments
  flows: []
  scope: read_payment
- description: Read and write payment gateways
  flows: []
  scope: write_payment_gateways
- description: Read subscription contracts
  flows: []
  scope: read_subscription_contracts
- description: Read and write subscription contracts
  flows: []
  scope: write_subscription_contracts
- description: Read selling plan groups
  flows: []
  scope: read_selling_plan_group
- description: Read and write selling plan groups
  flows: []
  scope: write_selling_plan_group
- description: Read assigned fulfillment orders
  flows: []
  scope: read_assigned_fulfillment_orders
- description: Read and write assigned fulfillment orders
  flows: []
  scope: write_assigned_fulfillment_orders
- description: Read fulfillment services
  flows: []
  scope: read_fulfillment_service
- description: Read and write fulfillment services
  flows: []
  scope: write_fulfillment_service
- description: Read shipping
  flows: []
  scope: read_shipping
- description: Read and write shipping
  flows: []
  scope: write_shipping
- description: Read markets
  flows: []
  scope: read_markets
- description: Read and write markets
  flows: []
  scope: write_markets
- description: Read marketing events
  flows: []
  scope: read_marketing_event
- description: Read and write marketing events
  flows: []
  scope: write_marketing_event
- description: Read content
  flows: []
  scope: read_content
- description: Read and write content
  flows: []
  scope: write_content
- description: Read pages
  flows: []
  scope: read_page
- description: Read and write pages
  flows: []
  scope: write_page
- description: Read themes
  flows: []
  scope: read_themes
- description: Read and write themes
  flows: []
  scope: write_themes
- description: Read translations
  flows: []
  scope: read_translation
- description: Read and write translations
  flows: []
  scope: write_translation
- description: Read and write files
  flows: []
  scope: write_files
- description: Read publications
  flows: []
  scope: read_publications
- description: Read and write publications
  flows: []
  scope: write_publications
- description: Read script tags
  flows: []
  scope: read_script_tags
- description: Read and write script tags
  flows: []
  scope: write_script_tags
- description: Read store information
  flows: []
  scope: read_store_information
- description: Read and write store information
  flows: []
  scope: write_store_information
- description: Read shop policies
  flows: []
  scope: read_shop_policy
- description: Read and write shop policies
  flows: []
  scope: write_shop_policy
- description: Read store staff
  flows: []
  scope: read_store_staff
- description: Read store logs
  flows: []
  scope: read_store_log
- description: Read store metrics
  flows: []
  scope: read_store_metrics
- description: Read bulk operation tasks
  flows: []
  scope: read_bulkoperation
- description: Read and write bulk operation tasks
  flows: []
  scope: write_bulkoperation
slug: shopline-scopes
source_filename: shopline-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.shopline.com/docs/apps/api-instructions-for-use/access-scope\ndocs: https://developer.shopline.com/docs/apps/api-instructions-for-use/access-scope\nschemes:\n  - name: OAuth2\n    flows:\n      - flow: authorizationCode\n        note: >-\n          Custom and Public apps request access scopes at install time; the\n          issued accessToken carries the granted scopes. Scopes follow a\n          read_<resource> / write_<resource> naming convention (a write scope\n          generally implies its corresponding read access).\nmodel: read_<resource> / write_<resource>\nscopes:\n  - {scope: read_products, description: Read products}\n  - {scope: write_products, description: Read and write products}\n  - {scope: read_product_listings, description: Read product listings}\n  - {scope: write_product_listings, description: Read and write product listings}\n  - {scope: read_product_variant_images, description: Read\
  \ product variant images}\n  - {scope: write_product_variant_images, description: Read and write product variant images}\n  - {scope: read_product_sizechart, description: Read product size charts}\n  - {scope: write_product_sizechart, description: Read and write product size charts}\n  - {scope: read_inventory, description: Read inventory}\n  - {scope: write_inventory, description: Read and write inventory}\n  - {scope: read_location, description: Read locations}\n  - {scope: read_orders, description: Read orders}\n  - {scope: write_orders, description: Read and write orders}\n  - {scope: read_draft_orders, description: Read draft orders}\n  - {scope: write_draft_orders, description: Read and write draft orders}\n  - {scope: write_checkouts, description: Read and write checkouts}\n  - {scope: read_returns, description: Read returns}\n  - {scope: write_return, description: Read and write returns}\n  - {scope: read_customers, description: Read customers}\n  - {scope: write_customers, description:\
  \ Read and write customers}\n  - {scope: read_discounts, description: Read discounts}\n  - {scope: write_discounts, description: Read and write discounts}\n  - {scope: read_price_rules, description: Read price rules}\n  - {scope: write_price_rules, description: Read and write price rules}\n  - {scope: read_gift_card, description: Read gift cards}\n  - {scope: read_payment, description: Read payments}\n  - {scope: write_payment_gateways, description: Read and write payment gateways}\n  - {scope: read_subscription_contracts, description: Read subscription contracts}\n  - {scope: write_subscription_contracts, description: Read and write subscription contracts}\n  - {scope: read_selling_plan_group, description: Read selling plan groups}\n  - {scope: write_selling_plan_group, description: Read and write selling plan groups}\n  - {scope: read_assigned_fulfillment_orders, description: Read assigned fulfillment orders}\n  - {scope: write_assigned_fulfillment_orders, description: Read and write\
  \ assigned fulfillment orders}\n  - {scope: read_fulfillment_service, description: Read fulfillment services}\n  - {scope: write_fulfillment_service, description: Read and write fulfillment services}\n  - {scope: read_shipping, description: Read shipping}\n  - {scope: write_shipping, description: Read and write shipping}\n  - {scope: read_markets, description: Read markets}\n  - {scope: write_markets, description: Read and write markets}\n  - {scope: read_marketing_event, description: Read marketing events}\n  - {scope: write_marketing_event, description: Read and write marketing events}\n  - {scope: read_content, description: Read content}\n  - {scope: write_content, description: Read and write content}\n  - {scope: read_page, description: Read pages}\n  - {scope: write_page, description: Read and write pages}\n  - {scope: read_themes, description: Read themes}\n  - {scope: write_themes, description: Read and write themes}\n  - {scope: read_translation, description: Read translations}\n\
  \  - {scope: write_translation, description: Read and write translations}\n  - {scope: write_files, description: Read and write files}\n  - {scope: read_publications, description: Read publications}\n  - {scope: write_publications, description: Read and write publications}\n  - {scope: read_script_tags, description: Read script tags}\n  - {scope: write_script_tags, description: Read and write script tags}\n  - {scope: read_store_information, description: Read store information}\n  - {scope: write_store_information, description: Read and write store information}\n  - {scope: read_shop_policy, description: Read shop policies}\n  - {scope: write_shop_policy, description: Read and write shop policies}\n  - {scope: read_store_staff, description: Read store staff}\n  - {scope: read_store_log, description: Read store logs}\n  - {scope: read_store_metrics, description: Read store metrics}\n  - {scope: read_bulkoperation, description: Read bulk operation tasks}\n  - {scope: write_bulkoperation,\
  \ description: Read and write bulk operation tasks}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopline/refs/heads/main/scopes/shopline-scopes.yml
summary_line: 63 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Commerce
- Retail
- Point of Sale
- Storefront
- Payments
- Webhooks
- GraphQL
- Developer Platform
- Apps
token_urls: []
---
