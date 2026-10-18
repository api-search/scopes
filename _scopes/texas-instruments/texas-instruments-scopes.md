---
api_specs:
- filename: texas-instruments-financial-api-openapi.yml
  format: yaml
  label: Texas Instruments Financial API
  slug: texas-instruments-financial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-financial-api-openapi.yml
- filename: texas-instruments-orders-api-openapi.yml
  format: yaml
  label: Texas Instruments Orders API
  slug: texas-instruments-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-orders-api-openapi.yml
- filename: texas-instruments-product-information-api-openapi.yml
  format: yaml
  label: Texas Instruments Product Information API
  slug: texas-instruments-product-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-product-information-api-openapi.yml
- filename: texas-instruments-product-information-orchestrated-api-openapi.yml
  format: yaml
  label: Texas Instruments Product Information Orchestrated API
  slug: texas-instruments-product-information-orchestrated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-product-information-orchestrated-api-openapi.yml
- filename: texas-instruments-products-api-openapi.yml
  format: yaml
  label: Texas Instruments Products API
  slug: texas-instruments-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-products-api-openapi.yml
- filename: texas-instruments-shipments-api-openapi.yml
  format: yaml
  label: Texas Instruments Shipments API
  slug: texas-instruments-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-shipments-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Texas Instruments Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Texas Instruments uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://transact.ti.com/v1/oauth/accesstoken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Texas Instruments
provider_slug: texas-instruments
schemes:
- description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret from your myTI company account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken
  name: OAuth2
  source: openapi/texas-instruments-financial-api-openapi.yml
- description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret from your myTI company account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken
  name: OAuth2
  source: openapi/texas-instruments-orders-api-openapi.yml
- description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret from your myTI developer account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken
  name: OAuth2
  source: openapi/texas-instruments-product-information-api-openapi.yml
- description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret from your myTI developer account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken
  name: OAuth2
  source: openapi/texas-instruments-product-information-orchestrated-api-openapi.yml
- description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret from your myTI company account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken
  name: OAuth2
  source: openapi/texas-instruments-products-api-openapi.yml
- description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret from your myTI company account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken
  name: OAuth2
  source: openapi/texas-instruments-shipments-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: texas-instruments-scopes
source_filename: texas-instruments-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/texas-instruments-financial-api-openapi.yml, openapi/texas-instruments-orders-api-openapi.yml,\n  openapi/texas-instruments-product-information-api-openapi.yml, openapi/texas-instruments-product-information-orchestrated-api-openapi.yml,\n  openapi/texas-instruments-products-api-openapi.yml, openapi/texas-instruments-shipments-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/texas-instruments-financial-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken\n  description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret\n    from your myTI company account.\n- name: OAuth2\n  source: openapi/texas-instruments-orders-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken\n  description: OAuth 2.0 client credentials flow. Obtain access token using client_id\
  \ and client_secret\n    from your myTI company account.\n- name: OAuth2\n  source: openapi/texas-instruments-product-information-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken\n  description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret\n    from your myTI developer account.\n- name: OAuth2\n  source: openapi/texas-instruments-product-information-orchestrated-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken\n  description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret\n    from your myTI developer account.\n- name: OAuth2\n  source: openapi/texas-instruments-products-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken\n  description: OAuth 2.0 client credentials flow. Obtain access token using client_id and\
  \ client_secret\n    from your myTI company account.\n- name: OAuth2\n  source: openapi/texas-instruments-shipments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken\n  description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret\n    from your myTI company account.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/scopes/texas-instruments-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Electronics
- Ordering
- Semiconductors
- Supply Chain
- Fortune 500
token_bound: false
token_urls:
- https://transact.ti.com/v1/oauth/accesstoken
---
