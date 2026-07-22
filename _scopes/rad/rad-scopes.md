---
authorization_urls:
- https://api.rad.live/oauth/authorize
description: ''
docs: https://developers.rad.live/docs/getting-started/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Rad Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rad. publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rad. API on a user''s behalf.


  Tokens are issued from https://api.rad.live/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rad.
provider_slug: rad
schemes:
- flows:
  - authorizationUrl: https://api.rad.live/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.rad.live/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: OAuth2
  pkce: S256
  source: https://api.rad.live/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Access to the Rad TV MCP tool surface (34 tools) for delegated agent access
  flows:
  - authorizationCode
  scope: mcp:tools
slug: rad-scopes
source_filename: rad-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.rad.live/.well-known/oauth-authorization-server\ndocs: https://developers.rad.live/docs/getting-started/authentication\nschemes:\n- name: OAuth2\n  source: https://api.rad.live/.well-known/oauth-authorization-server\n  pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.rad.live/oauth/authorize\n    tokenUrl: https://api.rad.live/oauth/token\nscopes:\n- scope: mcp:tools\n  description: Access to the Rad TV MCP tool surface (34 tools) for delegated agent access\n  flows: [authorizationCode]\n  sources: [well-known/rad-oauth-authorization-server.json]\nnotes:\n- >-\n  OAuth 2.1 delegated access is scoped for MCP clients. Direct API-key (Bearer)\n  access is unscoped and inherits the account's subscription-based permissions;\n  the GraphQL API itself does not advertise per-operation OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rad/refs/heads/main/scopes/rad-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Video
- Streaming
- Creator Economy
- Artificial Intelligence
- Media
- Monetization
- GraphQL
- MCP
token_urls:
- https://api.rad.live/oauth/token
---
