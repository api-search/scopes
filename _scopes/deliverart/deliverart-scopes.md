---
api_specs:
- filename: deliverart-openapi.yml
  format: yaml
  label: Deliverart API
  slug: deliverart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-openapi.yml
authorization_urls: []
description: ''
docs: https://apidoc.deliverart.it/
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Deliverart Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Deliverart publishes 44 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deliverart API on a user''s behalf.


  Tokens are issued from https://auth.deliverart.it/oauth.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deliverart
provider_slug: deliverart
schemes:
- description: OAuth2 password grant. Token endpoint is on the auth host.
  flows:
  - flow: password
    tokenUrl: https://auth.deliverart.it/oauth
  name: oauth2
  source: openapi/deliverart-openapi.yml
scope_count: 44
scope_names:
- address_admin
- address_create
- address_read
- company_admin
- company_pos_read
- company_read
- create_customer
- customer_address_create
- customer_address_read
- customer_address_update
- customer_admin
- customer_business_profile_create
- customer_business_profile_read
- customer_business_profile_update
- customer_orders_read
- customer_read
- customer_update
- deliveries_fee_read
- deliveries_read
- delivery_admin
- delivery_fee_admin
- delivery_fee_read
- delivery_read
- menu_admin
- menu_item_admin
- menu_item_allergen_admin
- menu_item_category_admin
- menu_item_ingredient_admin
- menu_read
- order_abort
- order_admin
- order_cancel
- order_create
- order_list
- order_read
- order_update
- point_of_sale_admin
- point_of_sale_read
- read_customer
- take_away_admin
- take_away_read
- take_away_time_read
- workshifts_admin
- workshifts_read
scopes:
- description: Manage addresses
  flows:
  - password
  scope: address_admin
- description: Create addresses
  flows:
  - password
  scope: address_create
- description: Read addresses
  flows:
  - password
  scope: address_read
- description: Full company management
  flows:
  - password
  scope: company_admin
- description: Read company points of sale
  flows:
  - password
  scope: company_pos_read
- description: Read company
  flows:
  - password
  scope: company_read
- description: Create customers
  flows:
  - password
  scope: create_customer
- description: Create customer addresses
  flows:
  - password
  scope: customer_address_create
- description: Read customer addresses
  flows:
  - password
  scope: customer_address_read
- description: Update customer addresses
  flows:
  - password
  scope: customer_address_update
- description: Full customer management
  flows:
  - password
  scope: customer_admin
- description: Create customer business profiles
  flows:
  - password
  scope: customer_business_profile_create
- description: Read customer business profiles
  flows:
  - password
  scope: customer_business_profile_read
- description: Update customer business profiles
  flows:
  - password
  scope: customer_business_profile_update
- description: Read customer orders
  flows:
  - password
  scope: customer_orders_read
- description: Read customers
  flows:
  - password
  scope: customer_read
- description: Update customers
  flows:
  - password
  scope: customer_update
- description: Read delivery fees
  flows:
  - password
  scope: deliveries_fee_read
- description: Read deliveries
  flows:
  - password
  scope: deliveries_read
- description: Full delivery management
  flows:
  - password
  scope: delivery_admin
- description: Manage delivery fees
  flows:
  - password
  scope: delivery_fee_admin
- description: Read delivery fees
  flows:
  - password
  scope: delivery_fee_read
- description: Read deliveries
  flows:
  - password
  scope: delivery_read
- description: Full menu management
  flows:
  - password
  scope: menu_admin
- description: Manage menu items
  flows:
  - password
  scope: menu_item_admin
- description: Manage menu allergens
  flows:
  - password
  scope: menu_item_allergen_admin
- description: Manage menu categories
  flows:
  - password
  scope: menu_item_category_admin
- description: Manage menu ingredients
  flows:
  - password
  scope: menu_item_ingredient_admin
- description: Read menu
  flows:
  - password
  scope: menu_read
- description: Abort orders
  flows:
  - password
  scope: order_abort
- description: Full order management
  flows:
  - password
  scope: order_admin
