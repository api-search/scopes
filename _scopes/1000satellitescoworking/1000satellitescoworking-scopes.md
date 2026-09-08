---
api_specs:
- filename: 1000satellitescoworking-content-api-openapi.yml
  format: yaml
  label: 1000 Satellites Content API (WordPress REST wp/v2)
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1000satellitescoworking/refs/heads/main/openapi/1000satellitescoworking-content-api-openapi.yml
authorization_urls:
- https://1000satellites.de/oauth/authorize
description: 1000 Satellites publishes RFC 8414 authorization-server metadata at the apex domain, emitted by the WordPress MCP Adapter plugin. It declares exactly one scope, `mcp`, which gates the remote MCP server. This is not a documented developer scope model — the company publishes no OAuth or permissions reference page — it is what the discovery document itself states. No scope descriptions are recorded because the provider publishes none, and writing them would be invention.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 1000Satellitescoworking Scopes
name_suffix: OAuth Scopes
note: ''
overview: '1000 Satellites publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 1000 Satellites API on a user''s behalf.


  Tokens are issued from https://1000satellites.de/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 1000 Satellites
provider_slug: 1000satellitescoworking
schemes:
- flows:
  - authorizationUrl: https://1000satellites.de/oauth/authorize
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://1000satellites.de/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://1000satellites.de/oauth/token
  name: OAuth2
  source: https://1000satellites.de/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: mcp
slug: 1000satellitescoworking-scopes
source_filename: 1000satellitescoworking-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://1000satellites.de/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  1000 Satellites publishes RFC 8414 authorization-server metadata at the apex domain, emitted by the\n  WordPress MCP Adapter plugin. It declares exactly one scope, `mcp`, which gates the remote MCP server.\n  This is not a documented developer scope model — the company publishes no OAuth or permissions reference\n  page — it is what the discovery document itself states. No scope descriptions are recorded because the\n  provider publishes none, and writing them would be invention.\nschemes:\n- name: OAuth2\n  source: https://1000satellites.de/.well-known/oauth-authorization-server\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://1000satellites.de/oauth/authorize\n    tokenUrl: https://1000satellites.de/oauth/token\n    revocationUrl: https://1000satellites.de/oauth/revoke\n    pkce: S256\n    scopes:\
  \ [mcp]\nscopes:\n- scope: mcp\n  description: null\n  description_source: none — the provider publishes no scope reference\n  flows: [authorizationCode]\n  protects: https://1000satellites.de/wp-json/mcp/mcp-oauth-server\n  sources: [https://1000satellites.de/.well-known/oauth-authorization-server]\nx-evidence:\n  fetched: '2026-09-05'\n  probes:\n  - url: https://1000satellites.de/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://1000satellites.de/.well-known/oauth-protected-resource\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1000satellitescoworking/refs/heads/main/scopes/1000satellitescoworking-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Coworking
- Flexible Workspace
- Real Estate
- Office Space
- Workplace
- Meeting Rooms
- Germany
- Content
- MCP
token_urls:
- https://1000satellites.de/oauth/token
---
