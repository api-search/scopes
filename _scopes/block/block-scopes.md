---
authorization_urls:
- https://connect.squareup.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Block Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Block publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Block API on a user''s behalf.


  Tokens are issued from https://connect.squareup.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Block
provider_slug: block
schemes:
- flows:
  - authorizationUrl: https://connect.squareup.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://connect.squareup.com/oauth2/token
  name: OAuth2
  source: openapi/block-square-api-openapi.yaml
scope_count: 6
scope_names:
- CUSTOMERS_READ
- CUSTOMERS_WRITE
- ORDERS_READ
- ORDERS_WRITE
- PAYMENTS_READ
- PAYMENTS_WRITE
scopes:
- description: Read customers
  flows:
  - authorizationCode
  scope: CUSTOMERS_READ
- description: Write customers
  flows:
  - authorizationCode
  scope: CUSTOMERS_WRITE
- description: Read orders
  flows:
  - authorizationCode
  scope: ORDERS_READ
- description: Write orders
  flows:
  - authorizationCode
  scope: ORDERS_WRITE
- description: Read payments
  flows:
  - authorizationCode
  scope: PAYMENTS_READ
- description: Write payments
  flows:
  - authorizationCode
  scope: PAYMENTS_WRITE
slug: block-scopes
source_filename: block-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/block-square-api-openapi.yaml\nschemes:\n- name: OAuth2\n  source: openapi/block-square-api-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://connect.squareup.com/oauth2/authorize\n    tokenUrl: https://connect.squareup.com/oauth2/token\nscopes:\n- scope: CUSTOMERS_READ\n  description: Read customers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/block-square-api-openapi.yaml\n- scope: CUSTOMERS_WRITE\n  description: Write customers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/block-square-api-openapi.yaml\n- scope: ORDERS_READ\n  description: Read orders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/block-square-api-openapi.yaml\n- scope: ORDERS_WRITE\n  description: Write orders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/block-square-api-openapi.yaml\n- scope: PAYMENTS_READ\n  description: Read payments\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/block-square-api-openapi.yaml\n- scope: PAYMENTS_WRITE\n  description: Write payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/block-square-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/block/refs/heads/main/scopes/block-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
token_urls:
- https://connect.squareup.com/oauth2/token
---
