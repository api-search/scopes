---
api_specs:
- filename: heymarvin-openapi-generated.yml
  format: yaml
  label: HeyMarvin API
  slug: heymarvin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heymarvin/openapi/_ae-authored/heymarvin-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Heymarvin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HeyMarvin publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the HeyMarvin API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HeyMarvin
provider_slug: heymarvin
schemes: []
scope_count: 6
scope_names:
- project:read
- project:write
- file:write
- survey:write
- insight:write
- mcp:read
scopes:
- description: List projects, required by every import flow.
  flows: []
  scope: project:read
- description: Create a project.
  flows: []
  scope: project:write
- description: File import operations (initialize, complete, status).
  flows: []
  scope: file:write
- description: Survey/CSV import operations.
  flows: []
  scope: survey:write
- description: Insight import operations.
  flows: []
  scope: insight:write
- description: MCP server access.
  flows: []
  scope: mcp:read
slug: heymarvin-scopes
source_filename: heymarvin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.heymarvin.com/getting-started/access\nname: HeyMarvin OAuth scopes\nscopes:\n  - name: project:read\n    description: List projects, required by every import flow.\n  - name: project:write\n    description: Create a project.\n  - name: file:write\n    description: File import operations (initialize, complete, status).\n  - name: survey:write\n    description: Survey/CSV import operations.\n  - name: insight:write\n    description: Insight import operations.\n  - name: mcp:read\n    description: MCP server access.\n"
source_yaml_url: https://artifacts.apis.io/heymarvin/scopes/heymarvin-scopes.yml
summary_line: 6 scopes
tags:
- AI
- CustomerInsights
- Analytics
- SaaS
- Platform
token_bound: false
token_urls: []
---
