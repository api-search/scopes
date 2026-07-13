---
api_specs:
- filename: openapi.json
  format: json
  label: Xata Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://api.xata.tech/openapi.json
- filename: openapi.json
  format: json
  label: Xata SQL Gateway
  slug: sql-gateway
  spec_type: OpenAPI
  url: https://api.xata.tech/openapi.json
authorization_urls:
- https://auth.xata.io/realms/xata/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Xata Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Xata publishes 15 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xata API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xata
provider_slug: xata
schemes:
- flows:
  - authorizationUrl: https://auth.xata.io/realms/xata/protocol/openid-connect/auth
    flow: implicit
  name: xata
  source: openapi/xata-management-api-openapi.yml
scope_count: 15
scope_names:
- branch:read
- branch:write
- credentials:read
- credentials:write
- invite:read
- invite:write
- keys:read
- keys:write
- logs:read
- marketplace:write
- metrics:read
- org:read
- org:write
- project:read
- project:write
scopes:
- description: Read branch information
  flows:
  - implicit
  scope: branch:read
- description: Create and modify branches
  flows:
  - implicit
  scope: branch:write
- description: Read credentials
  flows:
  - implicit
  scope: credentials:read
- description: Rotate credentials
  flows:
  - implicit
  scope: credentials:write
- description: ''
  flows: []
  scope: invite:read
- description: ''
  flows: []
  scope: invite:write
- description: Read API keys
  flows:
  - implicit
  scope: keys:read
- description: Create and manage API keys
  flows:
  - implicit
  scope: keys:write
- description: Read logs data
  flows:
  - implicit
  scope: logs:read
- description: Register with cloud marketplaces
  flows:
  - implicit
  scope: marketplace:write
- description: Read metrics data
  flows:
  - implicit
  scope: metrics:read
- description: Read organization information
  flows:
  - implicit
  scope: org:read
- description: Create and modify organizations
  flows:
  - implicit
  scope: org:write
- description: Read project information
  flows:
  - implicit
  scope: project:read
- description: Create and modify projects
  flows:
  - implicit
  scope: project:write
slug: xata-scopes
source_filename: xata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xata-management-api-openapi.yml\nschemes:\n- name: xata\n  source: openapi/xata-management-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.xata.io/realms/xata/protocol/openid-connect/auth\nscopes:\n- scope: branch:read\n  description: Read branch information\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: branch:write\n  description: Create and modify branches\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: credentials:read\n  description: Read credentials\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: credentials:write\n  description: Rotate credentials\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: invite:read\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: invite:write\n  sources:\n  - openapi/xata-management-api-openapi.yml\n\
  - scope: keys:read\n  description: Read API keys\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: keys:write\n  description: Create and manage API keys\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: logs:read\n  description: Read logs data\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: marketplace:write\n  description: Register with cloud marketplaces\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: metrics:read\n  description: Read metrics data\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: org:read\n  description: Read organization information\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: org:write\n  description: Create and modify organizations\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n\
  - scope: project:read\n  description: Read project information\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- scope: project:write\n  description: Create and modify projects\n  flows:\n  - implicit\n  sources:\n  - openapi/xata-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xata/refs/heads/main/scopes/xata-scopes.yml
summary_line: 15 scopes · implicit
tags:
- Database
- Postgres
- Serverless
- Developer Tools
- Branching
- AI Agent
token_urls: []
---
