---
authorization_urls:
- https://coinvest.liquid.trade/oauth/authorize
description: ''
docs: https://www.liquid.trade/coinvest-docs
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Liquid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Liquid publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Liquid API on a user''s behalf.


  Tokens are issued from https://coinvest.liquid.trade/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Liquid
provider_slug: liquid
schemes:
- flows:
  - authorizationUrl: https://coinvest.liquid.trade/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://coinvest.liquid.trade/oauth/token
  name: CoInvestOAuth
  source: https://coinvest.liquid.trade/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- read
- trade
scopes:
- description: Market data, portfolio and account state — live prices, funding, open interest, positioning, news, leaderboards, prediction markets, balances, open positions and resting orders.
  flows:
  - authorizationCode
  scope: read
- description: Placing and managing orders — opening long/short positions, market and limit orders, TP/SL attachment and modification, leverage changes, position closes, order cancels and prediction-market orders. Always behind an explicit human Confirm tap in the client.
  flows:
  - authorizationCode
  scope: trade
slug: liquid-scopes
source_filename: liquid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://coinvest.liquid.trade/.well-known/oauth-protected-resource\ndocs: https://www.liquid.trade/coinvest-docs\nnotes: >-\n  Not derived from OpenAPI — Liquid publishes no spec. Scopes are taken verbatim from the live\n  scopes_supported arrays in both the RFC 9728 protected-resource metadata and the RFC 8414\n  authorization-server metadata on coinvest.liquid.trade, with descriptions from the provider's\n  \"Signing in & permissions\" documentation.\nschemes:\n- name: CoInvestOAuth\n  source: https://coinvest.liquid.trade/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coinvest.liquid.trade/oauth/authorize\n    tokenUrl: https://coinvest.liquid.trade/oauth/token\nscopes:\n- scope: read\n  description: Market data, portfolio and account state — live prices, funding, open interest, positioning,\n    news, leaderboards, prediction markets, balances, open positions\
  \ and resting orders.\n  flows:\n  - authorizationCode\n  consequence: read\n  sources:\n  - https://coinvest.liquid.trade/.well-known/oauth-protected-resource\n  - https://www.liquid.trade/coinvest-docs\n- scope: trade\n  description: Placing and managing orders — opening long/short positions, market and limit orders, TP/SL\n    attachment and modification, leverage changes, position closes, order cancels and prediction-market\n    orders. Always behind an explicit human Confirm tap in the client.\n  flows:\n  - authorizationCode\n  consequence: financial\n  human_in_the_loop: required\n  sources:\n  - https://coinvest.liquid.trade/.well-known/oauth-protected-resource\n  - https://www.liquid.trade/coinvest-docs\nexcluded_by_design:\n- capability: withdraw or transfer funds\n  reason: No scope exists for it; the documentation states the connection can never move money out of\n    the account.\n- capability: change account settings\n  reason: No scope exists for it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid/refs/heads/main/scopes/liquid-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Crypto Defi
- Trading
- Perpetual Futures
- Prediction Markets
- Fintech
- MCP
- Agentic Commerce
- OAuth
token_urls:
- https://coinvest.liquid.trade/oauth/token
---
