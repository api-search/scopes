---
api_specs:
- filename: habu-clean-room-api-openapi.yml
  format: yaml
  label: Habu Clean Room API
  slug: habu-clean-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habu/refs/heads/main/openapi/habu-clean-room-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.liveramp.com/clean-room-api/reference/configuring-a-clean-room-api-user
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Habu Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Habu uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.habu.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Habu
provider_slug: habu
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.habu.com/v1/oauth/token
  name: application
  source: openapi/habu-clean-room-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: habu-scopes
source_filename: habu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/habu-clean-room-api-openapi.yml (components.securitySchemes.application) plus a search\n  of the Clean Room API documentation for a scopes/permissions reference.\ndocs: https://developers.liveramp.com/clean-room-api/reference/configuring-a-clean-room-api-user\nschemes:\n- name: application\n  source: openapi/habu-clean-room-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.habu.com/v1/oauth/token\nscope_count: 0\nscopes: []\nfinding: 'The OAuth 2.0 client-credentials flow declares scopes: {} and LiveRamp publishes no scope or\n  permission reference for the Clean Room API. Authorization is enforced by CLEAN ROOM ROLE (getCleanroomRoles\n  / addCleanroomUser / configureCleanRoomQuestionPermissions), which is data in the platform rather than\n  a claim in the token. An agent therefore cannot reason about what a token may do before calling — it\n  can only discover it from a 403.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/habu/refs/heads/main/scopes/habu-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Data Clean Room
- Data Collaboration
- Advertising
- Privacy
- Identity
- Marketing
- Analytics
token_urls:
- https://api.habu.com/v1/oauth/token
---
