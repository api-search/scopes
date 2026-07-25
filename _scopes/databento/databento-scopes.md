---
api_specs:
- filename: databento-timeseries-api-openapi.yml
  format: yaml
  label: Databento Historical Timeseries API
  slug: databento-historical-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-timeseries-api-openapi.yml
- filename: databento-metadata-api-openapi.yml
  format: yaml
  label: Databento Metadata API
  slug: databento-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-metadata-api-openapi.yml
- filename: databento-symbology-api-openapi.yml
  format: yaml
  label: Databento Symbology API
  slug: databento-symbology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-symbology-api-openapi.yml
- filename: databento-batch-api-openapi.yml
  format: yaml
  label: Databento Batch API
  slug: databento-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-batch-api-openapi.yml
- filename: databento-reference-api-openapi.yml
  format: yaml
  label: Databento Reference API
  slug: databento-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-reference-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Databento Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Databento uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /v0/auth/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Databento
provider_slug: databento
schemes:
- flows:
  - flow: password
    tokenUrl: /v0/auth/login
  name: OAuth2PasswordBearerWithCookie
  source: openapi/databento-platform-openapi-official.json
scope_count: 0
scope_names: []
scopes: []
slug: databento-scopes
source_filename: databento-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: derived\nsource: openapi/databento-platform-openapi-official.json\nschemes:\n- name: OAuth2PasswordBearerWithCookie\n  source: openapi/databento-platform-openapi-official.json\n  flows:\n  - flow: password\n    tokenUrl: /v0/auth/login\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/scopes/databento-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Market Data
- Financial Data
- Reference Data
- Historical Market Data
- Trading
token_urls:
- /v0/auth/login
---
