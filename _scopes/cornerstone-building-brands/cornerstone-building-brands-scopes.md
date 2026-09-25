---
authorization_urls:
- https://www.cornerstonebuildingbrands.com/oauth/authorize
description: Cornerstone Building Brands publishes RFC 8414 authorization-server metadata on www.cornerstonebuildingbrands.com, emitted by the WordPress MCP Adapter. It declares exactly one scope, `mcp`, which gates the remote MCP server. This is not a documented developer scope model — the company publishes no OAuth or permissions reference page — it is what the discovery document itself states. No scope description is recorded because the provider publishes none; writing one would be invention.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cornerstone Building Brands Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cornerstone Building Brands publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cornerstone Building Brands API on a user''s behalf.


  Tokens are issued from https://www.cornerstonebuildingbrands.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cornerstone Building Brands
provider_slug: cornerstone-building-brands
schemes:
- flows:
  - authorizationUrl: https://www.cornerstonebuildingbrands.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://www.cornerstonebuildingbrands.com/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://www.cornerstonebuildingbrands.com/oauth/token
  name: OAuth2
  source: https://www.cornerstonebuildingbrands.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: mcp
slug: cornerstone-building-brands-scopes
source_filename: cornerstone-building-brands-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://www.cornerstonebuildingbrands.com/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Cornerstone Building Brands publishes RFC 8414 authorization-server metadata on www.cornerstonebuildingbrands.com,\n  emitted by the WordPress MCP Adapter. It declares exactly one scope, `mcp`, which gates the remote MCP\n  server. This is not a documented developer scope model — the company publishes no OAuth or permissions\n  reference page — it is what the discovery document itself states. No scope description is recorded\n  because the provider publishes none; writing one would be invention.\nschemes:\n- name: OAuth2\n  source: https://www.cornerstonebuildingbrands.com/.well-known/oauth-authorization-server\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.cornerstonebuildingbrands.com/oauth/authorize\n    tokenUrl: https://www.cornerstonebuildingbrands.com/oauth/token\n\
  \    revocationUrl: https://www.cornerstonebuildingbrands.com/oauth/revoke\n    pkce: S256\n    scopes: [mcp]\nscopes:\n- scope: mcp\n  description: null\n  description_source: none — the provider publishes no scope reference\n  flows: [authorizationCode]\n  protects: https://www.cornerstonebuildingbrands.com/wp-json/mcp/mcp-oauth-server\n  sources: [https://www.cornerstonebuildingbrands.com/.well-known/oauth-authorization-server]\nx-evidence:\n  fetched: '2026-09-19'\n  probes:\n  - url: https://www.cornerstonebuildingbrands.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://www.cornerstonebuildingbrands.com/.well-known/oauth-protected-resource\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornerstone-building-brands/refs/heads/main/scopes/cornerstone-building-brands-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Building Products
- Construction
- Manufacturing
- Building Materials
- MCP
- WordPress
- News
token_urls:
- https://www.cornerstonebuildingbrands.com/oauth/token
---
