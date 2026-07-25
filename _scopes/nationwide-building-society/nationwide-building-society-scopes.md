---
api_specs:
- filename: obie-open-data-atm-locator-openapi.json
  format: json
  label: Nationwide ATM Locator API
  slug: nationwide-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/openapi/obie-open-data-atm-locator-openapi.json
- filename: obie-open-data-branch-locator-openapi.json
  format: json
  label: Nationwide Branch Locator API
  slug: nationwide-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/openapi/obie-open-data-branch-locator-openapi.json
- filename: obie-open-data-personal-current-accounts-openapi.json
  format: json
  label: Nationwide Personal Current Accounts API
  slug: nationwide-personal-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/openapi/obie-open-data-personal-current-accounts-openapi.json
authorization_urls: []
description: ''
docs: https://openbankinguk.github.io/read-write-api-site3/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Nationwide Building Society Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nationwide Building Society publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nationwide Building Society API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nationwide Building Society
provider_slug: nationwide-building-society
schemes:
- flows:
  - flow: authorizationCode
  - flow: clientCredentials
  name: OAuth2
scope_count: 4
scope_names:
- openid
- accounts
- payments
- fundsconfirmations
scopes:
- description: OpenID Connect authentication; returns an id_token binding the PSU authorisation to the consent intent.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the Account and Transaction Information (AIS) APIs — accounts, balances, transactions, beneficiaries, standing orders, direct debits, scheduled payments, statements, parties and products, subject to an authorised account-access-consent.
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: Access to the Payment Initiation (PIS) and Variable Recurring Payments (VRP) APIs — create and authorise domestic/international payment-order consents and VRP consents, then submit payment orders.
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: Access to the Confirmation of Funds (CBPII) API — create a funds-confirmation-consent and check whether funds are available on an account.
  flows:
  - authorizationCode
  - clientCredentials
  scope: fundsconfirmations
slug: nationwide-building-society-scopes
source_filename: nationwide-building-society-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.nationwide.co.uk/open-banking\nstandard: OBIE Read/Write API Standard (UK Open Banking)\ndocs: https://openbankinguk.github.io/read-write-api-site3/\nnotes: >-\n  OAuth 2.0 scopes in UK Open Banking are coarse-grained and fixed at client\n  registration. Fine-grained permissions are expressed through OBIE consent\n  \"intents\" (account-access-consent, payment-order consents,\n  funds-confirmation-consent) that the PSU authorises, not through additional\n  scopes. Only the four canonical OBIE scopes below apply to Nationwide's\n  Read/Write surface. The Open Data APIs use no scopes (public).\nschemes:\n- name: OAuth2\n  flows:\n  - flow: authorizationCode\n  - flow: clientCredentials\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an id_token binding the PSU authorisation to the consent intent.\n  flows: [authorizationCode]\n- scope: accounts\n  description: >-\n    Access\
  \ to the Account and Transaction Information (AIS) APIs — accounts,\n    balances, transactions, beneficiaries, standing orders, direct debits,\n    scheduled payments, statements, parties and products, subject to an\n    authorised account-access-consent.\n  flows: [authorizationCode, clientCredentials]\n  apis: [Nationwide Account and Transaction Information API (AIS)]\n- scope: payments\n  description: >-\n    Access to the Payment Initiation (PIS) and Variable Recurring Payments (VRP)\n    APIs — create and authorise domestic/international payment-order consents and\n    VRP consents, then submit payment orders.\n  flows: [authorizationCode, clientCredentials]\n  apis:\n  - Nationwide Payment Initiation API (PIS)\n  - Nationwide Variable Recurring Payments API (VRP)\n- scope: fundsconfirmations\n  description: >-\n    Access to the Confirmation of Funds (CBPII) API — create a\n    funds-confirmation-consent and check whether funds are available on an account.\n  flows: [authorizationCode,\
  \ clientCredentials]\n  apis: [Nationwide Confirmation of Funds API (CBPII)]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nationwide-building-society/refs/heads/main/scopes/nationwide-building-society-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Financial Services
- Banking
- Building Society
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
token_urls: []
---
