---
authorization_urls:
- https://use.kick.co/mcp/oauth/authorize
description: ''
docs: https://docs.kick.co/ai/permissions-and-security.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Kick Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kick publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kick API on a user''s behalf.


  Tokens are issued from https://use.kick.co/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kick
provider_slug: kick
schemes:
- flows:
  - authorizationUrl: https://use.kick.co/mcp/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://use.kick.co/mcp/oauth/register
    tokenUrl: https://use.kick.co/mcp/oauth/token
  name: OAuth2
  source: https://use.kick.co/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Tool discovery and read-only calls against the Kick MCP server.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Tools that can change data; write tools are preview-first and require explicit confirmation.
  flows:
  - authorizationCode
  scope: mcp:write
slug: kick-scopes
source_filename: kick-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://use.kick.co/.well-known/oauth-authorization-server\ndocs: https://docs.kick.co/ai/permissions-and-security.md\nschemes:\n- name: OAuth2\n  source: https://use.kick.co/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://use.kick.co/mcp/oauth/authorize\n    tokenUrl: https://use.kick.co/mcp/oauth/token\n    registrationUrl: https://use.kick.co/mcp/oauth/register\n    code_challenge_methods: [S256]\nscopes:\n- scope: mcp:read\n  description: Tool discovery and read-only calls against the Kick MCP server.\n  flows: [authorizationCode]\n  sources: [https://use.kick.co/.well-known/oauth-authorization-server]\n- scope: mcp:write\n  description: Tools that can change data; write tools are preview-first and require explicit confirmation.\n  flows: [authorizationCode]\n  sources: [https://use.kick.co/.well-known/oauth-authorization-server]\nnotes: >-\n  Scopes are those\
  \ advertised for the Kick MCP OAuth surface (RFC 8414 metadata +\n  the Permissions and Security docs). Kick has no public OpenAPI, so scopes are not\n  derived per-operation; the two coarse MCP scopes gate read vs. write across the\n  full tool roster.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kick/refs/heads/main/scopes/kick-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Bookkeeping
- Accounting
- Finance
- FinTech
- MCP
- AI Agents
- Small Business
token_urls:
- https://use.kick.co/mcp/oauth/token
---
