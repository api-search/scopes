---
api_specs:
- filename: alectra-utilities-applicationinformation-api-openapi.yml
  format: yaml
  label: Alectra Utilities Application Information API
  slug: alectra-utilities-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-applicationinformation-api-openapi.yml
- filename: alectra-utilities-authorization-api-openapi.yml
  format: yaml
  label: Alectra Utilities Authorization API
  slug: alectra-utilities-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-authorization-api-openapi.yml
- filename: alectra-utilities-batch-api-openapi.yml
  format: yaml
  label: Alectra Utilities Batch API
  slug: alectra-utilities-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-batch-api-openapi.yml
- filename: alectra-utilities-usagepoint-api-openapi.yml
  format: yaml
  label: Alectra Utilities Usage Point API
  slug: alectra-utilities-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-usagepoint-api-openapi.yml
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
name: Alectra Utilities Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Alectra Utilities uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox.greenbuttonalliance.org:8443/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alectra Utilities
provider_slug: alectra-utilities
schemes:
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/alectra-utilities-applicationinformation-api-openapi.yml
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/alectra-utilities-authorization-api-openapi.yml
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/alectra-utilities-batch-api-openapi.yml
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/alectra-utilities-usagepoint-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: alectra-utilities-scopes
source_filename: alectra-utilities-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/alectra-utilities-applicationinformation-api-openapi.yml, openapi/alectra-utilities-authorization-api-openapi.yml,\n  openapi/alectra-utilities-batch-api-openapi.yml, openapi/alectra-utilities-usagepoint-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/alectra-utilities-applicationinformation-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n- name: oauth2\n  source: openapi/alectra-utilities-authorization-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://sandbox.greenbuttonalliance.org:8443/oauth/token\n- name: oauth2\n  source: openapi/alectra-utilities-batch-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n- name: oauth2\n  source: openapi/alectra-utilities-usagepoint-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/scopes/alectra-utilities-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Ontario
- Green Button
- Smart Metering
- Energy Data
- Grid
- Municipal Utility
- ESPI
token_bound: false
token_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/token
---
