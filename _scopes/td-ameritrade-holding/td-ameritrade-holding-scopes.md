---
api_specs:
- filename: td-ameritrade-accounts-trading-openapi.yml
  format: yaml
  label: TD Ameritrade Accounts and Trading API
  slug: accounts-and-trading
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-accounts-trading-openapi.yml
authorization_urls:
- https://auth.tdameritrade.com/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Td Ameritrade Holding Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TD Ameritrade Holding publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TD Ameritrade Holding API on a user''s behalf.


  Tokens are issued from https://api.tdameritrade.com/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TD Ameritrade Holding
provider_slug: td-ameritrade-holding
schemes:
- description: TD Ameritrade uses OAuth 2.0 token-based authentication
  flows:
  - authorizationUrl: https://auth.tdameritrade.com/auth
    flow: authorizationCode
    tokenUrl: https://api.tdameritrade.com/v1/oauth2/token
  name: OAuth2
  source: openapi/td-ameritrade-accounts-trading-openapi.yml
scope_count: 3
scope_names:
- AccountAccess
- MoveMoney
- PlaceTrades
scopes:
- description: Access account information
  flows:
  - authorizationCode
  scope: AccountAccess
- description: Transfer funds between accounts
  flows:
  - authorizationCode
  scope: MoveMoney
- description: Place trades on behalf of the user
  flows:
  - authorizationCode
  scope: PlaceTrades
slug: td-ameritrade-holding-scopes
source_filename: td-ameritrade-holding-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/td-ameritrade-accounts-trading-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/td-ameritrade-accounts-trading-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tdameritrade.com/auth\n    tokenUrl: https://api.tdameritrade.com/v1/oauth2/token\n  description: TD Ameritrade uses OAuth 2.0 token-based authentication\nscopes:\n- scope: AccountAccess\n  description: Access account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-ameritrade-accounts-trading-openapi.yml\n- scope: MoveMoney\n  description: Transfer funds between accounts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-ameritrade-accounts-trading-openapi.yml\n- scope: PlaceTrades\n  description: Place trades on behalf of the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-ameritrade-accounts-trading-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/scopes/td-ameritrade-holding-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Finance
- Brokerage
- Trading
- Market Data
- Investment
- Charles Schwab
- Deprecated
- Fortune 1000
token_urls:
- https://api.tdameritrade.com/v1/oauth2/token
---
