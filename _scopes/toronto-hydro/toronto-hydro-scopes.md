---
api_specs:
- filename: toronto-hydro-applicationinformation-api-openapi.yml
  format: yaml
  label: Toronto Hydro Application Information API
  slug: toronto-hydro-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-applicationinformation-api-openapi.yml
- filename: toronto-hydro-authorization-api-openapi.yml
  format: yaml
  label: Toronto Hydro Authorization API
  slug: toronto-hydro-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-authorization-api-openapi.yml
- filename: toronto-hydro-batch-api-openapi.yml
  format: yaml
  label: Toronto Hydro Batch API
  slug: toronto-hydro-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-batch-api-openapi.yml
- filename: toronto-hydro-usagepoint-api-openapi.yml
  format: yaml
  label: Toronto Hydro Usage Point API
  slug: toronto-hydro-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-usagepoint-api-openapi.yml
authorization_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Toronto Hydro Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Toronto Hydro uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox.greenbuttonalliance.org:8443/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Toronto Hydro
provider_slug: toronto-hydro
schemes:
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/toronto-hydro-applicationinformation-api-openapi.yml
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/toronto-hydro-authorization-api-openapi.yml
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/toronto-hydro-batch-api-openapi.yml
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/toronto-hydro-usagepoint-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: toronto-hydro-scopes
source_filename: toronto-hydro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/toronto-hydro-applicationinformation-api-openapi.yml, openapi/toronto-hydro-authorization-api-openapi.yml,\n  openapi/toronto-hydro-batch-api-openapi.yml, openapi/toronto-hydro-usagepoint-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/toronto-hydro-applicationinformation-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n- name: oauth2\n  source: openapi/toronto-hydro-authorization-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n\
  - name: oauth2\n  source: openapi/toronto-hydro-batch-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n- name: oauth2\n  source: openapi/toronto-hydro-usagepoint-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/scopes/toronto-hydro-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Smart Metering
- Green Button
- Grid
- Ontario
- Consumer Data
- Electricity Distribution
token_bound: false
token_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/token
---
