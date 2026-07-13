---
api_specs:
- filename: tradestation-api-openapi.yml
  format: yaml
  label: TradeStation API
  slug: tradestation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/openapi/tradestation-api-openapi.yml
- filename: tradestation-streaming-asyncapi.yml
  format: yaml
  label: TradeStation Streaming API
  slug: tradestation-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/asyncapi/tradestation-streaming-asyncapi.yml
authorization_urls:
- https://signin.tradestation.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Tradestation Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TradeStation publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TradeStation API on a user''s behalf.


  Tokens are issued from https://signin.tradestation.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TradeStation
provider_slug: tradestation
schemes:
- description: OAuth 2.0 authorization code flow for accessing TradeStation API resources. Requires user authorization and supports token refresh.
  flows:
  - authorizationUrl: https://signin.tradestation.com/authorize
    flow: authorizationCode
    tokenUrl: https://signin.tradestation.com/oauth/token
  name: oauth2AuthCode
  source: openapi/tradestation-api-openapi.yml
scope_count: 3
scope_names:
- marketdata
- readaccount
- trade
scopes:
- description: Access to market data endpoints
  flows:
  - authorizationCode
  scope: marketdata
- description: Read access to account information
  flows:
  - authorizationCode
  scope: readaccount
- description: Access to order placement and management
  flows:
  - authorizationCode
  scope: trade
slug: tradestation-scopes
source_filename: tradestation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tradestation-api-openapi.yml\nschemes:\n- name: oauth2AuthCode\n  source: openapi/tradestation-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://signin.tradestation.com/authorize\n    tokenUrl: https://signin.tradestation.com/oauth/token\n  description: OAuth 2.0 authorization code flow for accessing TradeStation API resources. Requires\n    user authorization and supports token refresh.\nscopes:\n- scope: marketdata\n  description: Access to market data endpoints\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tradestation-api-openapi.yml\n- scope: readaccount\n  description: Read access to account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tradestation-api-openapi.yml\n- scope: trade\n  description: Access to order placement and management\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tradestation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/scopes/tradestation-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Brokerage
- Cryptocurrency
- Finance
- Futures
- Market Data
- Options
- Stocks
- Trading
token_urls:
- https://signin.tradestation.com/oauth/token
---
