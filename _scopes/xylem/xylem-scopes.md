---
api_specs:
- filename: xylem-docview-api-openapi.yml
  format: yaml
  label: Xylem Doc View API
  slug: xylem-docview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-docview-api-openapi.yml
- filename: xylem-infor-api-openapi.yml
  format: yaml
  label: Xylem Infor API
  slug: xylem-infor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-infor-api-openapi.yml
- filename: xylem-mes-api-openapi.yml
  format: yaml
  label: Xylem MES API
  slug: xylem-mes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-mes-api-openapi.yml
- filename: xylem-mes-v2-api-openapi.yml
  format: yaml
  label: Xylem MES V2 API
  slug: xylem-mes-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-mes-v2-api-openapi.yml
- filename: xylem-nameplate-api-openapi.yml
  format: yaml
  label: Xylem Name Plate API
  slug: xylem-nameplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-nameplate-api-openapi.yml
- filename: xylem-serialcard-api-openapi.yml
  format: yaml
  label: Xylem Serial Card API
  slug: xylem-serialcard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-serialcard-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Xylem Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Xylem uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xylem
provider_slug: xylem
schemes:
- flows:
  - flow: password
    tokenUrl: /token
  name: Apis Manager
  source: openapi/xylem-apis-manager-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: xylem-scopes
source_filename: xylem-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: none\nsource: openapi/xylem-apis-manager-openapi.yml\nschemes:\n- name: Apis Manager\n  source: openapi/xylem-apis-manager-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/scopes/xylem-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fortune 1000
- Water
- Water Technology
- Utilities
- Smart Metering
- Industrial IoT
- Water Quality
- Wastewater
- Manufacturing
token_bound: false
token_urls:
- /token
---
