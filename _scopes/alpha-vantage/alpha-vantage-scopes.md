---
api_specs:
- filename: alpha-vantage-stock-time-series-api-openapi.yml
  format: yaml
  label: Alpha Vantage Stock Time Series API
  slug: alpha-vantage-stock-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/openapi/alpha-vantage-stock-time-series-api-openapi.yml
authorization_urls:
- https://mcp.alphavantage.co/authorize
description: ''
docs: https://mcp.alphavantage.co/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Alpha Vantage Scopes
name_suffix: OAuth Scopes
note: The core Alpha Vantage REST API authenticates with an apikey query parameter and has no OAuth scope surface. OAuth applies to the official MCP server (mcp.alphavantage.co), which fronts the API key with an OAuth 2.0 authorization-code + PKCE flow and a single read scope.
overview: 'Alpha Vantage publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alpha Vantage API on a user''s behalf.


  Tokens are issued from https://mcp.alphavantage.co/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schemes:
- flows:
  - authorizationUrl: https://mcp.alphavantage.co/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://mcp.alphavantage.co/register
    tokenUrl: https://mcp.alphavantage.co/token
  name: AlphaVantageMCPOAuth
  source: well-known/alpha-vantage-mcp-oauth-authorization-server.json
scope_count: 1
scope_names:
- alphavantage:read
scopes:
- description: Read access to Alpha Vantage market data through the MCP server (the entire surface is read-only)
  flows:
  - authorizationCode
  scope: alphavantage:read
slug: alpha-vantage-scopes
source_filename: alpha-vantage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://mcp.alphavantage.co/.well-known/oauth-authorization-server\ndocs: https://mcp.alphavantage.co/\nnote: >-\n  The core Alpha Vantage REST API authenticates with an apikey query parameter and has no OAuth scope\n  surface. OAuth applies to the official MCP server (mcp.alphavantage.co), which fronts the API key with\n  an OAuth 2.0 authorization-code + PKCE flow and a single read scope.\nschemes:\n  - name: AlphaVantageMCPOAuth\n    source: well-known/alpha-vantage-mcp-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.alphavantage.co/authorize\n        tokenUrl: https://mcp.alphavantage.co/token\n        registrationUrl: https://mcp.alphavantage.co/register\n        pkce: S256\n        grant_types: [authorization_code, refresh_token]\nscopes:\n  - scope: alphavantage:read\n    description: Read access to Alpha Vantage market data through the MCP server (the\
  \ entire surface is read-only)\n    flows: [authorizationCode]\n    sources:\n      - well-known/alpha-vantage-mcp-oauth-authorization-server.json\n      - well-known/alpha-vantage-mcp-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/scopes/alpha-vantage-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Fintech
- Market Data
- Stocks
- FX
- Crypto
- Commodities
- Economic Indicators
- Technical Indicators
- Fundamentals
- News
- Sentiment
- Free
token_urls:
- https://mcp.alphavantage.co/token
---
