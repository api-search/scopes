---
authorization_urls: []
description: ''
docs: https://chiefisnext.com/docs/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Chief Scopes
name_suffix: OAuth Scopes
note: Scope names are read from the scopes_supported array of the protected-resource and authorization-server metadata (both HTTP 200). The docs do not publish a per-scope reference; descriptions are left out rather than invented. The docs state a new MCP connection "can read and propose; it cannot approve or start work, change billing or settings, or show your code."
overview: 'Chief publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Chief API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chief
provider_slug: chiefisnext-com
schemes: []
scope_count: 6
scope_names:
- projects:read
- milestones:read
- summaries:read
- manager_tasks:read
- milestones:propose
- manager_tasks:write
scopes:
- description: ''
  flows: []
  scope: projects:read
- description: ''
  flows: []
  scope: milestones:read
- description: ''
  flows: []
  scope: summaries:read
- description: ''
  flows: []
  scope: manager_tasks:read
- description: ''
  flows: []
  scope: milestones:propose
- description: ''
  flows: []
  scope: manager_tasks:write
slug: chiefisnext-com-scopes
source_filename: chiefisnext-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'generated: ''2026-11-03''

  method: probed

  source: https://mcp.chiefisnext.com/.well-known/oauth-protected-resource

  docs: https://chiefisnext.com/docs/mcp

  name: Chief OAuth scopes

  note: Scope names are read from the scopes_supported array of the protected-resource and authorization-server metadata (both HTTP 200). The docs do not publish a per-scope reference; descriptions are left out rather than invented. The docs state a new MCP connection "can read and propose; it cannot approve or start work, change billing or settings, or show your code."

  scopes:

  - name: projects:read

  - name: milestones:read

  - name: summaries:read

  - name: manager_tasks:read

  - name: milestones:propose

  - name: manager_tasks:write

  '
source_yaml_url: https://artifacts.apis.io/chiefisnext-com/scopes/chiefisnext-com-scopes.yml
summary_line: 6 scopes
tags:
- Company
- AI Agents
- Agent Management
- Coding Agents
- Developer Tools
- MCP
- Project Management
token_bound: false
token_urls: []
---
