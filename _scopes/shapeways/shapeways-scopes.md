---
api_specs:
- filename: shapeways-openapi.yml
  format: yaml
  label: Shapeways API
  slug: shapeways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeways/refs/heads/main/openapi/shapeways-openapi.yml
authorization_urls:
- https://api.shapeways.com/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Shapeways Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Shapeways uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.shapeways.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Shapeways
provider_slug: shapeways
schemes:
- description: OAuth 2.0. client_credentials for single-account apps; authorization_code (+ refresh_token) for multi-user apps.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.shapeways.com/oauth2/token
  - authorizationUrl: https://api.shapeways.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.shapeways.com/oauth2/token
  name: oauth2
  source: openapi/shapeways-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: shapeways-scopes
source_filename: shapeways-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/shapeways-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/shapeways-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.shapeways.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.shapeways.com/oauth2/authorize\n    tokenUrl: https://api.shapeways.com/oauth2/token\n  description: OAuth 2.0. client_credentials for single-account apps; authorization_code (+\n    refresh_token) for multi-user apps.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapeways/refs/heads/main/scopes/shapeways-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- 3D Printing
- Additive Manufacturing
- Manufacturing
- Prototyping
- Hardware
- Fulfillment
- eCommerce
token_urls:
- https://api.shapeways.com/oauth2/token
---
