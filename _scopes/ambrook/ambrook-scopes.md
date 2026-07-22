---
authorization_urls:
- https://ambrook.com/oauth/mcp/authorize
description: ''
docs: https://ambrook.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ambrook Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ambrook publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ambrook API on a user''s behalf.


  Tokens are issued from https://ambrook.com/api/v1/oauth/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ambrook
provider_slug: ambrook
schemes:
- flows:
  - authorizationUrl: https://ambrook.com/oauth/mcp/authorize
    flow: authorizationCode
    tokenUrl: https://ambrook.com/api/v1/oauth/mcp/token
  name: OAuth2
  source: well-known/ambrook-oauth-authorization-server.json
scope_count: 5
scope_names:
- mcp:readonly_graphql
- mcp:gateway
- mcp:readonly_admin
- external_mcp:read
- export:download
scopes:
- description: Read-only access to the Ambrook GraphQL data surface via the MCP server
  flows:
  - authorizationCode
  scope: mcp:readonly_graphql
- description: MCP gateway access
  flows:
  - authorizationCode
  scope: mcp:gateway
- description: Read-only administrative access via the MCP server
  flows:
  - authorizationCode
  scope: mcp:readonly_admin
- description: External MCP read access
  flows:
  - authorizationCode
  scope: external_mcp:read
- description: Download exported reports and data
  flows:
  - authorizationCode
  scope: export:download
slug: ambrook-scopes
source_filename: ambrook-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://ambrook.com/.well-known/oauth-authorization-server\ndocs: https://ambrook.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: well-known/ambrook-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ambrook.com/oauth/mcp/authorize\n    tokenUrl: https://ambrook.com/api/v1/oauth/mcp/token\nscopes:\n- scope: mcp:readonly_graphql\n  description: Read-only access to the Ambrook GraphQL data surface via the MCP server\n  flows: [authorizationCode]\n  sources: [well-known/ambrook-oauth-authorization-server.json]\n- scope: mcp:gateway\n  description: MCP gateway access\n  flows: [authorizationCode]\n  sources: [well-known/ambrook-oauth-authorization-server.json]\n- scope: mcp:readonly_admin\n  description: Read-only administrative access via the MCP server\n  flows: [authorizationCode]\n  sources: [well-known/ambrook-oauth-authorization-server.json]\n\
  - scope: external_mcp:read\n  description: External MCP read access\n  flows: [authorizationCode]\n  sources: [well-known/ambrook-oauth-authorization-server.json]\n- scope: export:download\n  description: Download exported reports and data\n  flows: [authorizationCode]\n  sources: [well-known/ambrook-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambrook/refs/heads/main/scopes/ambrook-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Fintech
- Agriculture
- Accounting
- Bookkeeping
- Payments
- Farm Management
- MCP
token_urls:
- https://ambrook.com/api/v1/oauth/mcp/token
---
