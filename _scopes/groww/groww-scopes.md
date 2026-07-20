---
api_specs:
- filename: groww-trade-api-openapi.yml
  format: yaml
  label: Groww Trading API
  slug: groww-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-trade-api-openapi.yml
authorization_urls:
- https://groww.in/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Groww Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Groww uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.groww.in/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Groww
provider_slug: groww
schemes:
- description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://groww.in/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.groww.in/oauth2/v1/token
  name: oauth2
  source: openapi/groww-trade-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: groww-scopes
source_filename: groww-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/groww-trade-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/groww-trade-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://groww.in/oauth/authorize\n    tokenUrl: https://api.groww.in/oauth2/v1/token\n  description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/scopes/groww-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Fintech
- Trading
- Investing
- Stock Broking
- Market Data
- Algorithmic Trading
- India
token_urls:
- https://api.groww.in/oauth2/v1/token
---
