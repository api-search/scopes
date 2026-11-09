---
authorization_urls: []
description: ''
docs: https://manifest.build/llm-gateway/docs/integrations/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Manifest Scopes
name_suffix: OAuth Scopes
note: Write tools are not exposed at all to a token without mcp:write. The gateway proxy itself uses harness bearer keys, not scopes.
overview: 'Manifest publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Manifest API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Manifest
provider_slug: manifest
schemes: []
scope_count: 3
scope_names:
- mcp:read
- mcp:write
- offline_access
scopes:
- description: Read harnesses, provider connections, routing, models, prices, and the request log.
  flows: []
  scope: mcp:read
- description: Create, update, and delete harnesses, providers, and routing, and reveal harness keys.
  flows: []
  scope: mcp:write
- description: A refresh token, so the client stays connected after the short-lived access token expires.
  flows: []
  scope: offline_access
slug: manifest-scopes
source_filename: manifest-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'generated: ''2026-11-05''

  method: searched

  source: https://manifest.build/llm-gateway/docs/integrations/mcp

  docs: https://manifest.build/llm-gateway/docs/integrations/mcp

  applies_to: Remote MCP management server (OAuth 2.1)

  scopes:

  - {name: ''mcp:read'', description: ''Read harnesses, provider connections, routing, models, prices, and the request log.''}

  - {name: ''mcp:write'', description: ''Create, update, and delete harnesses, providers, and routing, and reveal harness keys.''}

  - {name: offline_access, description: ''A refresh token, so the client stays connected after the short-lived access token expires.''}

  note: Write tools are not exposed at all to a token without mcp:write. The gateway proxy itself uses harness bearer keys, not scopes.

  '
source_yaml_url: https://artifacts.apis.io/manifest/scopes/manifest-scopes.yml
summary_line: 3 scopes
tags:
- Company
- LLM Gateway
- AI Agents
- Artificial Intelligence
- Open Source
- Observability
- OpenAI-Compatible
- Self-Hosted
token_bound: false
token_urls: []
---
