---
api_specs:
- filename: shoplazza-admin-openapi-original.json
  format: json
  label: Shoplazza Admin API
  slug: shoplazza-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-admin-openapi-original.json
authorization_urls: []
description: ''
docs: https://www.shoplazza.dev/docs/app/building-blocks/authentication/access-scopes/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Shoplazza Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Shoplazza publishes 29 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Shoplazza API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Shoplazza
provider_slug: shoplazza
schemes:
- flow: authorizationCode
  name: OAuth2
  source: docs
scope_count: 29
scope_names:
- read_shop
- read_themes
- write_themes
- read_shop_navigation
- write_shop_navigation
- read_product
- write_product
- read_collection
- write_collection
- read_comments
- write_comments
- read_payment_info
- write_payment_info
- read_order
- write_order
- read_customer
- write_customer
- read_price_rules
- write_price_rules
- read_gift_cards
- write_gift_cards
- read_app_proxy
- write_app_proxy
- read_data
- write_data
- read_script_tags
- write_script_tags
- read_finance
- write_finance
scopes:
- description: Read access to shop information.
  flows: []
  scope: read_shop
- description: Read access to theme management.
  flows: []
  scope: read_themes
- description: Write access to theme management.
  flows: []
  scope: write_themes
- description: Read access to pages, blogs, articles, and redirects.
  flows: []
  scope: read_shop_navigation
- description: Write access to pages, blogs, articles, and redirects.
  flows: []
  scope: write_shop_navigation
- description: Read access to products and variants.
  flows: []
  scope: read_product
- description: Write access to products and variants.
  flows: []
  scope: write_product
- description: Read access to collections and collects.
  flows: []
  scope: read_collection
- description: Write access to collections and collects.
  flows: []
  scope: write_collection
- description: Read access to comments.
  flows: []
  scope: read_comments
- description: Write access to comments.
  flows: []
  scope: write_comments
- description: Read access to payments apps.
  flows: []
  scope: read_payment_info
- description: Write access to payments apps.
  flows: []
  scope: write_payment_info
- description: Read access to orders.
  flows: []
  scope: read_order
- description: Write access to orders.
  flows: []
  scope: write_order
- description: Read access to customers.
  flows: []
  scope: read_customer
- description: Write access to customers.
  flows: []
  scope: write_customer
- description: Read access to price rules — discount codes, coupons, flash sales, rebates, popups, and sales pops.
  flows: []
  scope: read_price_rules
- description: Write access to price rules — discount codes, coupons, flash sales, rebates, popups, and sales pops.
  flows: []
  scope: write_price_rules
- description: Read access to gift cards.
  flows: []
  scope: read_gift_cards
- description: Write access to gift cards.
  flows: []
  scope: write_gift_cards
- description: Read access to app proxies.
  flows: []
  scope: read_app_proxy
- description: Write access to app proxies.
  flows: []
  scope: write_app_proxy
- description: Read access to data.
  flows: []
  scope: read_data
- description: Write access to data.
  flows: []
  scope: write_data
- description: Read access to script tags.
  flows: []
  scope: read_script_tags
- description: Write access to script tags.
  flows: []
  scope: write_script_tags
- description: Read access to Shoplazza payment information.
  flows: []
  scope: read_finance
- description: Write access to Shoplazza payment information.
  flows: []
  scope: write_finance
slug: shoplazza-scopes
source_filename: shoplazza-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.shoplazza.dev/docs/app/building-blocks/authentication/access-scopes/\ndocs: https://www.shoplazza.dev/docs/app/building-blocks/authentication/access-scopes/\nschemes:\n- name: OAuth2\n  flow: authorizationCode\n  source: docs\nscopes:\n- scope: read_shop\n  description: Read access to shop information.\n- scope: read_themes\n  description: Read access to theme management.\n- scope: write_themes\n  description: Write access to theme management.\n- scope: read_shop_navigation\n  description: Read access to pages, blogs, articles, and redirects.\n- scope: write_shop_navigation\n  description: Write access to pages, blogs, articles, and redirects.\n- scope: read_product\n  description: Read access to products and variants.\n- scope: write_product\n  description: Write access to products and variants.\n- scope: read_collection\n  description: Read access to collections and collects.\n- scope: write_collection\n  description:\
  \ Write access to collections and collects.\n- scope: read_comments\n  description: Read access to comments.\n- scope: write_comments\n  description: Write access to comments.\n- scope: read_payment_info\n  description: Read access to payments apps.\n- scope: write_payment_info\n  description: Write access to payments apps.\n- scope: read_order\n  description: Read access to orders.\n- scope: write_order\n  description: Write access to orders.\n- scope: read_customer\n  description: Read access to customers.\n- scope: write_customer\n  description: Write access to customers.\n- scope: read_price_rules\n  description: Read access to price rules — discount codes, coupons, flash sales, rebates, popups, and sales pops.\n- scope: write_price_rules\n  description: Write access to price rules — discount codes, coupons, flash sales, rebates, popups, and sales pops.\n- scope: read_gift_cards\n  description: Read access to gift cards.\n- scope: write_gift_cards\n  description: Write access to gift\
  \ cards.\n- scope: read_app_proxy\n  description: Read access to app proxies.\n- scope: write_app_proxy\n  description: Write access to app proxies.\n- scope: read_data\n  description: Read access to data.\n- scope: write_data\n  description: Write access to data.\n- scope: read_script_tags\n  description: Read access to script tags.\n- scope: write_script_tags\n  description: Write access to script tags.\n- scope: read_finance\n  description: Read access to Shoplazza payment information.\n- scope: write_finance\n  description: Write access to Shoplazza payment information.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/scopes/shoplazza-scopes.yml
summary_line: 29 scopes
tags:
- Company
- Enterprise
- E-Commerce
- Online Store
- Retail
- Payments
- Webhooks
- REST API
- Apps
- Developer Platform
token_urls: []
---
