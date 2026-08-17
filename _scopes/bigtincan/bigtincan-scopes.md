---
api_specs:
- filename: bigtincan-hub-api-openapi.json
  format: json
  label: Bigtincan Hub API
  slug: bigtincan-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-hub-api-openapi.json
authorization_urls:
- https://pubapi.bigtincan.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- password
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bigtincan Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bigtincan uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://pubapi.bigtincan.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bigtincan
provider_slug: bigtincan
schemes:
- description: 'Client ID + Client Secret + API Key exchanged at /services/oauth2/token with grant_type=password. Returns access_token + refresh_token. The As-User header is available only with this flow. Source: https://pubapi.bigtincan.com/doc/interactive/'
  flows:
  - flow: password
    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token
  name: oauth2_password
  source: openapi/bigtincan-hub-api-openapi.json
- description: 'Interactive Bigtincan Hub user login. The As-User header is disabled for this flow. Source: https://pubapi.bigtincan.com/doc/interactive/'
  flows:
  - authorizationUrl: https://pubapi.bigtincan.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token
  name: oauth2_authorization_code
  source: openapi/bigtincan-hub-api-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: bigtincan-scopes
source_filename: bigtincan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/bigtincan-hub-api-openapi.json\nschemes:\n- name: oauth2_password\n  source: openapi/bigtincan-hub-api-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token\n  description: 'Client ID + Client Secret + API Key exchanged at /services/oauth2/token with\n    grant_type=password. Returns access_token + refresh_token. The As-User header is available\n    only with this flow. Source: https://pubapi.bigtincan.com/doc/interactive/'\n- name: oauth2_authorization_code\n  source: openapi/bigtincan-hub-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://pubapi.bigtincan.com/services/oauth2/authorize\n    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token\n  description: 'Interactive Bigtincan Hub user login. The As-User header is disabled for this\n    flow. Source: https://pubapi.bigtincan.com/doc/interactive/'\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/scopes/bigtincan-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Sales Enablement
- Content Management
- Training
- Coaching
- Buyer Engagement
- Analytics
- CRM Integration
- Digital Sales Rooms
token_urls:
- https://pubapi.bigtincan.com/services/oauth2/token
---
