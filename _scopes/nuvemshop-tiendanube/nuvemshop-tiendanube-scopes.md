---
api_specs:
- filename: nuvemshop-tiendanube-events-asyncapi.yml
  format: yaml
  label: Nuvemshop Tiendanube API
  slug: nuvemshop-tiendanube-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop-tiendanube/refs/heads/main/asyncapi/nuvemshop-tiendanube-events-asyncapi.yml
authorization_urls:
- https://www.tiendanube.com/apps/{app_id}/authorize
description: ''
docs: https://tiendanube.github.io/api-documentation/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nuvemshop Tiendanube Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nuvemshop Tiendanube publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nuvemshop Tiendanube API on a user''s behalf.


  Tokens are issued from https://www.tiendanube.com/apps/authorize/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nuvemshop Tiendanube
provider_slug: nuvemshop-tiendanube
schemes:
- flows:
  - authorizationUrl: https://www.tiendanube.com/apps/{app_id}/authorize
    flow: authorizationCode
    tokenUrl: https://www.tiendanube.com/apps/authorize/token
  name: OAuth2
scope_count: 12
scope_names:
- read_content
- write_content
- read_products
- write_products
- read_customers
- write_customers
- read_orders
- write_orders
- read_coupons
- write_coupons
- write_scripts
- write_shipping
scopes:
- description: Read access to store content pages.
  flows: []
  scope: read_content
- description: Write access to store content pages (implies read_content).
  flows: []
  scope: write_content
- description: Read access to products, variants, images and categories.
  flows: []
  scope: read_products
- description: Write access to products, variants, images and categories (implies read_products).
  flows: []
  scope: write_products
- description: Read access to customers.
  flows: []
  scope: read_customers
- description: Write access to customers (implies read_customers).
  flows: []
  scope: write_customers
- description: Read access to orders.
  flows: []
  scope: read_orders
- description: Write access to orders (implies read_orders).
  flows: []
  scope: write_orders
- description: Read access to coupons.
  flows: []
  scope: read_coupons
- description: Write access to coupons (implies read_coupons).
  flows: []
  scope: write_coupons
- description: Manage storefront scripts (no separate read scope).
  flows: []
  scope: write_scripts
- description: Manage shipping carriers (no separate read scope).
  flows: []
  scope: write_shipping
slug: nuvemshop-tiendanube-scopes
source_filename: nuvemshop-tiendanube-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://tiendanube.github.io/api-documentation/authentication\ndocs: https://tiendanube.github.io/api-documentation/authentication\nschemes:\n- name: OAuth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.tiendanube.com/apps/{app_id}/authorize\n    tokenUrl: https://www.tiendanube.com/apps/authorize/token\nnotes: >-\n  Requesting any write scope implies the matching read scope. Scopes are granted\n  by the merchant at app authorization time and returned in the token response.\nscopes:\n- scope: read_content\n  description: Read access to store content pages.\n- scope: write_content\n  description: Write access to store content pages (implies read_content).\n- scope: read_products\n  description: Read access to products, variants, images and categories.\n- scope: write_products\n  description: Write access to products, variants, images and categories (implies read_products).\n- scope: read_customers\n\
  \  description: Read access to customers.\n- scope: write_customers\n  description: Write access to customers (implies read_customers).\n- scope: read_orders\n  description: Read access to orders.\n- scope: write_orders\n  description: Write access to orders (implies read_orders).\n- scope: read_coupons\n  description: Read access to coupons.\n- scope: write_coupons\n  description: Write access to coupons (implies read_coupons).\n- scope: write_scripts\n  description: Manage storefront scripts (no separate read scope).\n- scope: write_shipping\n  description: Manage shipping carriers (no separate read scope).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuvemshop-tiendanube/refs/heads/main/scopes/nuvemshop-tiendanube-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Retail
- Online Stores
- Payments
- Shipping
- Webhooks
- OAuth
- Latin America
- Storefront
- Apps Platform
token_urls:
- https://www.tiendanube.com/apps/authorize/token
---
