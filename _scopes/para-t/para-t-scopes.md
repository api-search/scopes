---
api_specs:
- filename: para-t-openapi-original.yml
  format: yaml
  label: Paraşüt API V4
  slug: paraşüt-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/para-t/refs/heads/main/openapi/para-t-openapi-original.yml
authorization_urls:
- https://api.parasut.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Para T Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Paraşüt uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.parasut.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paraşüt
provider_slug: para-t
schemes:
- flows:
  - authorizationUrl: https://api.parasut.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.parasut.com/oauth/token
  name: parasut_auth
  source: openapi/para-t-openapi-original.yml
scope_count: 0
scope_names: []
scopes: []
slug: para-t-scopes
source_filename: para-t-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/para-t-openapi-original.yml\nschemes:\n- name: parasut_auth\n  source: openapi/para-t-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.parasut.com/oauth/authorize\n    tokenUrl: https://api.parasut.com/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/para-t/refs/heads/main/scopes/para-t-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Accounting
- Pre-Accounting
- e-Invoicing
- Invoicing
- Fintech
- SaaS
- Turkey
- ERP
- JSON:API
token_urls:
- https://api.parasut.com/oauth/token
---
