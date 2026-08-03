---
api_specs:
- filename: blockchain.com-exchange-openapi.yml
  format: yaml
  label: Blockchain.com Exchange REST API
  slug: blockchaincom-exchange-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-exchange-openapi.yml
- filename: blockchain.com-pay-partner-api-openapi.yml
  format: yaml
  label: Blockchain.com Pay Partner API
  slug: blockchaincom-pay-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-pay-partner-api-openapi.yml
- filename: blockchain.com-nft-market-api-swagger.json
  format: json
  label: Blockchain.com NFT Market API
  slug: blockchaincom-nft-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-nft-market-api-swagger.json
authorization_urls: []
description: ''
docs: https://docs.blockchain.com/oauth-resources
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Blockchain.Com Scopes
name_suffix: OAuth Scopes
note: Blockchain.com operates an OAuth 2.0 resource gateway that lets a third-party app read a user's custodial wallet data with the user's consent. No OpenAPI declares these scopes and no /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource document is served (both 404 on api.blockchain.info/partner-resource-gateway), so the scopes below are harvested from the published OAuth Resources documentation only. The authorization server endpoints themselves are not publicly documented — partners are onboarded directly by Blockchain.com.
overview: 'Blockchain.com publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Blockchain.com API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blockchain.com
provider_slug: blockchain.com
schemes:
- authorization_url: not publicly documented
  in: header
  name: OAuth2 Bearer
  parameter: Authorization
  resource_server: https://api.blockchain.info/partner-resource-gateway
  source: https://docs.blockchain.com/oauth-resources/oauth-resources.md
  token_type: bearer
  token_url: not publicly documented
  type: oauth2
scope_count: 2
scope_names:
- read_transactions
- read_balance
scopes:
- description: Retrieve the authenticated user's transaction history from their Blockchain.com custodial wallet. Returns at most 30 days of history; types are withdrawal, deposit and trade.
  flows: []
  scope: read_transactions
- description: Retrieve an overview of the authenticated user's account, including per-asset symbol, fiat flag, quantity and current worth.
  flows: []
  scope: read_balance
slug: blockchain.com-scopes
source_filename: blockchain.com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.blockchain.com/oauth-resources/oauth-resources.md\ndocs: https://docs.blockchain.com/oauth-resources\nnote: >-\n  Blockchain.com operates an OAuth 2.0 resource gateway that lets a third-party\n  app read a user's custodial wallet data with the user's consent. No OpenAPI\n  declares these scopes and no /.well-known/oauth-authorization-server or\n  /.well-known/oauth-protected-resource document is served (both 404 on\n  api.blockchain.info/partner-resource-gateway), so the scopes below are\n  harvested from the published OAuth Resources documentation only. The\n  authorization server endpoints themselves are not publicly documented —\n  partners are onboarded directly by Blockchain.com.\nschemes:\n- name: OAuth2 Bearer\n  type: oauth2\n  token_type: bearer\n  in: header\n  parameter: Authorization\n  resource_server: https://api.blockchain.info/partner-resource-gateway\n  authorization_url: not publicly documented\n\
  \  token_url: not publicly documented\n  source: https://docs.blockchain.com/oauth-resources/oauth-resources.md\nscopes:\n- scope: read_transactions\n  description: >-\n    Retrieve the authenticated user's transaction history from their\n    Blockchain.com custodial wallet. Returns at most 30 days of history; types\n    are withdrawal, deposit and trade.\n  operation: GET /v1/transactions\n  sources: [https://docs.blockchain.com/oauth-resources/oauth-resources.md]\n- scope: read_balance\n  description: >-\n    Retrieve an overview of the authenticated user's account, including per-asset\n    symbol, fiat flag, quantity and current worth.\n  operation: GET /v1/balances\n  sources: [https://docs.blockchain.com/oauth-resources/oauth-resources.md]\nx-evidence:\n  fetched: '2026-08-02'\n  probes:\n  - url: https://api.blockchain.info/partner-resource-gateway/v1/balances\n    http_status: 401\n    note: endpoint is live and rejects anonymous requests\n  - url: https://api.blockchain.info/partner-resource-gateway/.well-known/oauth-authorization-server\n\
  \    http_status: 404\n  - url: https://api.blockchain.info/partner-resource-gateway/.well-known/oauth-protected-resource\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/scopes/blockchain.com-scopes.yml
summary_line: 2 scopes
tags:
- cryptocurrency
- bitcoin
- blockchain
- exchange
- trading
- market-data
- payments
- on-ramp
- wallet
- block-explorer
- fintech
- webhooks
token_urls: []
---
