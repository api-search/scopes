---
api_specs:
- filename: presto-foundation-statement-api-openapi.yml
  format: yaml
  label: Presto Foundation Statement API
  slug: presto-foundation-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/presto-foundation/refs/heads/main/openapi/presto-foundation-statement-api-openapi.yml
authorization_urls:
- https://example.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Presto Foundation Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Presto Foundation uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Presto Foundation
provider_slug: presto-foundation
schemes:
- description: OAuth 2.0 authenticator (when enabled on the coordinator).
  flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/oauth/token
  name: oauth2
  source: openapi/presto-foundation-statement-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: presto-foundation-scopes
source_filename: presto-foundation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/presto-foundation-statement-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/presto-foundation-statement-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\n  description: OAuth 2.0 authenticator (when enabled on the coordinator).\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/presto-foundation/refs/heads/main/scopes/presto-foundation-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Big Data
- Distributed SQL
- Linux Foundation
- Open Source
- Query Engine
- SQL
token_bound: false
token_urls:
- https://example.com/oauth/token
---
