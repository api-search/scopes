---
authorization_urls:
- https://id.livevol.com/connect/authorize
description: OAuth scopes for the Cboe LiveVol platform, taken verbatim from the scopes_supported list in the OpenID Connect discovery document published by the Cboe LiveVol IdentityServer (id.livevol.com). Cboe does not publish a public per-scope reference, so descriptions are only given where the scope maps to a documented API product; all other scopes are listed without interpretation.
docs: https://api.livevol.com/v1/docs/Home/Authentication
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cboe Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cboe Global Markets publishes 42 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cboe Global Markets API on a user''s behalf.


  Tokens are issued from https://id.livevol.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cboe Global Markets
provider_slug: cboe
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://id.livevol.com/connect/token
  - authorizationUrl: https://id.livevol.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://id.livevol.com/connect/token
  name: LiveVolOAuth2
  source: well-known/cboe-openid-configuration.json
scope_count: 42
scope_names:
- openid
- roles
- idmgr
- username
- offline_access
- backtester_v1
- api_v1
- api.theocalc.1
- api.obverror.1
- identity.api.1
- gateway
- quoteserver
- watchlist
- feedback
- statistics
- settings
- reports
- mail
- api
- api.theocalc
- api.obverror
- api.taq
- api.market
- api.backtester
- api.scans.options
- api.scans.underlying
- control_messages
- api.scans.custom
- trial
- api.tradeoptimizer
- api.events
- api.smartmarket
- etrade_api_qa
- api.fundamentals
- api.flexcalc
- api.dataplus
- api.allaccess
- api.marketref
- api.datashop.vendor
- api.livevolman
- livevolman
- api.system_control
scopes:
- description: OpenID Connect authentication
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: roles
- description: ''
  flows: []
  scope: idmgr
- description: ''
  flows: []
  scope: username
- description: Request refresh tokens
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: backtester_v1
- description: ''
  flows: []
  scope: api_v1
- description: ''
  flows: []
  scope: api.theocalc.1
- description: ''
  flows: []
  scope: api.obverror.1
- description: ''
  flows: []
  scope: identity.api.1
- description: ''
  flows: []
  scope: gateway
- description: ''
  flows: []
  scope: quoteserver
- description: ''
  flows: []
  scope: watchlist
- description: ''
  flows: []
  scope: feedback
- description: ''
  flows: []
  scope: statistics
- description: ''
  flows: []
  scope: settings
- description: ''
  flows: []
  scope: reports
- description: ''
  flows: []
  scope: mail
- description: ''
  flows: []
  scope: api
- description: ''
  flows: []
  scope: api.theocalc
- description: ''
  flows: []
  scope: api.obverror
- description: Time and sales (TAQ) endpoints
  flows: []
  scope: api.taq
- description: Market at a Glance endpoints
  flows: []
  scope: api.market
- description: Backtester API
  flows: []
  scope: api.backtester
- description: Option strategy scans
  flows: []
  scope: api.scans.options
- description: Underlying scanner
  flows: []
  scope: api.scans.underlying
- description: ''
  flows: []
  scope: control_messages
- description: Custom scanner
  flows: []
  scope: api.scans.custom
- description: Free-trial access
  flows: []
  scope: trial
- description: Trade optimizer
  flows: []
  scope: api.tradeoptimizer
- description: Events / earnings endpoints
  flows: []
  scope: api.events
- description: Smart Markets API
  flows: []
  scope: api.smartmarket
- description: ''
  flows: []
  scope: etrade_api_qa
- description: ''
  flows: []
  scope: api.fundamentals
- description: ''
  flows: []
  scope: api.flexcalc
- description: ''
  flows: []
  scope: api.dataplus
- description: All Access API suite
  flows: []
  scope: api.allaccess
- description: Market reference data endpoints
  flows: []
  scope: api.marketref
- description: DataShop vendor API
  flows: []
  scope: api.datashop.vendor
- description: ''
  flows: []
  scope: api.livevolman
- description: ''
  flows: []
  scope: livevolman
- description: ''
  flows: []
  scope: api.system_control
slug: cboe-scopes
source_filename: cboe-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://id.livevol.com/.well-known/openid-configuration\ndocs: https://api.livevol.com/v1/docs/Home/Authentication\ndescription: >-\n  OAuth scopes for the Cboe LiveVol platform, taken verbatim from the\n  scopes_supported list in the OpenID Connect discovery document published by\n  the Cboe LiveVol IdentityServer (id.livevol.com). Cboe does not publish a\n  public per-scope reference, so descriptions are only given where the scope\n  maps to a documented API product; all other scopes are listed without\n  interpretation.\nschemes:\n  - name: LiveVolOAuth2\n    source: well-known/cboe-openid-configuration.json\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://id.livevol.com/connect/token\n      - flow: authorizationCode\n        authorizationUrl: https://id.livevol.com/connect/authorize\n        tokenUrl: https://id.livevol.com/connect/token\nscopes:\n  - scope: openid\n    description: OpenID Connect\
  \ authentication\n  - scope: roles\n  - scope: idmgr\n  - scope: username\n  - scope: offline_access\n    description: Request refresh tokens\n  - scope: backtester_v1\n  - scope: api_v1\n  - scope: api.theocalc.1\n  - scope: api.obverror.1\n  - scope: identity.api.1\n  - scope: gateway\n  - scope: quoteserver\n  - scope: watchlist\n  - scope: feedback\n  - scope: statistics\n  - scope: settings\n  - scope: reports\n  - scope: mail\n  - scope: api\n  - scope: api.theocalc\n  - scope: api.obverror\n  - scope: api.taq\n    description: Time and sales (TAQ) endpoints\n  - scope: api.market\n    description: Market at a Glance endpoints\n  - scope: api.backtester\n    description: Backtester API\n  - scope: api.scans.options\n    description: Option strategy scans\n  - scope: api.scans.underlying\n    description: Underlying scanner\n  - scope: control_messages\n  - scope: api.scans.custom\n    description: Custom scanner\n  - scope: trial\n    description: Free-trial access\n  - scope: api.tradeoptimizer\n\
  \    description: Trade optimizer\n  - scope: api.events\n    description: Events / earnings endpoints\n  - scope: api.smartmarket\n    description: Smart Markets API\n  - scope: etrade_api_qa\n  - scope: api.fundamentals\n  - scope: api.flexcalc\n  - scope: api.dataplus\n  - scope: api.allaccess\n    description: All Access API suite\n  - scope: api.marketref\n    description: Market reference data endpoints\n  - scope: api.datashop.vendor\n    description: DataShop vendor API\n  - scope: api.livevolman\n  - scope: livevolman\n  - scope: api.system_control\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cboe/refs/heads/main/scopes/cboe-scopes.yml
summary_line: 42 scopes · clientCredentials/authorizationCode
tags:
- Market Data
- Options
- Equities
- Derivatives
- Volatility
- Financial Markets
- Exchanges
- Trading
token_urls:
- https://id.livevol.com/connect/token
---
