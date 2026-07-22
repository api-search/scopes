---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Zubale Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zubale uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.zubale.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zubale
provider_slug: zubale
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.zubale.com/oauth2/token
  name: oauth2
  source: openapi/zubale-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: zubale-scopes
source_filename: zubale-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zubale-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/zubale-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.zubale.com/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/scopes/zubale-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Ecommerce
token_urls:
- https://api.zubale.com/oauth2/token
---
