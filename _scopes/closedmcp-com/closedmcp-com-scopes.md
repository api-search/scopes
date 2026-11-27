---
authorization_urls: []
description: Scopes as listed in the documented oauth-protected-resource example (scopes_supported) and token response (scope "mcp:tools mcp:list"). The docs give no per-scope descriptions; descriptions below are left minimal.
docs: https://closedmcp.com/docs/api?task=signin
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: ClosedMCP Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ClosedMCP publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClosedMCP API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClosedMCP
provider_slug: closedmcp-com
schemes:
- name: closedmcpOAuth
scope_count: 2
scope_names:
- mcp:tools
- mcp:list
scopes:
- description: ''
  flows: []
  scope: mcp:tools
- description: ''
  flows: []
  scope: mcp:list
slug: closedmcp-com-scopes
source_filename: closedmcp-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://closedmcp.com/docs/api?task=signin\ndocs: https://closedmcp.com/docs/api?task=signin\ndescription: Scopes as listed in the documented oauth-protected-resource example (scopes_supported) and token response (scope\n  \"mcp:tools mcp:list\"). The docs give no per-scope descriptions; descriptions below are left minimal.\nschemes:\n- name: closedmcpOAuth\nscopes:\n- name: mcp:tools\n  description: null\n  evidence: scopes_supported example in GET /.well-known/oauth-protected-resource\n- name: mcp:list\n  description: null\n  evidence: scopes_supported example in GET /.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/closedmcp-com/scopes/closedmcp-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- MCP
- AI Agents
- Gateways
- Access Control
- Serverless
- Developer Tools
token_bound: false
token_urls: []
---
