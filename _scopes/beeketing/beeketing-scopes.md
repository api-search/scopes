---
authorization_urls:
- https://{shop}.onshopbase.com/admin/oauth/authorize
description: ''
docs: https://developers.shopbase.com/build-an-app/making-your-first-request/authentication/api-access-scopes.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Beeketing Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Beeketing publishes 24 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beeketing API on a user''s behalf.


  Tokens are issued from https://{shop}.onshopbase.com/admin/oauth/access_token.json.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beeketing
provider_slug: beeketing
schemes:
- flows:
  - authorizationUrl: https://{shop}.onshopbase.com/admin/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{shop}.onshopbase.com/admin/oauth/access_token.json
  name: PublicAppOAuth2
scope_count: 24
scope_names:
- read_themes
- write_themes
- read_products
- write_products
- read_product_listings
- read_inventory
- write_inventory
- read_customers
- write_customers
- read_orders
- write_orders
- read_fulfillments
- write_fulfillments
- read_script_tags
- write_script_tags
- read_content
- write_content
- read_shipping
- write_shipping
- read_checkouts
- write_checkouts
- read_price_rules
- write_price_rules
- read_analytics
scopes:
- description: Read access to Asset and Theme
  flows: []
  scope: read_themes
- description: Write access to Asset and Theme
  flows: []
  scope: write_themes
- description: Read Product
  flows: []
  scope: read_products
- description: Write Product
  flows: []
  scope: write_products
- description: Read Product Listing and Collection Listing
  flows: []
  scope: read_product_listings
- description: Read Inventory Level and Inventory Item
  flows: []
  scope: read_inventory
- description: Write Inventory Level and Inventory Item
  flows: []
  scope: write_inventory
- description: Read Customer Detail and Customer Group
  flows: []
  scope: read_customers
- description: Write Customer Detail and Customer Group
  flows: []
  scope: write_customers
- description: Read Order
  flows: []
  scope: read_orders
- description: Write Order
  flows: []
  scope: write_orders
- description: Read Fulfillment Service
  flows: []
  scope: read_fulfillments
- description: Write Fulfillment Service
  flows: []
  scope: write_fulfillments
- description: Read Script Tag
  flows: []
  scope: read_script_tags
- description: Write Script Tag
  flows: []
  scope: write_script_tags
- description: Read Page and Redirect
  flows: []
  scope: read_content
- description: Write Page and Redirect
  flows: []
  scope: write_content
- description: Read Carrier Service
  flows: []
  scope: read_shipping
- description: Write Carrier Service
  flows: []
  scope: write_shipping
- description: Read Checkouts
  flows: []
  scope: read_checkouts
- description: Write Checkouts
  flows: []
  scope: write_checkouts
- description: Read Price Rules
  flows: []
  scope: read_price_rules
- description: Write Price Rules
  flows: []
  scope: write_price_rules
- description: Read Analytics
  flows: []
  scope: read_analytics
slug: beeketing-scopes
source_filename: beeketing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.shopbase.com/build-an-app/making-your-first-request/authentication/api-access-scopes.md\ndocs: https://developers.shopbase.com/build-an-app/making-your-first-request/authentication/api-access-scopes.md\nschemes:\n- name: PublicAppOAuth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{shop}.onshopbase.com/admin/oauth/authorize\n    tokenUrl: https://{shop}.onshopbase.com/admin/oauth/access_token.json\nnotes: >-\n  Authenticated access scopes control access to REST Admin API and GraphQL Admin\n  API resources. Any write scope implicitly grants the matching read scope.\n  Granted scopes can be inspected via the AccessScope resource.\nscopes:\n- {scope: read_themes, description: Read access to Asset and Theme}\n- {scope: write_themes, description: Write access to Asset and Theme}\n- {scope: read_products, description: Read Product, Product Variant, Product Image, Product Custom Collection}\n\
  - {scope: write_products, description: Write Product, Product Variant, Product Image, Product Custom Collection}\n- {scope: read_product_listings, description: Read Product Listing and Collection Listing}\n- {scope: read_inventory, description: Read Inventory Level and Inventory Item}\n- {scope: write_inventory, description: Write Inventory Level and Inventory Item}\n- {scope: read_customers, description: Read Customer Detail and Customer Group}\n- {scope: write_customers, description: Write Customer Detail and Customer Group}\n- {scope: read_orders, description: Read Order, Transaction and Fulfillment}\n- {scope: write_orders, description: Write Order, Transaction and Fulfillment}\n- {scope: read_fulfillments, description: Read Fulfillment Service}\n- {scope: write_fulfillments, description: Write Fulfillment Service}\n- {scope: read_script_tags, description: Read Script Tag}\n- {scope: write_script_tags, description: Write Script Tag}\n- {scope: read_content, description: Read Page and\
  \ Redirect}\n- {scope: write_content, description: Write Page and Redirect}\n- {scope: read_shipping, description: Read Carrier Service, Shipping Rate, Country and Province}\n- {scope: write_shipping, description: Write Carrier Service, Shipping Rate, Country and Province}\n- {scope: read_checkouts, description: Read Checkouts}\n- {scope: write_checkouts, description: Write Checkouts}\n- {scope: read_price_rules, description: Read Price Rules}\n- {scope: write_price_rules, description: Write Price Rules}\n- {scope: read_analytics, description: Read Analytics}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeketing/refs/heads/main/scopes/beeketing-scopes.yml
summary_line: 24 scopes · authorizationCode
tags:
- Company
- E-commerce
- Cross-border Commerce
- Marketing
- Shopify Apps
- REST API
- OAuth
- Webhooks
- Themes
- Payments
token_urls:
- https://{shop}.onshopbase.com/admin/oauth/access_token.json
---
