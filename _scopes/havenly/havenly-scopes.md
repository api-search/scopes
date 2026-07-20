---
api_specs:
- filename: havenly-openapi.yml
  format: yaml
  label: Havenly API
  slug: havenly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Havenly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Havenly uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.havenly.com/oauth.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Havenly
provider_slug: havenly
schemes:
- flows:
  - flow: password
    tokenUrl: https://api.havenly.com/oauth
  name: oauth2
  source: openapi/havenly-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: havenly-scopes
source_filename: havenly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/havenly-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/havenly-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.havenly.com/oauth\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/scopes/havenly-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Interior Design
- Home Decor
- Furniture
- E-Commerce
- Marketplace
- Design
- Retail
- AI
token_urls:
- https://api.havenly.com/oauth
---
