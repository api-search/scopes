---
api_specs:
- filename: coinlist-documentsubmissions-api-openapi.yml
  format: yaml
  label: CoinList DocumentSubmissions API
  slug: coinlist-documentsubmissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-documentsubmissions-api-openapi.yml
- filename: coinlist-kyc-api-openapi.yml
  format: yaml
  label: CoinList KYC API
  slug: coinlist-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-kyc-api-openapi.yml
- filename: coinlist-oauth-api-openapi.yml
  format: yaml
  label: CoinList OAuth API
  slug: coinlist-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-oauth-api-openapi.yml
- filename: coinlist-offers-api-openapi.yml
  format: yaml
  label: CoinList Offers API
  slug: coinlist-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-offers-api-openapi.yml
- filename: coinlist-participations-api-openapi.yml
  format: yaml
  label: CoinList Participations API
  slug: coinlist-participations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-participations-api-openapi.yml
- filename: coinlist-pii-api-openapi.yml
  format: yaml
  label: CoinList Pii API
  slug: coinlist-pii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-pii-api-openapi.yml
- filename: coinlist-requirements-api-openapi.yml
  format: yaml
  label: CoinList Requirements API
  slug: coinlist-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-requirements-api-openapi.yml
- filename: coinlist-swap-api-openapi.yml
  format: yaml
  label: CoinList Swap API
  slug: coinlist-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-swap-api-openapi.yml
- filename: coinlist-token-api-openapi.yml
  format: yaml
  label: CoinList Token API
  slug: coinlist-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-token-api-openapi.yml
- filename: coinlist-wallet-api-openapi.yml
  format: yaml
  label: CoinList Wallet API
  slug: coinlist-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-wallet-api-openapi.yml
- filename: coinlist-wallet-ownership-api-openapi.yml
  format: yaml
  label: CoinList Wallet Ownership API
  slug: coinlist-wallet-ownership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-wallet-ownership-api-openapi.yml
authorization_urls:
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Coinlist Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CoinList uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoinList
provider_slug: coinlist
schemes:
- description: OAuth 2.0 authorization and token endpoints
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/coinlist-passage-openapi-original.json
scope_count: 0
scope_names: []
scopes: []
slug: coinlist-scopes
source_filename: coinlist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/coinlist-passage-openapi-original.json\nschemes:\n- name: OAuth2\n  source: openapi/coinlist-passage-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: OAuth 2.0 authorization and token endpoints\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/scopes/coinlist-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Fintech
- Cryptocurrency
- Token Sales
- Tokenized Equities
- KYC
- Authentication
- Blockchain
- Digital Assets
- Embedded Finance
token_urls:
- /oauth/token
---
