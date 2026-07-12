---
authorization_urls: []
description: ''
docs: https://api.ibisworld.com/docs/authentication-22026063e0
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Ibisworld Scopes
name_suffix: OAuth Scopes
note: IBISWorld's OAuth 2.0 implementation (password grant against /authentication/token) does not use or document scopes; the security scheme defines an empty scopes object and access is governed by the account's subscription (https://api.ibisworld.com/docs/authentication-22026063e0).
overview: 'IBISWorld uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.ibisworld.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IBISWorld
provider_slug: ibisworld
schemes:
- description: OAuth 2.0 bearer token authentication.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ibisworld.com/oauth/token
  name: OAuth2
  source: openapi/ibisworld-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: ibisworld-scopes
source_filename: ibisworld-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ibisworld-openapi.yml\ndocs: https://api.ibisworld.com/docs/authentication-22026063e0\nnote: IBISWorld's OAuth 2.0 implementation (password grant against /authentication/token) does not use or document scopes; the security scheme defines an empty scopes object and access is governed by the account's subscription (https://api.ibisworld.com/docs/authentication-22026063e0).\nschemes:\n- name: OAuth2\n  source: openapi/ibisworld-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ibisworld.com/oauth/token\n  description: OAuth 2.0 bearer token authentication.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/scopes/ibisworld-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Business Intelligence
- Economics
- Industry Data
- Market Research
token_urls:
- https://api.ibisworld.com/oauth/token
---
