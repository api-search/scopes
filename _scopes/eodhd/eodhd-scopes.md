---
api_specs:
- filename: eodhd-financial-data-openapi.yml
  format: yaml
  label: EODHD Financial Data API
  slug: financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/openapi/eodhd-financial-data-openapi.yml
- filename: eodhd-websockets-asyncapi.yml
  format: yaml
  label: EODHD WebSockets Real-Time API
  slug: websockets-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/asyncapi/eodhd-websockets-asyncapi.yml
- filename: eodhd-eod-api-openapi.yml
  format: yaml
  label: EODHD Eod API
  slug: eodhd-eod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/openapi/eodhd-eod-api-openapi.yml
authorization_urls:
- https://mcpv2.eodhd.dev/authorize
description: ''
docs: https://eodhd.com/financial-apis-blog/eodhd-mcp-server-update-75-tools-oauth-and-api-versioning
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Eodhd Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EODHD publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the EODHD API on a user''s behalf.


  Tokens are issued from https://mcpv2.eodhd.dev/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EODHD
provider_slug: eodhd
schemes:
- flows:
  - authorizationUrl: https://mcpv2.eodhd.dev/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcpv2.eodhd.dev/token
  introspection_endpoint: https://mcpv2.eodhd.dev/introspect
  name: EODHD MCP OAuth
  registration_endpoint: https://mcpv2.eodhd.dev/register
scope_count: 12
scope_names:
- read:eod
- read:intraday
- read:live
- read:fundamentals
- read:news
- read:technicals
- read:options
- read:marketplace
- read:screener
- read:macro
- read:user
- full-access
scopes:
- description: ''
  flows: []
  scope: read:eod
- description: ''
  flows: []
  scope: read:intraday
- description: ''
  flows: []
  scope: read:live
- description: ''
  flows: []
  scope: read:fundamentals
- description: ''
  flows: []
  scope: read:news
- description: ''
  flows: []
  scope: read:technicals
- description: ''
  flows: []
  scope: read:options
- description: ''
  flows: []
  scope: read:marketplace
- description: ''
  flows: []
  scope: read:screener
- description: ''
  flows: []
  scope: read:macro
- description: ''
  flows: []
  scope: read:user
- description: ''
  flows: []
  scope: full-access
slug: eodhd-scopes
source_filename: eodhd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://mcpv2.eodhd.dev/.well-known/oauth-authorization-server\ndocs: https://eodhd.com/financial-apis-blog/eodhd-mcp-server-update-75-tools-oauth-and-api-versioning\nnotes: >-\n  The core REST API uses api_token query-parameter authentication with no OAuth scopes.\n  OAuth 2.0 (authorization code + PKCE S256, dynamic client registration RFC 7591,\n  resource indicators RFC 8707) is published for the v2 MCP server at\n  https://mcpv2.eodhd.dev/v2/mcp; these 12 scopes come verbatim from its RFC 8414\n  authorization-server metadata (scope descriptions are not published — names only).\nschemes:\n  - name: EODHD MCP OAuth\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcpv2.eodhd.dev/authorize\n        tokenUrl: https://mcpv2.eodhd.dev/token\n        pkce: S256\n    registration_endpoint: https://mcpv2.eodhd.dev/register\n    introspection_endpoint: https://mcpv2.eodhd.dev/introspect\nscopes:\n\
  \  - scope: read:eod\n  - scope: read:intraday\n  - scope: read:live\n  - scope: read:fundamentals\n  - scope: read:news\n  - scope: read:technicals\n  - scope: read:options\n  - scope: read:marketplace\n  - scope: read:screener\n  - scope: read:macro\n  - scope: read:user\n  - scope: full-access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/scopes/eodhd-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Financial
- Market Data
- Stock Options
- Stocks
- ETFs
- Forex
- Cryptocurrency
- Fundamentals
- News
token_urls:
- https://mcpv2.eodhd.dev/token
---
