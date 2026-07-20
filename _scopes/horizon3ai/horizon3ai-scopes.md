---
authorization_urls:
- https://oauth-proxy.horizon3ai.com/authorize
description: ''
docs: https://docs.horizon3.ai/api/getting_started/authenticate/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Horizon3Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Horizon3.ai publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Horizon3.ai API on a user''s behalf.


  Tokens are issued from https://oauth-proxy.horizon3ai.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Horizon3.ai
provider_slug: horizon3ai
schemes:
- flows:
  - authorizationUrl: https://oauth-proxy.horizon3ai.com/authorize
    flow: authorizationCode
    tokenUrl: https://oauth-proxy.horizon3ai.com/token
  name: mcp-oauth2.1
  source: https://mcp.horizon3ai.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to NodeZero data via the MCP server.
  flows:
  - authorizationCode
  scope: read
- description: Write / action access via the MCP server.
  flows:
  - authorizationCode
  scope: write
slug: horizon3ai-scopes
source_filename: horizon3ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.horizon3ai.com/.well-known/oauth-authorization-server\ndocs: https://docs.horizon3.ai/api/getting_started/authenticate/\nnotes: >-\n  The NodeZero GraphQL API uses API-key -> JWT bearer auth with coarse role-based\n  permissions (not per-scope). OAuth scopes below apply to the hosted MCP server's\n  OAuth 2.1 authorization server. API-key roles are captured as a permission model.\nschemes:\n- name: mcp-oauth2.1\n  source: https://mcp.horizon3ai.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth-proxy.horizon3ai.com/authorize\n    tokenUrl: https://oauth-proxy.horizon3ai.com/token\nscopes:\n- scope: read\n  description: Read access to NodeZero data via the MCP server.\n  flows: [authorizationCode]\n  sources: [https://mcp.horizon3ai.com/.well-known/oauth-authorization-server]\n- scope: write\n  description: Write / action access via the MCP server.\n\
  \  flows: [authorizationCode]\n  sources: [https://mcp.horizon3ai.com/.well-known/oauth-authorization-server]\napi_key_roles:\n- role: User\n  description: Basic read/write permissions; can run pentests and read results.\n- role: Read-only\n  description: Can read pentest results but cannot run pentests.\n- role: NodeZero Runner\n  description: Specialized, heavily restricted role for NodeZero Runner deployments.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon3ai/refs/heads/main/scopes/horizon3ai-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Security
- Cybersecurity
- Penetration Testing
- Autonomous Pentesting
- Attack Surface Management
- Exposure Management
- Vulnerability Management
- GraphQL
- Offensive Security
token_urls:
- https://oauth-proxy.horizon3ai.com/token
---
