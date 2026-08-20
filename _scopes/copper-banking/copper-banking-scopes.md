---
authorization_urls:
- https://mcp.getcopper.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Copper Banking Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Copper Banking publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Copper Banking API on a user''s behalf.


  Tokens are issued from https://mcp.getcopper.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Copper Banking
provider_slug: copper-banking
schemes:
- flows:
  - authorizationUrl: https://mcp.getcopper.com/authorize
    flow: authorizationCode
    pkce: S256
    refresh_token: true
    tokenUrl: https://mcp.getcopper.com/token
  name: CopperMCPOAuth2
  source: well-known/copper-banking-oauth-authorization-server.json
  type: oauth2
scope_count: 2
scope_names:
- mcp
- offline_access
scopes:
- description: Access to Copper's Model Context Protocol server. Copper publishes no description of what this scope grants; the name is taken verbatim from scopes_supported in the authorization server metadata.
  flows:
  - authorizationCode
  scope: mcp
- description: Issue a refresh token so the client can obtain new access tokens without the resource owner present (OpenID Connect / RFC 6749 offline access).
  flows:
  - authorizationCode
  scope: offline_access
slug: copper-banking-scopes
source_filename: copper-banking-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://mcp.getcopper.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: Copper publishes no scope or permission reference; the scope list below is\n  taken verbatim from the authorization server's own RFC 8414 metadata document.\nschemes:\n- name: CopperMCPOAuth2\n  type: oauth2\n  source: well-known/copper-banking-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.getcopper.com/authorize\n    tokenUrl: https://mcp.getcopper.com/token\n    pkce: S256\n    refresh_token: true\nscopes:\n- scope: mcp\n  description: Access to Copper's Model Context Protocol server. Copper publishes no\n    description of what this scope grants; the name is taken verbatim from\n    scopes_supported in the authorization server metadata.\n  flows: [authorizationCode]\n  sources: [well-known/copper-banking-oauth-authorization-server.json]\n- scope: offline_access\n  description:\
  \ Issue a refresh token so the client can obtain new access tokens without\n    the resource owner present (OpenID Connect / RFC 6749 offline access).\n  flows: [authorizationCode]\n  sources: [well-known/copper-banking-oauth-authorization-server.json]\ncoverage:\n  scopes_declared: 2\n  granularity: coarse\n  note: >-\n    A single `mcp` scope covers the entire protected resource. There is no per-tool or\n    per-resource scope decomposition, so an agent token cannot be least-privileged\n    against individual Copper capabilities.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://mcp.getcopper.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copper-banking/refs/heads/main/scopes/copper-banking-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Financial-Services
- Fintech
- Consumer Finance
- Financial Literacy
- Rewards
- Neobank
- Mobile Banking
- Teen Banking
- MCP
token_urls:
- https://mcp.getcopper.com/token
---
