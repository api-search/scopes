---
authorization_urls:
- https://www.genspark.ai/api/mcp/oauth/authorize
description: ''
docs: https://www.genspark.ai/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Genspark Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Genspark publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Genspark API on a user''s behalf.


  Tokens are issued from https://www.genspark.ai/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Genspark
provider_slug: genspark
schemes:
- flows:
  - authorizationUrl: https://www.genspark.ai/api/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.genspark.ai/api/mcp/oauth/token
  name: mcpOAuth
  source: well-known/genspark-openid-configuration.json
scope_count: 4
scope_names:
- mcp:tools:read
- mcp:tools:call
- mcp:resources:read
- mcp:prompts:read
scopes:
- description: List / discover the MCP tools the Genspark server exposes.
  flows:
  - authorizationCode
  scope: mcp:tools:read
- description: Invoke (call) Genspark MCP tools.
  flows:
  - authorizationCode
  scope: mcp:tools:call
- description: Read MCP resources exposed by the Genspark server.
  flows:
  - authorizationCode
  scope: mcp:resources:read
- description: Read MCP prompts exposed by the Genspark server.
  flows:
  - authorizationCode
  scope: mcp:prompts:read
slug: genspark-scopes
source_filename: genspark-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: well-known/genspark-openid-configuration.json\ndocs: https://www.genspark.ai/.well-known/openid-configuration\nschemes:\n- name: mcpOAuth\n  source: well-known/genspark-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.genspark.ai/api/mcp/oauth/authorize\n    tokenUrl: https://www.genspark.ai/api/mcp/oauth/token\nscopes:\n- scope: mcp:tools:read\n  description: List / discover the MCP tools the Genspark server exposes.\n  flows: [authorizationCode]\n  sources: [well-known/genspark-openid-configuration.json]\n- scope: mcp:tools:call\n  description: Invoke (call) Genspark MCP tools.\n  flows: [authorizationCode]\n  sources: [well-known/genspark-openid-configuration.json]\n- scope: mcp:resources:read\n  description: Read MCP resources exposed by the Genspark server.\n  flows: [authorizationCode]\n  sources: [well-known/genspark-openid-configuration.json]\n- scope: mcp:prompts:read\n\
  \  description: Read MCP prompts exposed by the Genspark server.\n  flows: [authorizationCode]\n  sources: [well-known/genspark-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genspark/refs/heads/main/scopes/genspark-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Ai
- Artificial Intelligence
- AI Agents
- MCP
- Model Context Protocol
- Productivity
- Automation
- Search
- Workspace
token_urls:
- https://www.genspark.ai/api/mcp/oauth/token
---
