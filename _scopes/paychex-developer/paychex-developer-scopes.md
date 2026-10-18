---
api_specs:
- filename: paychex-developer-companies-api-openapi.yml
  format: yaml
  label: Paychex Companies API
  slug: paychex-developer-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-developer-companies-api-openapi.yml
- filename: paychex-developer-time-entries-api-openapi.yml
  format: yaml
  label: Paychex Time Entries API
  slug: paychex-developer-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-developer-time-entries-api-openapi.yml
- filename: paychex-developer-workers-api-openapi.yml
  format: yaml
  label: Paychex Workers API
  slug: paychex-developer-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-developer-workers-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Paychex Developer Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Paychex uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.paychex.com/auth/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paychex
provider_slug: paychex-developer
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.paychex.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  source: openapi/paychex-developer-companies-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.paychex.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  source: openapi/paychex-developer-time-entries-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.paychex.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  source: openapi/paychex-developer-workers-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: paychex-developer-scopes
source_filename: paychex-developer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/paychex-developer-companies-api-openapi.yml, openapi/paychex-developer-time-entries-api-openapi.yml,\n  openapi/paychex-developer-workers-api-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/paychex-developer-companies-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paychex.com/auth/oauth/v2/token\n- name: oauth2ClientCredentials\n  source: openapi/paychex-developer-time-entries-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paychex.com/auth/oauth/v2/token\n- name: oauth2ClientCredentials\n  source: openapi/paychex-developer-workers-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paychex.com/auth/oauth/v2/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/scopes/paychex-developer-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Benefits
- HCM
- Human Resources
- Paychex Flex
- Payroll
- Time and Attendance
- Workforce
- Fortune 1000
- Employee Benefits
token_bound: false
token_urls:
- https://api.paychex.com/auth/oauth/v2/token
---
