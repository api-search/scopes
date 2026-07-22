---
authorization_urls:
- https://treasury.app/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Treasury Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Treasury publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Treasury API on a user''s behalf.


  Tokens are issued from https://treasury.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Treasury
provider_slug: treasury
schemes:
- flows:
  - authorizationUrl: https://treasury.app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://treasury.app/oauth/token
  name: OAuth2
  source: well-known/treasury-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp:connect
scopes:
- description: Connect to the Treasury Model Context Protocol (MCP) server at https://treasury.app/mcp.
  flows:
  - authorizationCode
  scope: mcp:connect
slug: treasury-scopes
source_filename: treasury-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://treasury.app/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: well-known/treasury-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://treasury.app/oauth/authorize\n    tokenUrl: https://treasury.app/oauth/token\nscopes:\n- scope: mcp:connect\n  description: Connect to the Treasury Model Context Protocol (MCP) server at https://treasury.app/mcp.\n  flows: [authorizationCode]\n  sources: [well-known/treasury-oauth-authorization-server.json]\nnotes: >-\n  Only one scope (mcp:connect) is advertised in the authorization server\n  metadata; it gates access to the MCP server. Individual tool-level scopes, if\n  any, are not exposed in the discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasury/refs/heads/main/scopes/treasury-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Investing
- Personal Finance
- Fintech
- Brokerage
- Financial Education
- MCP
- Agent
token_urls:
- https://treasury.app/oauth/token
---
