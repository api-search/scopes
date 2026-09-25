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
method: derived
name: Api Dash Scopes
name_suffix: OAuth Scopes
note: ''
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
  source: openapi/api-dash-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: api-dash-scopes
source_filename: api-dash-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/api-dash-openapi.yml\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/api-dash-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /login\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/scopes/api-dash-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Client
- Open Source
- Flutter
- Desktop
- Mobile
token_urls:
- /login
---
