---
api_specs:
- filename: 24sevenoffice-openapi-generated.yml
  format: yaml
  label: Finago API
  slug: 24sevenoffice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/24sevenoffice/openapi/_ae-authored/24sevenoffice-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Finago Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Finago uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://login.24sevenoffice.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Finago
provider_slug: 24sevenoffice
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.24sevenoffice.com/oauth/token
  name: OAuth2_Client_Credentials
  source: openapi/24sevenoffice-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: 24sevenoffice-scopes
source_filename: 24sevenoffice-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: none\nsource: openapi/24sevenoffice-openapi-generated.yml\nschemes:\n- name: OAuth2_Client_Credentials\n  source: openapi/24sevenoffice-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.24sevenoffice.com/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/24sevenoffice/scopes/24sevenoffice-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Accounting
- Payroll
- Business Management
- Norway
- Sweden
- Finland
token_bound: false
token_urls:
- https://login.24sevenoffice.com/oauth/token
---
