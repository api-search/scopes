---
api_specs:
- filename: granular-farm-management-openapi.yml
  format: yaml
  label: Granular Farm Management API
  slug: granular-farm-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/granular/refs/heads/main/openapi/granular-farm-management-openapi.yml
authorization_urls:
- https://auth.granular.ag/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Granular Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Granular (Corteva Agriscience) publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Granular (Corteva Agriscience) API on a user''s behalf.


  Tokens are issued from https://auth.granular.ag/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Granular (Corteva Agriscience)
provider_slug: granular
schemes:
- flows:
  - authorizationUrl: https://auth.granular.ag/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.granular.ag/oauth/token
  name: OAuth2
  source: openapi/granular-farm-management-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read farm data
  flows:
  - authorizationCode
  scope: read
- description: Write farm data
  flows:
  - authorizationCode
  scope: write
slug: granular-scopes
source_filename: granular-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/granular-farm-management-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/granular-farm-management-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.granular.ag/oauth/authorize\n    tokenUrl: https://auth.granular.ag/oauth/token\nscopes:\n- scope: read\n  description: Read farm data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/granular-farm-management-openapi.yml\n- scope: write\n  description: Write farm data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/granular-farm-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granular/refs/heads/main/scopes/granular-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Agriculture
- Farm Management
- Financial
- Crop Planning
- Agronomy
token_urls:
- https://auth.granular.ag/oauth/token
---
