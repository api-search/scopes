---
authorization_urls: []
description: ''
docs: https://github.com/wellknownmcp/cortex-gateway/blob/main/docs/security.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cortex Gateway Scopes
name_suffix: OAuth Scopes
note: Scopes are deployment-defined. Each backend may only declare scopes under its own prefix (default mcp:<id>:); tools/list is filtered by the token's scopes. The two demo scopes below come from the demo authorization server.
overview: 'Cortex Gateway publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cortex Gateway API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cortex Gateway
provider_slug: cortex-gateway-dev
schemes: []
scope_count: 3
scope_names:
- mcp:demo:read
- mcp:demo:write
- mcp:access
scopes:
- description: Use the read-only demo tools (echo, get_time, get_help)
  flows: []
  scope: mcp:demo:read
- description: Use the demo write tools (pro tier demonstration)
  flows: []
  scope: mcp:demo:write
- description: Example floor scope set via OAUTH_REQUIRED_SCOPES; when set, a token without it gets 403 insufficient_scope before any dispatch (docs/security.md §5).
  flows: []
  scope: mcp:access
slug: cortex-gateway-dev-scopes
source_filename: cortex-gateway-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://github.com/wellknownmcp/cortex-gateway/blob/main/demo/auth-server/src/lib/oauth/scopes.ts\ndocs: https://github.com/wellknownmcp/cortex-gateway/blob/main/docs/security.md\nformat: 'mcp:{domain}:{level}'\nnote: Scopes are deployment-defined. Each backend may only declare scopes under its own prefix (default mcp:<id>:); tools/list is filtered by the token's scopes. The two demo scopes below come from the demo authorization server.\nscopes:\n- name: mcp:demo:read\n  description: Use the read-only demo tools (echo, get_time, get_help)\n- name: mcp:demo:write\n  description: Use the demo write tools (pro tier demonstration)\n- name: mcp:access\n  description: Example floor scope set via OAUTH_REQUIRED_SCOPES; when set, a token without it gets 403 insufficient_scope before any dispatch (docs/security.md §5).\n"
source_yaml_url: https://artifacts.apis.io/cortex-gateway-dev/scopes/cortex-gateway-dev-scopes.yml
summary_line: 3 scopes
tags:
- Company
- MCP
- MCP Gateway
- Open Source
- OAuth 2.1
- AI Agents
- Identity
- Authorization
- Self-Hosted
token_bound: false
token_urls: []
---
