---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Manhattan Associates Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'manhattan-associates publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the manhattan-associates API on a user''s behalf.


  Tokens are issued from https://auth.developer.manh.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: manhattan-associates
provider_slug: manhattan-associates
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.developer.manh.com/oauth2/token
  name: OAuth2ClientCredentials
  source: openapi/manhattan-associates-omni-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.developer.manh.com/oauth2/token
  name: OAuth2ClientCredentials
  source: openapi/manhattan-associates-wms-openapi.yml
scope_count: 5
scope_names:
- inventory:read
- orders:read
- orders:write
- wms:read
- wms:write
scopes:
- description: Read inventory positions
  flows:
  - clientCredentials
  scope: inventory:read
- description: Read order data
  flows:
  - clientCredentials
  scope: orders:read
- description: Create and modify orders
  flows:
  - clientCredentials
  scope: orders:write
- description: Read warehouse data
  flows:
  - clientCredentials
  scope: wms:read
- description: Write warehouse operations
  flows:
  - clientCredentials
  scope: wms:write
slug: manhattan-associates-scopes
source_filename: manhattan-associates-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/manhattan-associates-omni-openapi.yml, openapi/manhattan-associates-wms-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/manhattan-associates-omni-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.developer.manh.com/oauth2/token\n- name: OAuth2ClientCredentials\n  source: openapi/manhattan-associates-wms-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.developer.manh.com/oauth2/token\nscopes:\n- scope: inventory:read\n  description: Read inventory positions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/manhattan-associates-omni-openapi.yml\n- scope: orders:read\n  description: Read order data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/manhattan-associates-omni-openapi.yml\n- scope: orders:write\n  description: Create and modify orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/manhattan-associates-omni-openapi.yml\n\
  - scope: wms:read\n  description: Read warehouse data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/manhattan-associates-wms-openapi.yml\n- scope: wms:write\n  description: Write warehouse operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/manhattan-associates-wms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manhattan-associates/refs/heads/main/scopes/manhattan-associates-scopes.yml
summary_line: 5 scopes · clientCredentials
tags: []
token_urls:
- https://auth.developer.manh.com/oauth2/token
---
