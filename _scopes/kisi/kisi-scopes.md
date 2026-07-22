---
api_specs:
- filename: kisi-openapi-original.yml
  format: yaml
  label: Kisi API
  slug: kisi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kisi/refs/heads/main/openapi/kisi-openapi-original.yml
authorization_urls:
- https://api.kisi.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Kisi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'KISI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.kisi.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: KISI
provider_slug: kisi
schemes:
- description: 'OAuth access tokens are sent as bearer tokens. Example: `Authorization: Bearer youraccesstoken`'
  flows:
  - authorizationUrl: https://api.kisi.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kisi.io/oauth/token
  name: OAuth2
  source: openapi/kisi-openapi-original.yml
scope_count: 0
scope_names: []
scopes: []
slug: kisi-scopes
source_filename: kisi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/kisi-openapi-original.yml\nschemes:\n- name: OAuth2\n  source: openapi/kisi-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kisi.io/oauth/authorize\n    tokenUrl: https://api.kisi.io/oauth/token\n  description: 'OAuth access tokens are sent as bearer tokens. Example: `Authorization: Bearer\n    youraccesstoken`'\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kisi/refs/heads/main/scopes/kisi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Physical Access Control
- Security
- Identity
- IoT
- Building Management
- Access Control
- SaaS
token_urls:
- https://api.kisi.io/oauth/token
---
