---
api_specs:
- filename: filepad-ai-openapi-generated.yml
  format: yaml
  label: Filepad API
  slug: filepad-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filepad-ai/openapi/_ae-authored/filepad-ai-openapi-generated.yml
authorization_urls: []
description: ''
docs: https://filepad.ai/docs/guides/connecting-an-agent/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Filepad Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Filepad publishes 8 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Filepad API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Filepad
provider_slug: filepad-ai
schemes: []
scope_count: 8
scope_names:
- events.write
- signals:write
- notifications:read
- env:read
- artifacts:read
- artifacts:write
- memory:read
- memory:write
scopes:
- description: Write external agent activity events and agent-hook invocations.
  flows: []
  scope: events.write
- description: Create signals (findings) on a workspace.
  flows: []
  scope: signals:write
- description: Read and acknowledge the agent's mailbox.
  flows: []
  scope: notifications:read
- description: List and read signals (findings) on a workspace.
  flows: []
  scope: env:read
- description: Search and read workspace artifacts via MCP.
  flows: []
  scope: artifacts:read
- description: Edit workspace artifacts via MCP (higher-risk writes may require approval).
  flows: []
  scope: artifacts:write
- description: Read workspace memory via MCP.
  flows: []
  scope: memory:read
- description: Write workspace memory via MCP.
  flows: []
  scope: memory:write
slug: filepad-ai-scopes
source_filename: filepad-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filepad.ai/docs/integrations/api-v1/\ndocs: https://filepad.ai/docs/guides/connecting-an-agent/\nscopes:\n  - name: events.write\n    description: Write external agent activity events and agent-hook invocations.\n    surface: agent-access\n  - name: signals:write\n    description: Create signals (findings) on a workspace.\n    surface: agent-access\n  - name: notifications:read\n    description: Read and acknowledge the agent's mailbox.\n    surface: agent-access\n  - name: env:read\n    description: List and read signals (findings) on a workspace.\n    surface: agent-access\n  - name: artifacts:read\n    description: Search and read workspace artifacts via MCP.\n    surface: mcp\n  - name: artifacts:write\n    description: Edit workspace artifacts via MCP (higher-risk writes may require approval).\n    surface: mcp\n  - name: memory:read\n    description: Read workspace memory via MCP.\n    surface: mcp\n  - name:\
  \ memory:write\n    description: Write workspace memory via MCP.\n    surface: mcp\nnotes: >-\n  Scopes are checked before a request touches any data. A key only carries the\n  scopes explicitly granted. Insufficient scope returns 403 FORBIDDEN_SCOPE.\n"
source_yaml_url: https://artifacts.apis.io/filepad-ai/scopes/filepad-ai-scopes.yml
summary_line: 8 scopes
tags:
- Low-Code
- No-Code
- AI Agents
- Workflows
- Developer Tools
- Internal Tools
- Workspace
- Apps
token_bound: false
token_urls: []
---
