---
authorization_urls: []
description: ''
docs: https://www.creativescope.ai/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CreativeScope Scopes
name_suffix: OAuth Scopes
note: The authorization-server and protected-resource metadata both publish scopes_supported ["mcp:use"]; the docs describe consent only as "creative intelligence under your account". Tool-level access (Free vs Pro/Team) is governed by plan, not scope.
overview: 'CreativeScope publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the CreativeScope API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CreativeScope
provider_slug: creativescope-ai
schemes: []
scope_count: 1
scope_names:
- mcp:use
scopes:
- description: Access the CreativeScope MCP server (creative intelligence under your account).
  flows: []
  scope: mcp:use
slug: creativescope-ai-scopes
source_filename: creativescope-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource:\n- https://api.creativescope.ai/.well-known/oauth-authorization-server\n- https://mcp.creativescope.ai/.well-known/oauth-protected-resource\ndocs: https://www.creativescope.ai/mcp\nnote: The authorization-server and protected-resource metadata both publish scopes_supported [\"mcp:use\"]; the docs describe consent only as \"creative intelligence under your account\". Tool-level access (Free vs Pro/Team) is governed by plan, not scope.\nscopes:\n- name: mcp:use\n  description: Access the CreativeScope MCP server (creative intelligence under your account).\n"
source_yaml_url: https://artifacts.apis.io/creativescope-ai/scopes/creativescope-ai-scopes.yml
summary_line: 1 scope
tags:
- Company
- Mobile Games
- Advertising
- Ad Intelligence
- User Acquisition
- Creative Analytics
- MCP
- AI Agents
token_bound: false
token_urls: []
---
