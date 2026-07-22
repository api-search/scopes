---
api_specs:
- filename: safello-institutional-openapi.json
  format: json
  label: Safello Institutional API
  slug: safello-institutional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/openapi/safello-institutional-openapi.json
- filename: safello-app-openapi.json
  format: json
  label: Safello App API
  slug: safello-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/openapi/safello-app-openapi.json
authorization_urls: []
description: ''
docs: https://safello.github.io/safello-api/docs/getting-started/tokens
flows:
- urn:safello:params:oauth:grant-type:bankid
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Safello Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Safello publishes 8 OAuth 2.0 scopes via the urn:safello:params:oauth:grant-type:bankid, clientCredentials, and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Safello API on a user''s behalf.


  Tokens are issued from /oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Safello
provider_slug: safello
schemes:
- flows:
  - flow: urn:safello:params:oauth:grant-type:bankid
    tokenUrl: /oauth2/token
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  - flow: authorizationCode
    tokenUrl: /oauth2/token
  name: OAuth2
  source: openapi/safello-institutional-openapi.json
scope_count: 8
scope_names:
- account.bank-account
- account.bank-account:read
- account.base
- account.base:read
- market
- order
- order:read
- wallet
scopes:
- description: View and modify users bank accounts.
  flows:
  - authorizationCode
  - urn:safello:params:oauth:grant-type:bankid
  scope: account.bank-account
- description: View users bank accounts.
  flows:
  - authorizationCode
  - urn:safello:params:oauth:grant-type:bankid
  scope: account.bank-account:read
- description: View and modify base information of accounts.
  flows:
  - authorizationCode
  - urn:safello:params:oauth:grant-type:bankid
  scope: account.base
- description: View base information of accounts.
  flows:
  - authorizationCode
  - urn:safello:params:oauth:grant-type:bankid
  scope: account.base:read
- description: View market data.
  flows:
  - authorizationCode
  - clientCredentials
  - urn:safello:params:oauth:grant-type:bankid
  scope: market
- description: View and create orders.
  flows:
  - authorizationCode
  - urn:safello:params:oauth:grant-type:bankid
  scope: order
- description: View orders.
  flows:
  - authorizationCode
  - urn:safello:params:oauth:grant-type:bankid
  scope: order:read
- description: View and modify wallet.
  flows:
  - authorizationCode
  - urn:safello:params:oauth:grant-type:bankid
  scope: wallet
slug: safello-scopes
source_filename: safello-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/safello-institutional-openapi.json\ndocs: https://safello.github.io/safello-api/docs/getting-started/tokens\nauthorization_server_metadata: https://api.safello.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: openapi/safello-institutional-openapi.json\n  flows:\n  - flow: urn:safello:params:oauth:grant-type:bankid\n    tokenUrl: /oauth2/token\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n  - flow: authorizationCode\n    tokenUrl: /oauth2/token\nscopes:\n- scope: account.bank-account\n  description: View and modify users bank accounts.\n  flows:\n  - authorizationCode\n  - urn:safello:params:oauth:grant-type:bankid\n  sources:\n  - openapi/safello-institutional-openapi.json\n- scope: account.bank-account:read\n  description: View users bank accounts.\n  flows:\n  - authorizationCode\n  - urn:safello:params:oauth:grant-type:bankid\n  sources:\n  - openapi/safello-institutional-openapi.json\n\
  - scope: account.base\n  description: View and modify base information of accounts.\n  flows:\n  - authorizationCode\n  - urn:safello:params:oauth:grant-type:bankid\n  sources:\n  - openapi/safello-institutional-openapi.json\n- scope: account.base:read\n  description: View base information of accounts.\n  flows:\n  - authorizationCode\n  - urn:safello:params:oauth:grant-type:bankid\n  sources:\n  - openapi/safello-institutional-openapi.json\n- scope: market\n  description: View market data.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - urn:safello:params:oauth:grant-type:bankid\n  sources:\n  - openapi/safello-institutional-openapi.json\n- scope: order\n  description: View and create orders.\n  flows:\n  - authorizationCode\n  - urn:safello:params:oauth:grant-type:bankid\n  sources:\n  - openapi/safello-institutional-openapi.json\n- scope: order:read\n  description: View orders.\n  flows:\n  - authorizationCode\n  - urn:safello:params:oauth:grant-type:bankid\n  sources:\n\
  \  - openapi/safello-institutional-openapi.json\n- scope: wallet\n  description: View and modify wallet.\n  flows:\n  - authorizationCode\n  - urn:safello:params:oauth:grant-type:bankid\n  sources:\n  - openapi/safello-institutional-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/scopes/safello-scopes.yml
summary_line: 8 scopes · urn:safello:params:oauth:grant-type:bankid/clientCredentials/authorizationCode
tags:
- Company
- Fintech
- Cryptocurrency
- Bitcoin
- Brokerage
- Payments
- Sweden
- Trading
- KYC
- BankID
token_urls:
- /oauth2/token
---
