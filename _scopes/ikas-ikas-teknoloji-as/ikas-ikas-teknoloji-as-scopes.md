---
authorization_urls: []
description: ''
docs: https://ikas.dev/docs/intro
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ikas Ikas Teknoloji As Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ikas, IKAS Teknoloji AS publishes 10 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ikas, IKAS Teknoloji AS API on a user''s behalf.


  Tokens are issued from https://{store_name}.myikas.com/api/admin/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ikas, IKAS Teknoloji AS
provider_slug: ikas-ikas-teknoloji-as
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{store_name}.myikas.com/api/admin/oauth/token
  - flow: authorizationCode
  name: OAuth2
scope_count: 10
scope_names:
- read_products
- write_products
- read_orders
- write_orders
- read_customers
- write_customers
- read_campaigns
- write_campaigns
- read_inventories
- write_inventories
scopes:
- description: View products
  flows:
  - clientCredentials
  - authorizationCode
  scope: read_products
- description: Manage products
  flows:
  - clientCredentials
  - authorizationCode
  scope: write_products
- description: View orders
  flows:
  - clientCredentials
  - authorizationCode
  scope: read_orders
- description: Manage orders
  flows:
  - clientCredentials
  - authorizationCode
  scope: write_orders
- description: View customers
  flows:
  - clientCredentials
  - authorizationCode
  scope: read_customers
- description: Manage customers
  flows:
  - clientCredentials
  - authorizationCode
  scope: write_customers
- description: View campaigns
  flows:
  - clientCredentials
  - authorizationCode
  scope: read_campaigns
- description: Manage campaigns
  flows:
  - clientCredentials
  - authorizationCode
  scope: write_campaigns
- description: View inventory levels
  flows:
  - clientCredentials
  - authorizationCode
  scope: read_inventories
- description: Manage inventory levels
  flows:
  - clientCredentials
  - authorizationCode
  scope: write_inventories
slug: ikas-ikas-teknoloji-as-scopes
source_filename: ikas-ikas-teknoloji-as-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://ikas.dev/docs/intro\ndocs: https://ikas.dev/docs/intro\nschemes:\n- name: OAuth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{store_name}.myikas.com/api/admin/oauth/token\n  - flow: authorizationCode\nscopes:\n- scope: read_products\n  description: View products\n  flows: [clientCredentials, authorizationCode]\n- scope: write_products\n  description: Manage products\n  flows: [clientCredentials, authorizationCode]\n- scope: read_orders\n  description: View orders\n  flows: [clientCredentials, authorizationCode]\n- scope: write_orders\n  description: Manage orders\n  flows: [clientCredentials, authorizationCode]\n- scope: read_customers\n  description: View customers\n  flows: [clientCredentials, authorizationCode]\n- scope: write_customers\n  description: Manage customers\n  flows: [clientCredentials, authorizationCode]\n- scope: read_campaigns\n  description: View campaigns\n  flows: [clientCredentials,\
  \ authorizationCode]\n- scope: write_campaigns\n  description: Manage campaigns\n  flows: [clientCredentials, authorizationCode]\n- scope: read_inventories\n  description: View inventory levels\n  flows: [clientCredentials, authorizationCode]\n- scope: write_inventories\n  description: Manage inventory levels\n  flows: [clientCredentials, authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikas-ikas-teknoloji-as/refs/heads/main/scopes/ikas-ikas-teknoloji-as-scopes.yml
summary_line: 10 scopes · clientCredentials/authorizationCode
tags:
- Company
- E-commerce
- Retail
- Storefront
- Orders
- Products
- Inventory
- GraphQL
- Webhooks
- OAuth
- SDK
- MCP
token_urls:
- https://{store_name}.myikas.com/api/admin/oauth/token
---
