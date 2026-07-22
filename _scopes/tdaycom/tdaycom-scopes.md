---
authorization_urls:
- https://tday.com/api/mcp/oauth/authorize
description: ''
docs: https://tday.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tdaycom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tdaycom publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tdaycom API on a user''s behalf.


  Tokens are issued from https://tday.com/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tdaycom
provider_slug: tdaycom
schemes:
- flows:
  - authorizationUrl: https://tday.com/api/mcp/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://tday.com/api/mcp/oauth/token
  name: OAuth2
  source: https://tday.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- tday
scopes:
- description: Single coarse-grained scope granting an OAuth client access to the tday MCP server (https://tday.com/api/mcp). tday does not (publicly) document finer-grained scopes; this is the only value advertised in scopes_supported.
  flows:
  - authorizationCode
  scope: tday
slug: tdaycom-scopes
source_filename: tdaycom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tday.com/.well-known/oauth-authorization-server\ndocs: https://tday.com/.well-known/oauth-protected-resource\nschemes:\n- name: OAuth2\n  source: https://tday.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://tday.com/api/mcp/oauth/authorize\n    tokenUrl: https://tday.com/api/mcp/oauth/token\n    pkce: S256\nscopes:\n- scope: tday\n  description: >-\n    Single coarse-grained scope granting an OAuth client access to the tday MCP\n    server (https://tday.com/api/mcp). tday does not (publicly) document finer-grained\n    scopes; this is the only value advertised in scopes_supported.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/tdaycom-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tdaycom/refs/heads/main/scopes/tdaycom-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Marketing
- Artificial Intelligence
- Content Generation
- Video
- Social Media
- Developer Tools
- MCP
- Agents
- Y Combinator
token_urls:
- https://tday.com/api/mcp/oauth/token
---
