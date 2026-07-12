---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Alaska Air Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Alaska Airlines publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alaska Airlines API on a user''s behalf.


  Tokens are issued from https://api.alaskaair.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alaska Airlines
provider_slug: alaska-air
schemes:
- description: OAuth 2.0 for Mileage Plan partner API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.alaskaair.com/oauth/token
  name: OAuth2
  source: openapi/alaska-air-mileage-plan-openapi.yaml
scope_count: 2
scope_names:
- loyalty:read
- loyalty:write
scopes:
- description: Read member data
  flows:
  - clientCredentials
  scope: loyalty:read
- description: Report and manage miles
  flows:
  - clientCredentials
  scope: loyalty:write
slug: alaska-air-scopes
source_filename: alaska-air-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alaska-air-mileage-plan-openapi.yaml\nschemes:\n- name: OAuth2\n  source: openapi/alaska-air-mileage-plan-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.alaskaair.com/oauth/token\n  description: OAuth 2.0 for Mileage Plan partner API access\nscopes:\n- scope: loyalty:read\n  description: Read member data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alaska-air-mileage-plan-openapi.yaml\n- scope: loyalty:write\n  description: Report and manage miles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alaska-air-mileage-plan-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/scopes/alaska-air-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
- Fortune 500
token_urls:
- https://api.alaskaair.com/oauth/token
---
