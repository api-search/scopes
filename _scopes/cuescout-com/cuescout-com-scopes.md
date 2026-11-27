---
authorization_urls: []
description: ''
docs: https://cuescout.com/mcp
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: CueScout Scopes
name_suffix: OAuth Scopes
note: The scope name comes from the MCP server's published oauth-protected-resource metadata (HTTP 200, recorded in mcp/cuescout-com-mcp.yml); the docs do not publish a scopes reference page. No REST OpenAPI exists, so derive-oauth-scopes.py has nothing to read.
overview: 'CueScout publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the CueScout API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CueScout
provider_slug: cuescout-com
schemes: []
scope_count: 1
scope_names:
- account:read
scopes:
- description: Read-only access to the connected CueScout account's brands, visibility, tracked prompts and answers, cited pages, To-dos and site audit through the hosted MCP server.
  flows: []
  scope: account:read
slug: cuescout-com-scopes
source_filename: cuescout-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: mcp/cuescout-com-mcp.yml\nname: CueScout OAuth scopes\ndocs: https://cuescout.com/mcp\nauthorization_server: https://api.cuescout.com\nprotected_resource_metadata: https://mcp.cuescout.com/.well-known/oauth-protected-resource\nscopes:\n- name: account:read\n  description: Read-only access to the connected CueScout account's brands, visibility, tracked prompts and answers, cited pages, To-dos and site audit through the hosted MCP server.\n  applies_to: [get_ai_visibility, list_prompts, get_prompt_answers, list_citation_sources, list_todos, get_todo, get_site_audit, list_brands, get_profile]\n  evidence: 'Docs: \"It only reads. It can''t add prompts, run a check, change settings or see billing.\"'\nnote: The scope name comes from the MCP server's published oauth-protected-resource metadata (HTTP 200, recorded in mcp/cuescout-com-mcp.yml); the docs do not publish a scopes reference page. No REST OpenAPI exists, so derive-oauth-scopes.py\
  \ has nothing to read.\n"
source_yaml_url: https://artifacts.apis.io/cuescout-com/scopes/cuescout-com-scopes.yml
summary_line: 1 scope
tags:
- Company
- AI Visibility
- Generative Engine Optimization
- Brand Monitoring
- SEO
- Competitor Analysis
- MCP
token_bound: false
token_urls: []
---
