---
api_specs:
- filename: depop-selling-openapi-original.yml
  format: yaml
  label: Depop Selling API
  slug: depop-selling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depop/refs/heads/main/openapi/depop-selling-openapi-original.yml
authorization_urls: []
description: ''
docs: https://partnerapi.depop.com/api-docs/concepts/authentication/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Depop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'depop publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the depop API on a user''s behalf.


  Tokens are issued from https://partnerapi.depop.com/api/v1/oauth2/access-token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: depop
provider_slug: depop
schemes:
- flows:
  - flow: authorizationCode
    tokenUrl: https://partnerapi.depop.com/api/v1/oauth2/access-token/
  name: OAuth2
  source: https://partnerapi.depop.com/api-docs/concepts/authentication/
scope_count: 7
scope_names:
- products_read
- products_write
- orders_read
- orders_write
- offers_read
- offers_write
- shop_read
scopes:
- description: Read product information and listings.
  flows:
  - authorizationCode
  scope: products_read
- description: Create, update, or delete products.
  flows:
  - authorizationCode
  scope: products_write
- description: Read order information and order history.
  flows:
  - authorizationCode
  scope: orders_read
- description: Mark orders as shipped or process refunds.
  flows:
  - authorizationCode
  scope: orders_write
- description: Read offer pricing information (auto send / auto negotiate offer price).
  flows:
  - authorizationCode
  scope: offers_read
- description: Set or modify offer prices (auto send / auto negotiate offer price).
  flows:
  - authorizationCode
  scope: offers_write
- description: Read shop information including seller addresses and available shipping providers.
  flows:
  - authorizationCode
  scope: shop_read
slug: depop-scopes
source_filename: depop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/depop-selling-openapi-original.yml\ndocs: https://partnerapi.depop.com/api-docs/concepts/authentication/\nnotes: >-\n  Scopes are documented in the OpenAPI info description and the authentication\n  concept page. The OpenAPI securitySchemes block declares only an http bearer\n  scheme, so scopes are captured here from the documented OAuth 2.0 model. API\n  key tokens implicitly hold all scopes; OAuth tokens are limited to those\n  granted. A 403 with error code insufficient_scope is returned when a required\n  scope is missing.\nschemes:\n- name: OAuth2\n  source: https://partnerapi.depop.com/api-docs/concepts/authentication/\n  flows:\n  - flow: authorizationCode\n    tokenUrl: https://partnerapi.depop.com/api/v1/oauth2/access-token/\nscopes:\n- scope: products_read\n  description: Read product information and listings.\n  flows: [authorizationCode]\n- scope: products_write\n  description: Create, update, or delete\
  \ products.\n  flows: [authorizationCode]\n- scope: orders_read\n  description: Read order information and order history.\n  flows: [authorizationCode]\n- scope: orders_write\n  description: Mark orders as shipped or process refunds.\n  flows: [authorizationCode]\n- scope: offers_read\n  description: Read offer pricing information (auto send / auto negotiate offer price).\n  flows: [authorizationCode]\n- scope: offers_write\n  description: Set or modify offer prices (auto send / auto negotiate offer price).\n  flows: [authorizationCode]\n- scope: shop_read\n  description: Read shop information including seller addresses and available shipping providers.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depop/refs/heads/main/scopes/depop-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Fashion
- Marketplace
- E-commerce
- Resale
- Retail
- Inventory Management
- Orders
- Sustainability
token_urls:
- https://partnerapi.depop.com/api/v1/oauth2/access-token/
---
