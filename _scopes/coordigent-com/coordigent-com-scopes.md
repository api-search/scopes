---
api_specs:
- filename: coordigent-com-agents-api-openapi.yml
  format: yaml
  label: Coordigent Agents API
  slug: coordigent-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-agents-api-openapi.yml
- filename: coordigent-com-events-api-openapi.yml
  format: yaml
  label: Coordigent Events API
  slug: coordigent-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-events-api-openapi.yml
- filename: coordigent-com-items-api-openapi.yml
  format: yaml
  label: Coordigent Items API
  slug: coordigent-com-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-items-api-openapi.yml
- filename: coordigent-com-me-api-openapi.yml
  format: yaml
  label: Coordigent Me API
  slug: coordigent-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-me-api-openapi.yml
- filename: coordigent-com-projects-api-openapi.yml
  format: yaml
  label: Coordigent Projects API
  slug: coordigent-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-projects-api-openapi.yml
- filename: coordigent-com-stream-api-openapi.yml
  format: yaml
  label: Coordigent Stream API
  slug: coordigent-com-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-stream-api-openapi.yml
- filename: coordigent-com-threads-api-openapi.yml
  format: yaml
  label: Coordigent Threads API
  slug: coordigent-com-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-threads-api-openapi.yml
- filename: coordigent-com-webhooks-api-openapi.yml
  format: yaml
  label: Coordigent Webhooks API
  slug: coordigent-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coordigent-com/openapi/coordigent-com-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Coordigent Scopes
name_suffix: OAuth Scopes
note: These are API-token (cgpat_) scopes, not OAuth2 scopes. The contract declares an http bearer scheme and names each operation's required scope in an x-scope extension; the full set is the ApiScope enum in components.schemas.
overview: 'Coordigent publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coordigent API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coordigent
provider_slug: coordigent-com
schemes: []
scope_count: 9
scope_names:
- projects:read
- context:read
- items:read
- items:write
- messages:read
- messages:write
- agents:read
- checks:read
- webhooks:manage
scopes:
- description: ''
  flows: []
  scope: projects:read
- description: ''
  flows: []
  scope: context:read
- description: ''
  flows: []
  scope: items:read
- description: ''
  flows: []
  scope: items:write
- description: ''
  flows: []
  scope: messages:read
- description: ''
  flows: []
  scope: messages:write
- description: ''
  flows: []
  scope: agents:read
- description: ''
  flows: []
  scope: checks:read
- description: ''
  flows: []
  scope: webhooks:manage
slug: coordigent-com-scopes
source_filename: coordigent-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/coordigent-com-openapi.yml\nnote: These are API-token (cgpat_) scopes, not OAuth2 scopes. The contract declares an http bearer scheme and names each operation's required scope in an x-scope extension; the full set is the ApiScope enum in components.schemas.\nscheme: apiToken\nscopes:\n- name: projects:read\n  operations: ['GET /v1/projects', 'GET /v1/projects/{id}']\n- name: context:read\n  operations: ['GET /v1/projects/{id}/context']\n- name: items:read\n  operations: ['GET /v1/items', 'GET /v1/items/{id}']\n- name: items:write\n  operations: ['POST /v1/items', 'PATCH /v1/items/{id}', 'POST /v1/items/{id}/events']\n- name: messages:read\n  operations: ['GET /v1/threads', 'GET /v1/threads/{id}/messages']\n- name: messages:write\n  operations: ['POST /v1/threads/{id}/messages']\n- name: agents:read\n  operations: ['GET /v1/agents']\n- name: checks:read\n  operations: []\n  note: In the ApiScope enum; no operation in\
  \ the published contract requires it.\n- name: webhooks:manage\n  operations: ['GET /v1/webhooks', 'POST /v1/webhooks', 'DELETE /v1/webhooks/{id}', 'POST /v1/webhooks/{id}/test']\n"
source_yaml_url: https://artifacts.apis.io/coordigent-com/scopes/coordigent-com-scopes.yml
summary_line: 9 scopes
tags:
- Company
- AI Agents
- Coding Agents
- MCP
- Developer Tools
- Agent Coordination
- CLI
token_bound: false
token_urls: []
---
