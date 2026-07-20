---
api_specs:
- filename: cintoo-openapi-original.json
  format: json
  label: Cintoo Open API
  slug: cintoo-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cintoo/refs/heads/main/openapi/cintoo-openapi-original.json
authorization_urls:
- https://aec.cintoo.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cintoo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cintoo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://aec.cintoo.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cintoo
provider_slug: cintoo
schemes:
- flows:
  - authorizationUrl: https://aec.cintoo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://aec.cintoo.com/oauth/token
  name: oauth2
  source: openapi/cintoo-openapi-original.json
scope_count: 0
scope_names: []
scopes: []
slug: cintoo-scopes
source_filename: cintoo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cintoo-openapi-original.json\nschemes:\n- name: oauth2\n  source: openapi/cintoo-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://aec.cintoo.com/oauth/authorize\n    tokenUrl: https://aec.cintoo.com/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cintoo/refs/heads/main/scopes/cintoo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Infrastructure SaaS
- Reality Capture
- Digital Twin
- Point Cloud
- 3D
- AEC
- BIM
- Construction
- Scan-to-BIM
- GIS
token_urls:
- https://aec.cintoo.com/oauth/token
---
