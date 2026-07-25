---
api_specs:
- filename: danske-bank-uk-opendata-openapi.json
  format: json
  label: Danske Bank (UK) Open Data API
  slug: danske-bank-uk-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-opendata-openapi.json
- filename: danske-bank-uk-account-transaction-openapi.json
  format: json
  label: Danske Bank (UK) Account and Transaction API
  slug: danske-bank-uk-account-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-account-transaction-openapi.json
- filename: danske-bank-uk-payment-initiation-openapi.json
  format: json
  label: Danske Bank (UK) Payment Initiation API
  slug: danske-bank-uk-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-payment-initiation-openapi.json
- filename: danske-bank-uk-confirmation-of-funds-openapi.json
  format: json
  label: Danske Bank (UK) Confirmation of Funds API
  slug: danske-bank-uk-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-confirmation-of-funds-openapi.json
- filename: danske-bank-uk-variable-recurring-payments-openapi.json
  format: json
  label: Danske Bank (UK) Variable Recurring Payments API
  slug: danske-bank-uk-variable-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-variable-recurring-payments-openapi.json
- filename: danske-bank-uk-events-openapi.json
  format: json
  label: Danske Bank (UK) Events API
  slug: danske-bank-uk-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-events-openapi.json
- filename: danske-bank-uk-account-transaction-balance-premium-openapi.json
  format: json
  label: Danske Bank (UK) Account Transaction & Balance API
  slug: danske-bank-uk-account-transaction-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-account-transaction-balance-premium-openapi.json
- filename: danske-bank-uk-payment-collection-premium-openapi.json
  format: json
  label: Danske Bank (UK) Payment Collection API
  slug: danske-bank-uk-payment-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-payment-collection-premium-openapi.json
- filename: danske-bank-uk-premium-payment-initiation-openapi.json
  format: json
  label: Danske Bank (UK) Premium Payment Initiation API
  slug: danske-bank-uk-premium-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-premium-payment-initiation-openapi.json
- filename: danske-bank-uk-fx-trade-report-openapi.json
  format: json
  label: Danske Bank (UK) FX Trade Report API
  slug: danske-bank-uk-fx-trade-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-fx-trade-report-openapi.json
- filename: danske-bank-uk-fx-trade-execution-openapi.json
  format: json
  label: Danske Bank (UK) FX Trade Execution API
  slug: danske-bank-uk-fx-trade-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-fx-trade-execution-openapi.json
authorization_urls: []
description: ''
docs: https://developers.danskebank.com/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Danske Bank Uk Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Danske Bank (UK) publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Danske Bank (UK) API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Danske Bank (UK)
provider_slug: danske-bank-uk
schemes:
- flow: authorizationCode
  name: OpenBankingOAuth2
  note: Access-token acquisition uses OAuth2 authorization-code with OIDC, PSD2 strong customer authentication, mutual TLS and a signed request object.
  standard: OBIE FAPI 1.0 Advanced
  type: oauth2
scope_count: 4
scope_names:
- accounts
- payments
- fundsconfirmations
- openid
scopes:
- description: Access account and transaction information (AIS) - balances, transactions, beneficiaries, standing orders, direct debits, statements, parties and products, within a granted account-access consent.
  flows: []
  scope: accounts
- description: Initiate and read payments (PIS) - domestic, scheduled, standing order, file, international and variable recurring payments, within a granted payment consent.
  flows: []
  scope: payments
- description: Confirm the availability of funds on an account (CBPII) for card-based payment instrument issuers, within a granted funds-confirmation consent.
  flows: []
  scope: fundsconfirmations
- description: OpenID Connect authentication of the payment service user (PSU).
  flows: []
  scope: openid
slug: danske-bank-uk-scopes
source_filename: danske-bank-uk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  UK Open Banking (OBIE) Read/Write Data API standard OAuth2 scopes. The Danske\n  Bank (UK) Read/Write APIs are FAPI-secured OAuth2/OIDC; the OpenAPI specs\n  declare a JWT BearerAuth scheme, so the granular scope set is documented by the\n  OBIE standard rather than enumerated in-spec.\ndocs: https://developers.danskebank.com/\nschemes:\n  - name: OpenBankingOAuth2\n    type: oauth2\n    flow: authorizationCode\n    standard: OBIE FAPI 1.0 Advanced\n    note: >-\n      Access-token acquisition uses OAuth2 authorization-code with OIDC, PSD2\n      strong customer authentication, mutual TLS and a signed request object.\nscopes:\n  - scope: accounts\n    description: >-\n      Access account and transaction information (AIS) - balances,\n      transactions, beneficiaries, standing orders, direct debits, statements,\n      parties and products, within a granted account-access consent.\n    apis: [danske-bank-uk-account-transaction-api]\n\
  \  - scope: payments\n    description: >-\n      Initiate and read payments (PIS) - domestic, scheduled, standing order,\n      file, international and variable recurring payments, within a granted\n      payment consent.\n    apis: [danske-bank-uk-payment-initiation-api, danske-bank-uk-variable-recurring-payments-api]\n  - scope: fundsconfirmations\n    description: >-\n      Confirm the availability of funds on an account (CBPII) for card-based\n      payment instrument issuers, within a granted funds-confirmation consent.\n    apis: [danske-bank-uk-confirmation-of-funds-api]\n  - scope: openid\n    description: OpenID Connect authentication of the payment service user (PSU).\nnotes: >-\n  Fine-grained data access is additionally bounded by the consent object (the\n  Permissions array and expiry granted at authorization time), not by scope\n  alone. Standard OBIE scopes above; the internal registration/onboarding scope\n  set is issued via the Open Banking Directory during TPP onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/scopes/danske-bank-uk-scopes.yml
summary_line: 4 scopes
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Northern Ireland
- Payments
- Account Information
- FAPI
- Fintech
token_urls: []
---
