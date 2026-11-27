---
api_specs:
- filename: fixter-dev-openapi-generated.yml
  format: yaml
  label: Fixter API
  slug: fixter-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixter-dev/openapi/_ae-authored/fixter-dev-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Fixter Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Fixter uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from tokenUrl.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fixter
provider_slug: fixter-dev
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: tokenUrl
  name: OAUTH2_CLIENT_CREDENTIALS
  source: openapi/fixter-dev-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: fixter-dev-scopes
source_filename: fixter-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: none\nsource: openapi/fixter-dev-openapi-generated.yml\nschemes:\n- name: OAUTH2_CLIENT_CREDENTIALS\n  source: openapi/fixter-dev-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: tokenUrl\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/fixter-dev/scopes/fixter-dev-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Monitoring
- Artificial Intelligence
- APM
- Error Tracking
- MCP
token_bound: false
token_urls:
- tokenUrl
---
