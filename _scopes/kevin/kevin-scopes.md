---
authorization_urls:
- https://api.kevin.eu/platform/auth
description: ''
docs: https://developer.kevin.eu/platform/account-information
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Kevin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kevin. publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kevin. API on a user''s behalf.


  Tokens are issued from https://api.kevin.eu/platform/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kevin.
provider_slug: kevin
schemes:
- flows:
  - authorizationUrl: https://api.kevin.eu/platform/auth
    flow: authorizationCode
    tokenUrl: https://api.kevin.eu/platform/auth/token
  name: UserBearerToken
  source: '@kevin.eu/kevin-platform-client'
scope_count: 2
scope_names:
- payments
- accounts_basic
scopes:
- description: Initiate and manage payments on behalf of the authorizing user.
  flows:
  - authorizationCode
  scope: payments
- description: Read basic account information (Account Information Service).
  flows:
  - authorizationCode
  scope: accounts_basic
slug: kevin-scopes
source_filename: kevin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.npmjs.com/package/@kevin.eu/kevin-platform-client (official SDK, startAuth example)\ndocs: https://developer.kevin.eu/platform/account-information\nschemes:\n- name: UserBearerToken\n  source: \"@kevin.eu/kevin-platform-client\"\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kevin.eu/platform/auth\n    tokenUrl: https://api.kevin.eu/platform/auth/token\nscopes:\n- scope: payments\n  description: Initiate and manage payments on behalf of the authorizing user.\n  flows: [authorizationCode]\n  sources: [\"@kevin.eu/kevin-platform-client\"]\n- scope: accounts_basic\n  description: Read basic account information (Account Information Service).\n  flows: [authorizationCode]\n  sources: [\"@kevin.eu/kevin-platform-client\"]\nnotes: >-\n  Scopes `payments` and `accounts_basic` are the values documented in the\n  official SDK `startAuth` example. kevin.'s AIS surface (getAccounts,\n  getAccount,\
  \ getAccountTransactions, getAccountBalance) implies additional\n  account-detail/transaction/balance scopes, but only the two verbatim SDK\n  scopes are recorded here to avoid fabrication. Authorization/token URLs are the\n  documented api.kevin.eu platform host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevin/refs/heads/main/scopes/kevin-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Payments
- Open Banking
- Account to Account
- PSD2
- Fintech
- Bank Payments
- Payment Initiation
- Account Information
- Europe
token_urls:
- https://api.kevin.eu/platform/auth/token
---
