---
api_specs:
- filename: tradier-asyncapi.yml
  format: yaml
  label: Tradier Streaming API
  slug: streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/asyncapi/tradier-asyncapi.yml
- filename: tradier-accounts-api-openapi.yml
  format: yaml
  label: Tradier Accounts API
  slug: tradier-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-accounts-api-openapi.yml
- filename: tradier-market-data-api-openapi.yml
  format: yaml
  label: Tradier Market Data API
  slug: tradier-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-market-data-api-openapi.yml
- filename: tradier-options-api-openapi.yml
  format: yaml
  label: Tradier Options API
  slug: tradier-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-options-api-openapi.yml
- filename: tradier-streaming-api-openapi.yml
  format: yaml
  label: Tradier Streaming API
  slug: tradier-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-streaming-api-openapi.yml
- filename: tradier-trading-api-openapi.yml
  format: yaml
  label: Tradier Trading API
  slug: tradier-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-trading-api-openapi.yml
- filename: tradier-user-api-openapi.yml
  format: yaml
  label: Tradier User API
  slug: tradier-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-user-api-openapi.yml
- filename: tradier-watchlists-api-openapi.yml
  format: yaml
  label: Tradier Watchlists API
  slug: tradier-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-watchlists-api-openapi.yml
authorization_urls:
- https://api.tradier.com/v1/oauth/authorize
description: ''
docs: https://docs.tradier.com/docs/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tradier Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tradier publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tradier API on a user''s behalf.


  Tokens are issued from https://api.tradier.com/v1/oauth/accesstoken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tradier
provider_slug: tradier
schemes:
- flows:
  - authorizationUrl: https://api.tradier.com/v1/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.tradier.com/v1/oauth/refreshtoken
    tokenUrl: https://api.tradier.com/v1/oauth/accesstoken
  name: OAuth2
  source: https://docs.tradier.com/docs/authentication
  token_lifespans:
    access_token: 24 hours
    authorization_code: 10 minutes
    refresh_token: does not expire (approved partners only)
scope_count: 5
scope_names:
- read
- write
- market
- trade
- stream
scopes:
- description: Read access to account information, positions, and market data.
  flows:
  - authorizationCode
  scope: read
- description: Write access to account data (does not include placing or updating trades).
  flows:
  - authorizationCode
  scope: write
- description: Access market data (does not include streaming).
  flows:
  - authorizationCode
  scope: market
- description: Permission to place and manage trades.
  flows:
  - authorizationCode
  scope: trade
- description: Access to real-time streaming data.
  flows:
  - authorizationCode
  scope: stream
slug: tradier-scopes
source_filename: tradier-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://docs.tradier.com/docs/authentication\ndocs: https://docs.tradier.com/docs/authentication\nnotes: >-\n  The OpenAPI models auth as a plain HTTP bearer scheme, so the derive pass found\n  no oauth2 flows; the scopes below come from Tradier's OAuth documentation.\n  OAuth (authorization-code flow) is for Tradier partners building public apps;\n  individual developers use a personal API token without scopes. The separate\n  MCP-server authorization server (p-be-auth.tradier.com) advertises its own\n  scopes: openid, mcp, claudeai (see well-known/tradier-mcp-oauth-authorization-server.json).\nschemes:\n  - name: OAuth2\n    source: https://docs.tradier.com/docs/authentication\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.tradier.com/v1/oauth/authorize\n        tokenUrl: https://api.tradier.com/v1/oauth/accesstoken\n        refreshUrl: https://api.tradier.com/v1/oauth/refreshtoken\n \
  \   token_lifespans:\n      authorization_code: 10 minutes\n      access_token: 24 hours\n      refresh_token: does not expire (approved partners only)\nscopes:\n  - scope: read\n    description: Read access to account information, positions, and market data.\n    flows: [authorizationCode]\n  - scope: write\n    description: Write access to account data (does not include placing or updating trades).\n    flows: [authorizationCode]\n  - scope: market\n    description: Access market data (does not include streaming).\n    flows: [authorizationCode]\n  - scope: trade\n    description: Permission to place and manage trades.\n    flows: [authorizationCode]\n  - scope: stream\n    description: Access to real-time streaming data.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/scopes/tradier-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Fintech
- Trading
- Stocks
- Options
- Brokerage
- Streaming
token_urls:
- https://api.tradier.com/v1/oauth/accesstoken
---
