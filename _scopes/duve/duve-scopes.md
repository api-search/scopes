---
api_specs:
- filename: duve-openapi-generated.yml
  format: yaml
  label: Duve API
  slug: duve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duve/refs/heads/main/openapi/_ae-authored/duve-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Duve Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Duve uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox.duve.com/api/openapi/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Duve
provider_slug: duve
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.duve.com/api/openapi/v1/oauth2/token
  name: client_credentials
  source: openapi/duve-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: duve-scopes
source_filename: duve-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: none\nsource: openapi/duve-openapi-generated.yml\nschemes:\n- name: client_credentials\n  source: openapi/duve-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.duve.com/api/openapi/v1/oauth2/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duve/refs/heads/main/scopes/duve-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Hospitality
- GuestExperience
- SaaS
- AI
- RevenueOptimization
- Company
token_bound: false
token_urls:
- https://sandbox.duve.com/api/openapi/v1/oauth2/token
---
