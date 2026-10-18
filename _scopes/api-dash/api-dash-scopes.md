---
api_specs:
- filename: api-dash-api-dash-apis-api-openapi.yml
  format: yaml
  label: API Dash API Dash APIs API
  slug: api-dash-api-dash-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-api-dash-apis-api-openapi.yml
- filename: api-dash-case-conversion-api-openapi.yml
  format: yaml
  label: API Dash Case Conversion API
  slug: api-dash-case-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-case-conversion-api-openapi.yml
- filename: api-dash-country-data-api-openapi.yml
  format: yaml
  label: API Dash Country Data API
  slug: api-dash-country-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-country-data-api-openapi.yml
- filename: api-dash-humanize-api-openapi.yml
  format: yaml
  label: API Dash Humanize API
  slug: api-dash-humanize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-humanize-api-openapi.yml
- filename: api-dash-i-o-api-openapi.yml
  format: yaml
  label: API Dash I/O API
  slug: api-dash-i-o-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-i-o-api-openapi.yml
- filename: api-dash-sse-api-openapi.yml
  format: yaml
  label: API Dash SSE API
  slug: api-dash-sse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-sse-api-openapi.yml
- filename: api-dash-text-conversion-api-openapi.yml
  format: yaml
  label: API Dash Text Conversion API
  slug: api-dash-text-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-text-conversion-api-openapi.yml
- filename: api-dash-user-authentication-api-openapi.yml
  format: yaml
  label: API Dash User Authentication API
  slug: api-dash-user-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-user-authentication-api-openapi.yml
- filename: api-dash-user-data-api-openapi.yml
  format: yaml
  label: API Dash User Data API
  slug: api-dash-user-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-user-data-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Api Dash Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'API Dash uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: API Dash
provider_slug: api-dash
schemes:
- flows:
  - flow: password
    tokenUrl: /login
  name: OAuth2PasswordBearer
  source: openapi/api-dash-api-dash-apis-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /login
  name: OAuth2PasswordBearer
  source: openapi/api-dash-case-conversion-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /login
  name: OAuth2PasswordBearer
  source: openapi/api-dash-country-data-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /login
  name: OAuth2PasswordBearer
  source: openapi/api-dash-humanize-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /login
  name: OAuth2PasswordBearer
  source: openapi/api-dash-i-o-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /login
  name: OAuth2PasswordBearer
  source: openapi/api-dash-sse-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /login
  name: OAuth2PasswordBearer
  source: openapi/api-dash-text-conversion-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /login
  name: OAuth2PasswordBearer
  source: openapi/api-dash-user-authentication-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /login
  name: OAuth2PasswordBearer
  source: openapi/api-dash-user-data-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: api-dash-scopes
source_filename: api-dash-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/api-dash-api-dash-apis-api-openapi.yml, openapi/api-dash-case-conversion-api-openapi.yml,\n  openapi/api-dash-country-data-api-openapi.yml, openapi/api-dash-humanize-api-openapi.yml,\n  openapi/api-dash-i-o-api-openapi.yml, openapi/api-dash-sse-api-openapi.yml, openapi/api-dash-text-conversion-api-openapi.yml,\n  openapi/api-dash-user-authentication-api-openapi.yml, openapi/api-dash-user-data-api-openapi.yml\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-api-dash-apis-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /login\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-case-conversion-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /login\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-country-data-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /login\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-humanize-api-openapi.yml\n  flows:\n\
  \  - flow: password\n    tokenUrl: /login\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-i-o-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /login\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-sse-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /login\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-text-conversion-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /login\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-user-authentication-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /login\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-user-data-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /login\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/scopes/api-dash-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Client
- Open Source
- Flutter
- Desktop
- Mobile
token_bound: false
token_urls:
- /login
---
