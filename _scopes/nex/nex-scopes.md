---
api_specs:
- filename: nex-ai-lists-api-openapi.yml
  format: yaml
  label: Nex AI Lists API
  slug: nex-ai-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-ai-lists-api-openapi.yml
- filename: nex-compounding-api-openapi.yml
  format: yaml
  label: Nex Compounding API
  slug: nex-compounding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-compounding-api-openapi.yml
- filename: nex-context-api-openapi.yml
  format: yaml
  label: Nex Context API
  slug: nex-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-context-api-openapi.yml
- filename: nex-graph-api-openapi.yml
  format: yaml
  label: Nex Graph API
  slug: nex-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-graph-api-openapi.yml
- filename: nex-insights-api-openapi.yml
  format: yaml
  label: Nex Insights API
  slug: nex-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-insights-api-openapi.yml
- filename: nex-integrations-api-openapi.yml
  format: yaml
  label: Nex Integrations API
  slug: nex-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-integrations-api-openapi.yml
- filename: nex-lists-api-openapi.yml
  format: yaml
  label: Nex Lists API
  slug: nex-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-lists-api-openapi.yml
- filename: nex-notes-api-openapi.yml
  format: yaml
  label: Nex Notes API
  slug: nex-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-notes-api-openapi.yml
- filename: nex-notifications-api-openapi.yml
  format: yaml
  label: Nex Notifications API
  slug: nex-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-notifications-api-openapi.yml
- filename: nex-objects-api-openapi.yml
  format: yaml
  label: Nex Objects API
  slug: nex-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-objects-api-openapi.yml
- filename: nex-records-api-openapi.yml
  format: yaml
  label: Nex Records API
  slug: nex-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-records-api-openapi.yml
- filename: nex-relationships-api-openapi.yml
  format: yaml
  label: Nex Relationships API
  slug: nex-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-relationships-api-openapi.yml
- filename: nex-schema-api-openapi.yml
  format: yaml
  label: Nex Schema API
  slug: nex-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-schema-api-openapi.yml
- filename: nex-search-api-openapi.yml
  format: yaml
  label: Nex Search API
  slug: nex-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-search-api-openapi.yml
- filename: nex-tasks-api-openapi.yml
  format: yaml
  label: Nex Tasks API
  slug: nex-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-tasks-api-openapi.yml
- filename: nex-timeline-api-openapi.yml
  format: yaml
  label: Nex Timeline API
  slug: nex-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-timeline-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.nex.ai/api-reference/introduction
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Nex Scopes
name_suffix: OAuth Scopes
note: 'Nex uses API-key authentication (Authorization: Bearer). Scopes are attached to each API key at generation time in the Nex web UI; there is no OAuth2 flow. This is the published permission/scope reference for API keys.'
overview: 'Nex publishes 18 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nex API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nex
provider_slug: nex
schemes: []
scope_count: 18
scope_names:
- object.read
- object.write
- record.read
- record.write
- list.read
- list.member.read
- list.member.write
- relationship.read
- relationship.write
- task.read
- task.write
- note.read
- note.write
- integration.read
- integration.write
- notification.read
- notification.write
- insight.stream
scopes:
- description: Read object definitions and their attributes
  flows: []
  scope: object.read
- description: Create, update, and delete object definitions, attributes, and lists
  flows: []
  scope: object.write
- description: Read records, search, view timelines, and access knowledge graph
  flows: []
  scope: record.read
- description: Create, update, and delete records and list memberships
  flows: []
  scope: record.write
- description: Read list definitions
  flows: []
  scope: list.read
- description: Read list members and records
  flows: []
  scope: list.member.read
- description: Add, update, and remove list members
  flows: []
  scope: list.member.write
- description: Read relationship definitions
  flows: []
  scope: relationship.read
- description: Create and delete relationship definitions and instances
  flows: []
  scope: relationship.write
- description: Read tasks
  flows: []
  scope: task.read
- description: Create, update, and delete tasks
  flows: []
  scope: task.write
- description: Read notes
  flows: []
  scope: note.read
- description: Create, update, and delete notes
  flows: []
  scope: note.write
- description: List integrations and check connection status
  flows: []
  scope: integration.read
- description: Connect and disconnect integrations
  flows: []
  scope: integration.write
- description: Read notification preferences and custom notification rules
  flows: []
  scope: notification.read
- description: Create, update, and delete notification preferences and custom rules
  flows: []
  scope: notification.write
- description: SSE insight streaming
  flows: []
  scope: insight.stream
slug: nex-scopes
source_filename: nex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nex-openapi-original.json\ndocs: https://docs.nex.ai/api-reference/introduction\nnote: >-\n  Nex uses API-key authentication (Authorization: Bearer). Scopes are attached\n  to each API key at generation time in the Nex web UI; there is no OAuth2 flow.\n  This is the published permission/scope reference for API keys.\nscopes:\n- scope: object.read\n  description: Read object definitions and their attributes\n- scope: object.write\n  description: Create, update, and delete object definitions, attributes, and lists\n- scope: record.read\n  description: Read records, search, view timelines, and access knowledge graph\n- scope: record.write\n  description: Create, update, and delete records and list memberships\n- scope: list.read\n  description: Read list definitions\n- scope: list.member.read\n  description: Read list members and records\n- scope: list.member.write\n  description: Add, update, and remove list members\n\
  - scope: relationship.read\n  description: Read relationship definitions\n- scope: relationship.write\n  description: Create and delete relationship definitions and instances\n- scope: task.read\n  description: Read tasks\n- scope: task.write\n  description: Create, update, and delete tasks\n- scope: note.read\n  description: Read notes\n- scope: note.write\n  description: Create, update, and delete notes\n- scope: integration.read\n  description: List integrations and check connection status\n- scope: integration.write\n  description: Connect and disconnect integrations\n- scope: notification.read\n  description: Read notification preferences and custom notification rules\n- scope: notification.write\n  description: Create, update, and delete notification preferences and custom rules\n- scope: insight.stream\n  description: SSE insight streaming\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/scopes/nex-scopes.yml
summary_line: 18 scopes
tags:
- Company
- AI Agents
- Knowledge Graph
- Context
- Memory
- MCP
- Model Context Protocol
- Workflow Automation
- Integrations
- Developer API
token_urls: []
---