- description: Cancel orders
  flows:
  - password
  scope: order_cancel
- description: Create orders
  flows:
  - password
  scope: order_create
- description: List orders
  flows:
  - password
  scope: order_list
- description: Read orders
  flows:
  - password
  scope: order_read
- description: Update orders
  flows:
  - password
  scope: order_update
- description: Full point-of-sale management
  flows:
  - password
  scope: point_of_sale_admin
- description: Read points of sale
  flows:
  - password
  scope: point_of_sale_read
- description: Read customer
  flows:
  - password
  scope: read_customer
- description: Manage take-away
  flows:
  - password
  scope: take_away_admin
- description: Read take-away
  flows:
  - password
  scope: take_away_read
- description: Read take-away times
  flows:
  - password
  scope: take_away_time_read
- description: Manage workshifts
  flows:
  - password
  scope: workshifts_admin
- description: Read workshifts
  flows:
  - password
  scope: workshifts_read
slug: deliverart-scopes
source_filename: deliverart-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/deliverart-openapi.yml\ndocs: https://apidoc.deliverart.it/\nschemes:\n- name: oauth2\n  source: openapi/deliverart-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://auth.deliverart.it/oauth\n  description: OAuth2 password grant. Token endpoint is on the auth host.\nscopes:\n- scope: address_admin\n  description: Manage addresses\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: address_create\n  description: Create addresses\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: address_read\n  description: Read addresses\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: company_admin\n  description: Full company management\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: company_pos_read\n  description: Read company points of sale\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n\
  - scope: company_read\n  description: Read company\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: create_customer\n  description: Create customers\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: customer_address_create\n  description: Create customer addresses\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: customer_address_read\n  description: Read customer addresses\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: customer_address_update\n  description: Update customer addresses\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: customer_admin\n  description: Full customer management\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: customer_business_profile_create\n  description: Create customer business profiles\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n-\
  \ scope: customer_business_profile_read\n  description: Read customer business profiles\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: customer_business_profile_update\n  description: Update customer business profiles\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: customer_orders_read\n  description: Read customer orders\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: customer_read\n  description: Read customers\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: customer_update\n  description: Update customers\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: deliveries_fee_read\n  description: Read delivery fees\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: deliveries_read\n  description: Read deliveries\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope:\
  \ delivery_admin\n  description: Full delivery management\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: delivery_fee_admin\n  description: Manage delivery fees\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: delivery_fee_read\n  description: Read delivery fees\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: delivery_read\n  description: Read deliveries\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: menu_admin\n  description: Full menu management\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: menu_item_admin\n  description: Manage menu items\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: menu_item_allergen_admin\n  description: Manage menu allergens\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: menu_item_category_admin\n  description: Manage menu\
  \ categories\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: menu_item_ingredient_admin\n  description: Manage menu ingredients\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: menu_read\n  description: Read menu\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: order_abort\n  description: Abort orders\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: order_admin\n  description: Full order management\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: order_cancel\n  description: Cancel orders\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: order_create\n  description: Create orders\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: order_list\n  description: List orders\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: order_read\n\
  \  description: Read orders\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: order_update\n  description: Update orders\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: point_of_sale_admin\n  description: Full point-of-sale management\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: point_of_sale_read\n  description: Read points of sale\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: read_customer\n  description: Read customer\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: take_away_admin\n  description: Manage take-away\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: take_away_read\n  description: Read take-away\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: take_away_time_read\n  description: Read take-away times\n  flows:\n  - password\n  sources:\n\
  \  - openapi/deliverart-openapi.yml\n- scope: workshifts_admin\n  description: Manage workshifts\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n- scope: workshifts_read\n  description: Read workshifts\n  flows:\n  - password\n  sources:\n  - openapi/deliverart-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/scopes/deliverart-scopes.yml
summary_line: 44 scopes · password
tags:
- Company
- Food Delivery
- Restaurants
- Order Management
- Logistics
- Delivery
- Menu Management
- Point of Sale
token_urls:
- https://auth.deliverart.it/oauth
---
