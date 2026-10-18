---
api_specs:
- filename: hydro-ottawa-applicationinformation-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Application Information API
  slug: hydro-ottawa-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-applicationinformation-api-openapi.yml
- filename: hydro-ottawa-authorization-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Authorization API
  slug: hydro-ottawa-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-authorization-api-openapi.yml
- filename: hydro-ottawa-batch-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Batch API
  slug: hydro-ottawa-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-batch-api-openapi.yml
- filename: hydro-ottawa-usagepoint-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Usage Point API
  slug: hydro-ottawa-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-usagepoint-api-openapi.yml
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
name: Hydro Ottawa Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Hydro Ottawa uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox.greenbuttonalliance.org:8443/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hydro Ottawa
provider_slug: hydro-ottawa
schemes:
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/hydro-ottawa-applicationinformation-api-openapi.yml
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/hydro-ottawa-authorization-api-openapi.yml
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/hydro-ottawa-batch-api-openapi.yml
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/hydro-ottawa-usagepoint-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: hydro-ottawa-scopes
source_filename: hydro-ottawa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/hydro-ottawa-applicationinformation-api-openapi.yml, openapi/hydro-ottawa-authorization-api-openapi.yml,\n  openapi/hydro-ottawa-batch-api-openapi.yml, openapi/hydro-ottawa-usagepoint-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/hydro-ottawa-applicationinformation-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n- name: oauth2\n  source: openapi/hydro-ottawa-authorization-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n\
  - name: oauth2\n  source: openapi/hydro-ottawa-batch-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n- name: oauth2\n  source: openapi/hydro-ottawa-usagepoint-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/scopes/hydro-ottawa-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Canada
- Ontario
- Utilities
- Electricity
- Electricity Distribution
- Smart Metering
- Green Button
- ESPI
- Municipal Utility
- Renewables
- Hydroelectric
- Solar
- Demand Response
- Grid
token_bound: false
token_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/token
---
