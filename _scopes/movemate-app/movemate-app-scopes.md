---
api_specs:
- filename: movemate-app-health-api-openapi.yml
  format: yaml
  label: MoveMate Health API
  slug: movemate-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movemate-app/openapi/movemate-app-health-api-openapi.yml
- filename: movemate-app-mcp-api-openapi.yml
  format: yaml
  label: MoveMate MCP API
  slug: movemate-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movemate-app/openapi/movemate-app-mcp-api-openapi.yml
- filename: movemate-app-oauth-api-openapi.yml
  format: yaml
  label: MoveMate OAuth API
  slug: movemate-app-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movemate-app/openapi/movemate-app-oauth-api-openapi.yml
authorization_urls:
- https://api.movemate.app/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: MoveMate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MoveMate publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MoveMate API on a user''s behalf.


  Tokens are issued from https://api.movemate.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MoveMate
provider_slug: movemate-app
schemes:
- description: OAuth 2.1 authorization code with PKCE S256. Dynamic client registration (RFC 7591) at /oauth/register.
  flows:
  - authorizationUrl: https://api.movemate.app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.movemate.app/oauth/token
  name: oauth2
  source: openapi/movemate-app-openapi.json
scope_count: 4
scope_names:
- library:read
- profile:read
- stats:read
- workouts:write
scopes:
- description: Read the exercise library and workouts, including the user’s own
  flows:
  - authorizationCode
  scope: library:read
- description: Read the connected user’s profile and body stats
  flows:
  - authorizationCode
  scope: profile:read
- description: Read training history, stats, progression, personal records and planned workouts
  flows:
  - authorizationCode
  scope: stats:read
- description: Save, edit, schedule, reschedule and cancel workouts, add custom exercises, and log finished workouts
  flows:
  - authorizationCode
  scope: workouts:write
slug: movemate-app-scopes
source_filename: movemate-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/movemate-app-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/movemate-app-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.movemate.app/oauth/authorize\n    tokenUrl: https://api.movemate.app/oauth/token\n  description: OAuth 2.1 authorization code with PKCE S256. Dynamic client registration (RFC\n    7591) at /oauth/register.\nscopes:\n- scope: library:read\n  description: Read the exercise library and workouts, including the user’s own\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/movemate-app-openapi.json\n- scope: profile:read\n  description: Read the connected user’s profile and body stats\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/movemate-app-openapi.json\n- scope: stats:read\n  description: Read training history, stats, progression, personal records and planned workouts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/movemate-app-openapi.json\n\
  - scope: workouts:write\n  description: Save, edit, schedule, reschedule and cancel workouts, add custom exercises, and\n    log finished workouts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/movemate-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/movemate-app/scopes/movemate-app-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Fitness
- Artificial Intelligence
- Workouts
- Health
- Mobile
token_bound: false
token_urls:
- https://api.movemate.app/oauth/token
---
