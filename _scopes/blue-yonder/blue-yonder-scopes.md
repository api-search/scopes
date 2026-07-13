---
api_specs:
- filename: blue-yonder-warehouse-management-openapi.yml
  format: yaml
  label: Blue Yonder Warehouse Management API
  slug: blue-yonder-warehouse-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/openapi/blue-yonder-warehouse-management-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Blue Yonder Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'blue-yonder publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the blue-yonder API on a user''s behalf.


  Tokens are issued from https://auth.blueyonder.example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: blue-yonder
provider_slug: blue-yonder
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.blueyonder.example.com/oauth/token
  name: oauth2
  source: openapi/blue-yonder-warehouse-management-openapi.yml
scope_count: 2
scope_names:
- wms:read
- wms:write
scopes:
- description: Read warehouse data
  flows:
  - clientCredentials
  scope: wms:read
- description: Write warehouse data
  flows:
  - clientCredentials
  scope: wms:write
slug: blue-yonder-scopes
source_filename: blue-yonder-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blue-yonder-warehouse-management-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/blue-yonder-warehouse-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.blueyonder.example.com/oauth/token\nscopes:\n- scope: wms:read\n  description: Read warehouse data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/blue-yonder-warehouse-management-openapi.yml\n- scope: wms:write\n  description: Write warehouse data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/blue-yonder-warehouse-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/scopes/blue-yonder-scopes.yml
summary_line: 2 scopes · clientCredentials
tags: []
token_urls:
- https://auth.blueyonder.example.com/oauth/token
---
