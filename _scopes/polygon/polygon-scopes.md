---
api_specs:
- filename: polygon-websocket-asyncapi.yml
  format: yaml
  label: Polygon WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/asyncapi/polygon-websocket-asyncapi.yml
- filename: polygon-aggregates-api-openapi.yml
  format: yaml
  label: Polygon Aggregates API
  slug: polygon-aggregates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-aggregates-api-openapi.yml
- filename: polygon-books-api-openapi.yml
  format: yaml
  label: Polygon Books API
  slug: polygon-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-books-api-openapi.yml
- filename: polygon-contracts-api-openapi.yml
  format: yaml
  label: Polygon Contracts API
  slug: polygon-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-contracts-api-openapi.yml
- filename: polygon-conversion-api-openapi.yml
  format: yaml
  label: Polygon Conversion API
  slug: polygon-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-conversion-api-openapi.yml
- filename: polygon-corporateactions-api-openapi.yml
  format: yaml
  label: Polygon CorporateActions API
  slug: polygon-corporateactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-corporateactions-api-openapi.yml
- filename: polygon-dailybars-api-openapi.yml
  format: yaml
  label: Polygon DailyBars API
  slug: polygon-dailybars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-dailybars-api-openapi.yml
- filename: polygon-markets-api-openapi.yml
  format: yaml
  label: Polygon Markets API
  slug: polygon-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-markets-api-openapi.yml
- filename: polygon-news-api-openapi.yml
  format: yaml
  label: Polygon News API
  slug: polygon-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-news-api-openapi.yml
- filename: polygon-quotes-api-openapi.yml
  format: yaml
  label: Polygon Quotes API
  slug: polygon-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-quotes-api-openapi.yml
- filename: polygon-snapshots-api-openapi.yml
  format: yaml
  label: Polygon Snapshots API
  slug: polygon-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-snapshots-api-openapi.yml
- filename: polygon-tickers-api-openapi.yml
  format: yaml
  label: Polygon Tickers API
  slug: polygon-tickers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-tickers-api-openapi.yml
authorization_urls:
- https://auth.massive.com/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Polygon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Polygon publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Polygon API on a user''s behalf.


  Tokens are issued from https://auth.massive.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Polygon
provider_slug: polygon
schemes:
- bearer_methods:
  - header
  flows:
  - authorizationUrl: https://auth.massive.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://auth.massive.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://auth.massive.com/oauth2/token
  name: OAuth2 (remote MCP server)
  registration: https://auth.massive.com/oauth2/register
  resource: https://mcp.massive.com
scope_count: 6
scope_names:
- openid
- offline_access
- account
- profile
- email
- offline
scopes:
- description: OpenID Connect authentication (standard OIDC scope).
  flows: []
  scope: openid
- description: Refresh-token issuance for long-lived MCP sessions (standard OIDC scope).
  flows: []
  scope: offline_access
- description: Massive account access used by the MCP resource server.
  flows: []
  scope: account
- description: Profile claims (standard OIDC scope; advertised by the authorization server only).
  flows: []
  scope: profile
- description: Email claim (standard OIDC scope; advertised by the authorization server only).
  flows: []
  scope: email
- description: Legacy alias for offline_access (advertised by the authorization server only).
  flows: []
  scope: offline
slug: polygon-scopes
source_filename: polygon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://mcp.massive.com/.well-known/oauth-protected-resource + https://auth.massive.com/.well-known/openid-configuration\ndocs: null\nnotes: >-\n  The market-data REST API itself is API-key authenticated and declares no OAuth scopes. This\n  scope surface belongs to Massive's hosted remote MCP server (mcp.massive.com), whose RFC 9728\n  protected-resource metadata names auth.massive.com as the authorization server. Scope\n  descriptions below are the standard OIDC meanings; Massive publishes no per-scope reference page.\nschemes:\n  - name: OAuth2 (remote MCP server)\n    resource: https://mcp.massive.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.massive.com/oauth2/auth\n        tokenUrl: https://auth.massive.com/oauth2/token\n      - flow: clientCredentials\n        tokenUrl: https://auth.massive.com/oauth2/token\n    registration: https://auth.massive.com/oauth2/register\n    bearer_methods:\
  \ [header]\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (standard OIDC scope).\n    sources: [well-known/polygon-oauth-protected-resource.json, well-known/polygon-openid-configuration.json]\n  - scope: offline_access\n    description: Refresh-token issuance for long-lived MCP sessions (standard OIDC scope).\n    sources: [well-known/polygon-oauth-protected-resource.json, well-known/polygon-openid-configuration.json]\n  - scope: account\n    description: Massive account access used by the MCP resource server.\n    sources: [well-known/polygon-oauth-protected-resource.json, well-known/polygon-openid-configuration.json]\n  - scope: profile\n    description: Profile claims (standard OIDC scope; advertised by the authorization server only).\n    sources: [well-known/polygon-openid-configuration.json]\n  - scope: email\n    description: Email claim (standard OIDC scope; advertised by the authorization server only).\n    sources: [well-known/polygon-openid-configuration.json]\n\
  \  - scope: offline\n    description: Legacy alias for offline_access (advertised by the authorization server only).\n    sources: [well-known/polygon-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/scopes/polygon-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Finance
- Fintech
- Market Data
- Stocks
- Options
- Forex
- Crypto
- Indices
- Futures
- WebSockets
- Real-Time
- Historical
- Public APIs
token_urls:
- https://auth.massive.com/oauth2/token
---
