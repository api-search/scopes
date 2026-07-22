---
authorization_urls:
- https://api.lightyear.com/oauth2/internal-mcp/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lightyear Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lightyear publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lightyear API on a user''s behalf.


  Tokens are issued from https://api.lightyear.com/oauth2/internal-mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lightyear
provider_slug: lightyear
schemes:
- flows:
  - authorizationUrl: https://api.lightyear.com/oauth2/internal-mcp/authorize
    flow: authorizationCode
    tokenUrl: https://api.lightyear.com/oauth2/internal-mcp/token
  name: internal-mcp
  source: well-known/lightyear-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: mcp
slug: lightyear-scopes
source_filename: lightyear-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.lightyear.com/.well-known/oauth-authorization-server\ndocs: null\nnotes: >-\n  Lightyear publishes no scopes/permissions reference page. The single scope below is the only one\n  advertised in the RFC 8414 authorization server metadata (scopes_supported), for an internal MCP\n  integration. No scope descriptions are published by the provider.\nschemes:\n- name: internal-mcp\n  source: well-known/lightyear-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.lightyear.com/oauth2/internal-mcp/authorize\n    tokenUrl: https://api.lightyear.com/oauth2/internal-mcp/token\nscopes:\n- scope: mcp\n  description: null\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/lightyear-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightyear/refs/heads/main/scopes/lightyear-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Financial Services
- Investing
- Brokerage
- Stocks
- ETFs
- Fintech
- Wealth Management
- Europe
token_urls:
- https://api.lightyear.com/oauth2/internal-mcp/token
---
