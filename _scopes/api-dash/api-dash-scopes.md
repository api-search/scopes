---
api_specs:
- filename: api-dash-openapi.yml
  format: yaml
  label: API Dash
  slug: api-dash
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-openapi.yml
- filename: api-dash-openapi.yml
  format: yaml
  label: API Dash APIs
  slug: api-dash-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-openapi.yml
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
- Open-Source
- Flutter
- Desktop
- Mobile
token_urls:
- /login
---
