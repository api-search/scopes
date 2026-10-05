---
authorization_urls:
- https://edge.vinkius.com/oauth/authorize
description: OAuth scopes advertised by the Vinkius Edge authorization server (the MCP resource server). Descriptions are not published; only the scope names are.
docs: https://vinkius.com/learn/en/tokens
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Vinkius Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vinkius publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vinkius API on a user''s behalf.


  Tokens are issued from https://edge.vinkius.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vinkius
provider_slug: vinkius-com
schemes: []
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: ''
  flows: []
  scope: mcp:read
- description: ''
  flows: []
  scope: mcp:write
slug: vinkius-com-scopes
source_filename: vinkius-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: https://edge.vinkius.com/.well-known/oauth-authorization-server\ndocs: https://vinkius.com/learn/en/tokens\ndescription: OAuth scopes advertised by the Vinkius Edge authorization server (the MCP resource server). Descriptions are not published; only the scope names are.\nauthorization_server: https://edge.vinkius.com\nauthorization_endpoint: https://edge.vinkius.com/oauth/authorize\ntoken_endpoint: https://edge.vinkius.com/oauth/token\nregistration_endpoint: https://edge.vinkius.com/oauth/register\ngrant_types: [authorization_code, refresh_token]\npkce: [S256]\nscopes:\n- name: mcp:read\n  description: null\n  note: Name only - the metadata document and docs publish no description.\n- name: mcp:write\n  description: null\n  note: Name only - the metadata document and docs publish no description.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vinkius-com/refs/heads/main/scopes/vinkius-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- MCP
- AI Agents
- Integration
- Connectors
- AI Governance
- Developer Tools
- Agent-Native
token_bound: false
token_urls:
- https://edge.vinkius.com/oauth/token
---
