---
api_specs:
- filename: alpaca-trading-api-openapi.yml
  format: yaml
  label: Alpaca Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-trading-api-openapi.yml
- filename: alpaca-oauth-api-openapi.yml
  format: yaml
  label: Alpaca OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-oauth-api-openapi.yml
- filename: alpaca-accounts-api-openapi.yml
  format: yaml
  label: Alpaca Accounts API
  slug: alpaca-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-accounts-api-openapi.yml
- filename: alpaca-assets-api-openapi.yml
  format: yaml
  label: Alpaca Assets API
  slug: alpaca-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-assets-api-openapi.yml
- filename: alpaca-calendar-api-openapi.yml
  format: yaml
  label: Alpaca Calendar API
  slug: alpaca-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-calendar-api-openapi.yml
- filename: alpaca-clock-api-openapi.yml
  format: yaml
  label: Alpaca Clock API
  slug: alpaca-clock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-clock-api-openapi.yml
- filename: alpaca-corporate-actions-api-openapi.yml
  format: yaml
  label: Alpaca Corporate Actions API
  slug: alpaca-corporate-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-corporate-actions-api-openapi.yml
- filename: alpaca-crypto-pricing-data-api-api-openapi.yml
  format: yaml
  label: Alpaca Crypto Pricing Data API API
  slug: alpaca-crypto-pricing-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-crypto-pricing-data-api-api-openapi.yml
- filename: alpaca-documents-api-openapi.yml
  format: yaml
  label: Alpaca Documents API
  slug: alpaca-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-documents-api-openapi.yml
- filename: alpaca-events-api-openapi.yml
  format: yaml
  label: Alpaca Events API
  slug: alpaca-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-events-api-openapi.yml
- filename: alpaca-funding-api-openapi.yml
  format: yaml
  label: Alpaca Funding API
  slug: alpaca-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-funding-api-openapi.yml
- filename: alpaca-journals-api-openapi.yml
  format: yaml
  label: Alpaca Journals API
  slug: alpaca-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-journals-api-openapi.yml
- filename: alpaca-logo-api-openapi.yml
  format: yaml
  label: Alpaca Logo API
  slug: alpaca-logo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-logo-api-openapi.yml
- filename: alpaca-news-api-openapi.yml
  format: yaml
  label: Alpaca News API
  slug: alpaca-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-news-api-openapi.yml
- filename: alpaca-screener-api-openapi.yml
  format: yaml
  label: Alpaca Screener API
  slug: alpaca-screener-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-screener-api-openapi.yml
- filename: alpaca-stock-pricing-data-api-api-openapi.yml
  format: yaml
  label: Alpaca Stock Pricing Data API API
  slug: alpaca-stock-pricing-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-stock-pricing-data-api-api-openapi.yml
- filename: alpaca-watchlist-api-openapi.yml
  format: yaml
  label: Alpaca Watchlist API
  slug: alpaca-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-watchlist-api-openapi.yml
authorization_urls:
- https://app.alpaca.markets/oauth/authorize
- https://authx.alpaca.markets/v1/oauth2/authorize
description: OAuth 2.0 scopes for Alpaca Connect (third-party apps acting for Alpaca users on the Trading and Market Data APIs). Read-only endpoint access is assumed by default when no scope is requested. The harvested OpenAPI declares only apiKey/basic schemes, so this scope surface comes from the published OAuth docs, plus the RFC 8414 metadata of the authx authorization server that fronts the hosted Broker MCP Server.
docs: https://docs.alpaca.markets/docs/using-oauth2-and-trading-api
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Alpaca Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Alpaca publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alpaca API on a user''s behalf.


  Tokens are issued from https://api.alpaca.markets/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alpaca
provider_slug: alpaca
schemes:
- flows:
  - authorizationUrl: https://app.alpaca.markets/oauth/authorize
    flow: authorizationCode
    notes:
    - Optional env parameter (live | paper); both prompted if unspecified.
    - scope is a space-delimited list; read-only access is the default grant.
    tokenUrl: https://api.alpaca.markets/oauth/token
  name: Alpaca Connect OAuth 2.0
  source: https://docs.alpaca.markets/docs/using-oauth2-and-trading-api
- flows:
  - authorizationUrl: https://authx.alpaca.markets/v1/oauth2/authorize
    flow: authorizationCode
    notes:
    - PKCE (S256) supported; grants also include client_credentials, jwt-bearer, refresh_token.
    - The protected-resource metadata for /mcp advertises scopes_supported [] (no public scope registry).
    tokenUrl: https://authx.alpaca.markets/v1/oauth2/token
  metadata: well-known/alpaca-authx-oauth-authorization-server.json
  name: authx (Broker MCP authorization server)
  source: https://authx.alpaca.markets/v1/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- account:write
- trading
- data
- (default / no scope)
scopes:
- description: Write access for account configurations and watchlists.
  flows:
  - authorizationCode
  scope: account:write
- description: Place, cancel or modify orders.
  flows:
  - authorizationCode
  scope: trading
- description: Access to the Data API.
  flows:
  - authorizationCode
  scope: data
- description: Read-only endpoint access is assumed by default.
  flows:
  - authorizationCode
  scope: (default / no scope)
slug: alpaca-scopes
source_filename: alpaca-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://docs.alpaca.markets/us/docs/using-oauth2-and-trading-api.md\ndocs: https://docs.alpaca.markets/docs/using-oauth2-and-trading-api\ndescription: >-\n  OAuth 2.0 scopes for Alpaca Connect (third-party apps acting for Alpaca users on the Trading and\n  Market Data APIs). Read-only endpoint access is assumed by default when no scope is requested.\n  The harvested OpenAPI declares only apiKey/basic schemes, so this scope surface comes from the\n  published OAuth docs, plus the RFC 8414 metadata of the authx authorization server that fronts\n  the hosted Broker MCP Server.\nschemes:\n  - name: Alpaca Connect OAuth 2.0\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.alpaca.markets/oauth/authorize\n        tokenUrl: https://api.alpaca.markets/oauth/token\n        notes:\n          - Optional env parameter (live | paper); both prompted if unspecified.\n          - scope is a space-delimited\
  \ list; read-only access is the default grant.\n    source: https://docs.alpaca.markets/docs/using-oauth2-and-trading-api\n  - name: authx (Broker MCP authorization server)\n    metadata: well-known/alpaca-authx-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://authx.alpaca.markets/v1/oauth2/authorize\n        tokenUrl: https://authx.alpaca.markets/v1/oauth2/token\n        notes:\n          - PKCE (S256) supported; grants also include client_credentials, jwt-bearer, refresh_token.\n          - The protected-resource metadata for /mcp advertises scopes_supported [] (no public scope registry).\n    source: https://authx.alpaca.markets/v1/.well-known/oauth-authorization-server\nscopes:\n  - scope: account:write\n    description: Write access for account configurations and watchlists.\n    flows: [authorizationCode]\n  - scope: trading\n    description: Place, cancel or modify orders.\n    flows: [authorizationCode]\n  - scope:\
  \ data\n    description: Access to the Data API.\n    flows: [authorizationCode]\n  - scope: (default / no scope)\n    description: Read-only endpoint access is assumed by default.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/scopes/alpaca-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Fintech
- Trading
- Stocks
- Crypto
- Brokerage
- Market Data
- Options
token_urls:
- https://api.alpaca.markets/oauth/token
- https://authx.alpaca.markets/v1/oauth2/token
---
