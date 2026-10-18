---
api_specs:
- filename: ibisworld-business-environment-api-openapi.yml
  format: yaml
  label: IBISWorld Business Environment API
  slug: ibisworld-business-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-business-environment-api-openapi.yml
- filename: ibisworld-classification-api-openapi.yml
  format: yaml
  label: IBISWorld Classification API
  slug: ibisworld-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-classification-api-openapi.yml
- filename: ibisworld-company-api-openapi.yml
  format: yaml
  label: IBISWorld Company API
  slug: ibisworld-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-company-api-openapi.yml
- filename: ibisworld-downloads-api-openapi.yml
  format: yaml
  label: IBISWorld Downloads API
  slug: ibisworld-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-downloads-api-openapi.yml
- filename: ibisworld-industry-api-openapi.yml
  format: yaml
  label: IBISWorld Industry API
  slug: ibisworld-industry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-industry-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Ibisworld Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'IBISWorld uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.ibisworld.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IBISWorld
provider_slug: ibisworld
schemes:
- description: OAuth 2.0 bearer token authentication.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ibisworld.com/oauth/token
  name: OAuth2
  source: openapi/ibisworld-business-environment-api-openapi.yml
- description: OAuth 2.0 bearer token authentication.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ibisworld.com/oauth/token
  name: OAuth2
  source: openapi/ibisworld-classification-api-openapi.yml
- description: OAuth 2.0 bearer token authentication.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ibisworld.com/oauth/token
  name: OAuth2
  source: openapi/ibisworld-company-api-openapi.yml
- description: OAuth 2.0 bearer token authentication.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ibisworld.com/oauth/token
  name: OAuth2
  source: openapi/ibisworld-downloads-api-openapi.yml
- description: OAuth 2.0 bearer token authentication.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ibisworld.com/oauth/token
  name: OAuth2
  source: openapi/ibisworld-industry-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: ibisworld-scopes
source_filename: ibisworld-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/ibisworld-business-environment-api-openapi.yml, openapi/ibisworld-classification-api-openapi.yml,\n  openapi/ibisworld-company-api-openapi.yml, openapi/ibisworld-downloads-api-openapi.yml, openapi/ibisworld-industry-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/ibisworld-business-environment-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ibisworld.com/oauth/token\n  description: OAuth 2.0 bearer token authentication.\n- name: OAuth2\n  source: openapi/ibisworld-classification-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ibisworld.com/oauth/token\n  description: OAuth 2.0 bearer token authentication.\n- name: OAuth2\n  source: openapi/ibisworld-company-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ibisworld.com/oauth/token\n  description: OAuth 2.0 bearer token authentication.\n- name: OAuth2\n  source:\
  \ openapi/ibisworld-downloads-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ibisworld.com/oauth/token\n  description: OAuth 2.0 bearer token authentication.\n- name: OAuth2\n  source: openapi/ibisworld-industry-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ibisworld.com/oauth/token\n  description: OAuth 2.0 bearer token authentication.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/scopes/ibisworld-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Business Intelligence
- Economics
- Industry Data
- Market Research
token_bound: false
token_urls:
- https://api.ibisworld.com/oauth/token
---
