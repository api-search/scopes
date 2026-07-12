---
authorization_urls:
- https://accounts.salla.sa/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Salla Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salla publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salla API on a user''s behalf.


  Tokens are issued from https://accounts.salla.sa/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salla
provider_slug: salla
schemes:
- flows:
  - authorizationUrl: https://accounts.salla.sa/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.salla.sa/oauth2/token
  name: OAuth2
  source: openapi/salla-merchant-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.salla.sa/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.salla.sa/oauth2/token
  name: OAuth2
  source: openapi/salla-shipping-fulfillment-api-openapi.yml
scope_count: 11
scope_names:
- customers.read
- customers.read_write
- offline_access
- orders.read
- orders.read_write
- products.read
- products.read_write
- settings.read
- shipments.read
- shipments.read_write
- webhooks.read_write
scopes:
- description: Read customers.
  flows:
  - authorizationCode
  scope: customers.read
- description: Read and write customers.
  flows:
  - authorizationCode
  scope: customers.read_write
- description: Required to receive a refresh token.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read orders.
  flows:
  - authorizationCode
  scope: orders.read
- description: Read and write orders.
  flows:
  - authorizationCode
  scope: orders.read_write
- description: Read products.
  flows:
  - authorizationCode
  scope: products.read
- description: Read and write products.
  flows:
  - authorizationCode
  scope: products.read_write
- description: Read store settings.
  flows:
  - authorizationCode
  scope: settings.read
- description: Read shipments.
  flows:
  - authorizationCode
  scope: shipments.read
- description: Read and write shipments.
  flows:
  - authorizationCode
  scope: shipments.read_write
- description: Manage webhook subscriptions.
  flows:
  - authorizationCode
  scope: webhooks.read_write
slug: salla-scopes
source_filename: salla-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salla-merchant-api-openapi.yml, openapi/salla-shipping-fulfillment-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/salla-merchant-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.salla.sa/oauth2/auth\n    tokenUrl: https://accounts.salla.sa/oauth2/token\n- name: OAuth2\n  source: openapi/salla-shipping-fulfillment-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.salla.sa/oauth2/auth\n    tokenUrl: https://accounts.salla.sa/oauth2/token\nscopes:\n- scope: customers.read\n  description: Read customers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n- scope: customers.read_write\n  description: Read and write customers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n- scope: offline_access\n  description: Required to receive a refresh\
  \ token.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n  - openapi/salla-shipping-fulfillment-api-openapi.yml\n- scope: orders.read\n  description: Read orders.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n- scope: orders.read_write\n  description: Read and write orders.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n- scope: products.read\n  description: Read products.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n- scope: products.read_write\n  description: Read and write products.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n- scope: settings.read\n  description: Read store settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n- scope: shipments.read\n  description: Read shipments.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/salla-shipping-fulfillment-api-openapi.yml\n- scope: shipments.read_write\n  description: Read and write shipments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-shipping-fulfillment-api-openapi.yml\n- scope: webhooks.read_write\n  description: Manage webhook subscriptions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salla-merchant-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salla/refs/heads/main/scopes/salla-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Arabic
- E-Commerce
- GCC
- Headless Commerce
- Merchant
- MENA
- Online Stores
- Retail
- Saudi Arabia
- SMB
- Storefront
token_urls:
- https://accounts.salla.sa/oauth2/token
---
