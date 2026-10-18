---
api_specs:
- filename: groww-authentication-api-openapi.yml
  format: yaml
  label: Groww Authentication API
  slug: groww-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-authentication-api-openapi.yml
- filename: groww-historical-data-api-openapi.yml
  format: yaml
  label: Groww Historical Data API
  slug: groww-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-historical-data-api-openapi.yml
- filename: groww-live-data-api-openapi.yml
  format: yaml
  label: Groww Live Data API
  slug: groww-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-live-data-api-openapi.yml
- filename: groww-margin-api-openapi.yml
  format: yaml
  label: Groww Margin API
  slug: groww-margin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-margin-api-openapi.yml
- filename: groww-orders-api-openapi.yml
  format: yaml
  label: Groww Orders API
  slug: groww-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-orders-api-openapi.yml
- filename: groww-portfolio-api-openapi.yml
  format: yaml
  label: Groww Portfolio API
  slug: groww-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-portfolio-api-openapi.yml
authorization_urls:
- https://groww.in/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Groww Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
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
  source: openapi/groww-authentication-api-openapi.yml
- description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://groww.in/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.groww.in/oauth2/v1/token
  name: oauth2
  source: openapi/groww-historical-data-api-openapi.yml
- description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://groww.in/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.groww.in/oauth2/v1/token
  name: oauth2
  source: openapi/groww-live-data-api-openapi.yml
- description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://groww.in/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.groww.in/oauth2/v1/token
  name: oauth2
  source: openapi/groww-margin-api-openapi.yml
- description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://groww.in/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.groww.in/oauth2/v1/token
  name: oauth2
  source: openapi/groww-orders-api-openapi.yml
- description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://groww.in/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.groww.in/oauth2/v1/token
  name: oauth2
  source: openapi/groww-portfolio-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: groww-scopes
source_filename: groww-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/groww-authentication-api-openapi.yml, openapi/groww-historical-data-api-openapi.yml,\n  openapi/groww-live-data-api-openapi.yml, openapi/groww-margin-api-openapi.yml, openapi/groww-orders-api-openapi.yml,\n  openapi/groww-portfolio-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/groww-authentication-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://groww.in/oauth/authorize\n    tokenUrl: https://api.groww.in/oauth2/v1/token\n  description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server\n- name: oauth2\n  source: openapi/groww-historical-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://groww.in/oauth/authorize\n    tokenUrl: https://api.groww.in/oauth2/v1/token\n  description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server\n\
  - name: oauth2\n  source: openapi/groww-live-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://groww.in/oauth/authorize\n    tokenUrl: https://api.groww.in/oauth2/v1/token\n  description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server\n- name: oauth2\n  source: openapi/groww-margin-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://groww.in/oauth/authorize\n    tokenUrl: https://api.groww.in/oauth2/v1/token\n  description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server\n- name: oauth2\n  source: openapi/groww-orders-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://groww.in/oauth/authorize\n    tokenUrl: https://api.groww.in/oauth2/v1/token\n  description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server\n\
  - name: oauth2\n  source: openapi/groww-portfolio-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://groww.in/oauth/authorize\n    tokenUrl: https://api.groww.in/oauth2/v1/token\n  description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
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
token_bound: false
token_urls:
- https://api.groww.in/oauth2/v1/token
---
