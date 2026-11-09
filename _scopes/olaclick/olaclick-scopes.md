---
api_specs:
- filename: olaclick-openapi-generated.yml
  format: yaml
  label: OlaClick API
  slug: olaclick-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/olaclick/openapi/_ae-authored/olaclick-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Olaclick Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OlaClick publishes 23 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the OlaClick API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OlaClick
provider_slug: olaclick
schemes: []
scope_count: 23
scope_names:
- menu:read
- menu:write
- orders:read
- orders:write
- promotions:read
- promotions:write
- clients:read
- clients:write
- addresses:read
- addresses:write
- reports:read
- webhooks:read
- webhooks:write
- companies:read
- payment-methods:read
- stores:read
- users:read
- fiscal-notes:write
- logistics:write
- cashiers:read
- conections:read
- conections:write
- portfolio:read
scopes:
- description: Read menu categories and products
  flows: []
  scope: menu:read
- description: Create and update products
  flows: []
  scope: menu:write
- description: Read orders
  flows: []
  scope: orders:read
- description: Create orders, update order status, items, payments and discounts, and cancel orders
  flows: []
  scope: orders:write
- description: Read active promotions and coupons
  flows: []
  scope: promotions:read
- description: Create, update, and delete promotions (coupons)
  flows: []
  scope: promotions:write
- description: Read client list with filters and pagination
  flows: []
  scope: clients:read
- description: Create and update clients
  flows: []
  scope: clients:write
- description: List client delivery addresses
  flows: []
  scope: addresses:read
- description: Create, update, and delete client delivery addresses
  flows: []
  scope: addresses:write
- description: Read reports
  flows: []
  scope: reports:read
- description: List and view webhook configurations
  flows: []
  scope: webhooks:read
- description: Create, update, and delete webhooks
  flows: []
  scope: webhooks:write
- description: Read company information
  flows: []
  scope: companies:read
- description: Read the company payment methods
  flows: []
  scope: payment-methods:read
- description: Read food-app store open/closed status
  flows: []
  scope: stores:read
- description: Read the company user list with role filter and pagination
  flows: []
  scope: users:read
- description: Create and update fiscal note invoices
  flows: []
  scope: fiscal-notes:write
- description: Assign riders and update delivery status
  flows: []
  scope: logistics:write
- description: Read cash register openings and closings
  flows: []
  scope: cashiers:read
- description: List connector conections
  flows: []
  scope: conections:read
- description: Update conection status
  flows: []
  scope: conections:write
- description: Read the connector portfolio of companies on the qualifying plan
  flows: []
  scope: portfolio:read
slug: olaclick-scopes
source_filename: olaclick-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://developers.olaclick.app/docs/authentication/scopes\nscopes:\n  - name: menu:read\n    description: Read menu categories and products\n  - name: menu:write\n    description: Create and update products\n  - name: orders:read\n    description: Read orders\n  - name: orders:write\n    description: Create orders, update order status, items, payments and discounts, and cancel orders\n  - name: promotions:read\n    description: Read active promotions and coupons\n  - name: promotions:write\n    description: Create, update, and delete promotions (coupons)\n  - name: clients:read\n    description: Read client list with filters and pagination\n  - name: clients:write\n    description: Create and update clients\n  - name: addresses:read\n    description: List client delivery addresses\n  - name: addresses:write\n    description: Create, update, and delete client delivery addresses\n  - name: reports:read\n    description: Read\
  \ reports\n  - name: webhooks:read\n    description: List and view webhook configurations\n  - name: webhooks:write\n    description: Create, update, and delete webhooks\n  - name: companies:read\n    description: Read company information\n  - name: payment-methods:read\n    description: Read the company payment methods\n  - name: stores:read\n    description: Read food-app store open/closed status\n  - name: users:read\n    description: Read the company user list with role filter and pagination\n  - name: fiscal-notes:write\n    description: Create and update fiscal note invoices\n  - name: logistics:write\n    description: Assign riders and update delivery status\n  - name: cashiers:read\n    description: Read cash register openings and closings\n  - name: conections:read\n    description: List connector conections\n  - name: conections:write\n    description: Update conection status\n  - name: portfolio:read\n    description: Read the connector portfolio of companies on the qualifying\
  \ plan\n"
source_yaml_url: https://artifacts.apis.io/olaclick/scopes/olaclick-scopes.yml
summary_line: 23 scopes
tags:
- Restaurant
- Point-of-Sale
- Artificial Intelligence
- Software-as-a-Service
- Delivery
token_bound: false
token_urls: []
---
