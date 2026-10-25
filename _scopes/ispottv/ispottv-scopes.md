---
api_specs:
- filename: ispottv-openapi-generated.yml
  format: yaml
  label: iSpot.tv API
  slug: ispottv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispottv/refs/heads/main/openapi/_ae-authored/ispottv-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Ispottv Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'iSpot.tv uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.ispot.tv/v4/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: iSpot.tv
provider_slug: ispottv
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.ispot.tv/v4/oauth2/token
  name: OAuth2ClientCredentials
  source: openapi/ispottv-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: ispottv-scopes
source_filename: ispottv-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: none\nsource: openapi/ispottv-openapi-generated.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/ispottv-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ispot.tv/v4/oauth2/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ispottv/refs/heads/main/scopes/ispottv-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- TV Advertising
- Advertising Measurement
- Analytics
- Attribution
- Media
- Marketing
- Streaming
token_bound: false
token_urls:
- https://api.ispot.tv/v4/oauth2/token
---
