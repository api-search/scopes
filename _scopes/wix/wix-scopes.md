---
api_specs:
- filename: wix-asyncapi.yml
  format: yaml
  label: Wix Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/asyncapi/wix-asyncapi.yml
- filename: wix-cart-api-openapi.yml
  format: yaml
  label: Wix Cart API
  slug: wix-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-cart-api-openapi.yml
- filename: wix-checkout-api-openapi.yml
  format: yaml
  label: Wix Checkout API
  slug: wix-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-checkout-api-openapi.yml
- filename: wix-orders-api-openapi.yml
  format: yaml
  label: Wix Orders API
  slug: wix-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-orders-api-openapi.yml
- filename: wix-products-api-openapi.yml
  format: yaml
  label: Wix Products API
  slug: wix-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-products-api-openapi.yml
- filename: wix-oauth-api-openapi.yml
  format: yaml
  label: Wix O Auth API
  slug: wix-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-oauth-api-openapi.yml
authorization_urls:
- https://www.wix.com/installer/install
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Wix Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Wix uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://www.wixapis.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wix
provider_slug: wix
schemes:
- description: OAuth 2.0 for Wix third-party apps
  flows:
  - authorizationUrl: https://www.wix.com/installer/install
    flow: authorizationCode
    tokenUrl: https://www.wixapis.com/oauth2/token
  name: oauth2
  source: openapi/wix-cart-api-openapi.yml
- description: OAuth 2.0 for Wix third-party apps
  flows:
  - authorizationUrl: https://www.wix.com/installer/install
    flow: authorizationCode
    tokenUrl: https://www.wixapis.com/oauth2/token
  name: oauth2
  source: openapi/wix-checkout-api-openapi.yml
- description: OAuth 2.0 for Wix third-party apps
  flows:
  - authorizationUrl: https://www.wix.com/installer/install
    flow: authorizationCode
    tokenUrl: https://www.wixapis.com/oauth2/token
  name: oauth2
  source: openapi/wix-oauth-api-openapi.yml
- description: OAuth 2.0 for Wix third-party apps
  flows:
  - authorizationUrl: https://www.wix.com/installer/install
    flow: authorizationCode
    tokenUrl: https://www.wixapis.com/oauth2/token
  name: oauth2
  source: openapi/wix-orders-api-openapi.yml
- description: OAuth 2.0 for Wix third-party apps
  flows:
  - authorizationUrl: https://www.wix.com/installer/install
    flow: authorizationCode
    tokenUrl: https://www.wixapis.com/oauth2/token
  name: oauth2
  source: openapi/wix-products-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: wix-scopes
source_filename: wix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/wix-cart-api-openapi.yml, openapi/wix-checkout-api-openapi.yml, openapi/wix-oauth-api-openapi.yml,\n  openapi/wix-orders-api-openapi.yml, openapi/wix-products-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/wix-cart-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wix.com/installer/install\n    tokenUrl: https://www.wixapis.com/oauth2/token\n  description: OAuth 2.0 for Wix third-party apps\n- name: oauth2\n  source: openapi/wix-checkout-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wix.com/installer/install\n    tokenUrl: https://www.wixapis.com/oauth2/token\n  description: OAuth 2.0 for Wix third-party apps\n- name: oauth2\n  source: openapi/wix-oauth-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wix.com/installer/install\n    tokenUrl: https://www.wixapis.com/oauth2/token\n  description:\
  \ OAuth 2.0 for Wix third-party apps\n- name: oauth2\n  source: openapi/wix-orders-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wix.com/installer/install\n    tokenUrl: https://www.wixapis.com/oauth2/token\n  description: OAuth 2.0 for Wix third-party apps\n- name: oauth2\n  source: openapi/wix-products-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wix.com/installer/install\n    tokenUrl: https://www.wixapis.com/oauth2/token\n  description: OAuth 2.0 for Wix third-party apps\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/scopes/wix-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CMS
- E-Commerce
- Headless
- Website Builder
token_bound: false
token_urls:
- https://www.wixapis.com/oauth2/token
---
