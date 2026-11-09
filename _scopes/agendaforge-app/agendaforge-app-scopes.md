---
api_specs:
- filename: agendaforge-app-connection-api-openapi.yml
  format: yaml
  label: agendaforge-app Connection API
  slug: agendaforge-app-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-connection-api-openapi.yml
- filename: agendaforge-app-jobs-api-openapi.yml
  format: yaml
  label: agendaforge-app Jobs API
  slug: agendaforge-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-jobs-api-openapi.yml
- filename: agendaforge-app-records-api-openapi.yml
  format: yaml
  label: agendaforge-app Records API
  slug: agendaforge-app-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-records-api-openapi.yml
- filename: agendaforge-app-webhooks-api-openapi.yml
  format: yaml
  label: agendaforge-app Webhooks API
  slug: agendaforge-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Agendaforge App Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'agendaforge-app publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the agendaforge-app API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: agendaforge-app
provider_slug: agendaforge-app
schemes: []
scope_count: 4
scope_names:
- public_api
- mcp:read
- mcp:write
- tickets:import
scopes:
- description: Grants access to the REST API (default).
  flows: []
  scope: public_api
- description: Read access to the AgendaForge MCP server for AI clients.
  flows: []
  scope: mcp:read
- description: Write access to the AgendaForge MCP server for AI clients.
  flows: []
  scope: mcp:write
- description: Allows importing tickets via POST /imports/tickets.
  flows: []
  scope: tickets:import
slug: agendaforge-app-scopes
source_filename: agendaforge-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://agendaforge.app/docs/api#authentication\nscopes:\n  - name: public_api\n    description: Grants access to the REST API (default).\n  - name: mcp:read\n    description: Read access to the AgendaForge MCP server for AI clients.\n  - name: mcp:write\n    description: Write access to the AgendaForge MCP server for AI clients.\n  - name: tickets:import\n    description: Allows importing tickets via POST /imports/tickets.\n"
source_yaml_url: https://artifacts.apis.io/agendaforge-app/scopes/agendaforge-app-scopes.yml
summary_line: 4 scopes
tags:
- Event Management
- Software-as-a-Service
- AI-native
- Conferences
- Software
token_bound: false
token_urls: []
---
