---
api_specs:
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Product Reference Data API
  slug: beyond-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Accounts & Balances API
  slug: beyond-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Transactions API
  slug: beyond-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Direct Debits & Scheduled Payments API
  slug: beyond-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
- filename: beyond-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Beyond Bank Australia CDR Payees API
  slug: beyond-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/openapi/beyond-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Beyond Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Beyond Bank Australia publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beyond Bank Australia API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beyond Bank Australia
provider_slug: beyond-bank
schemes:
- flows:
  - flow: authorizationCode
    note: OIDC hybrid/authorization-code with PAR (Pushed Authorization Requests), request object signing, and mTLS-bound tokens per the CDR FAPI profile.
  name: cdr-oauth2-fapi
  profile: FAPI 1.0 Advanced (CDR security profile)
  source: openapi/beyond-bank-cds-banking-products-openapi.yml (x-scopes)
  type: oauth2
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Read account identifiers and balances — the account list and balance endpoints. Grants basic account data without masked account numbers or product detail.
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information including masked account numbers, account terms, features, addresses, and product-category detail.
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions and transaction detail (with date/amount/text filters).
  flows: []
  scope: bank:transactions:read
- description: Read direct debits, scheduled payments, and instalment plans authorised against the consumer's accounts.
  flows: []
  scope: bank:regular_payments:read
- description: Read the consumer's saved payees (domestic, international, and BPAY payee types).
  flows: []
  scope: bank:payees:read
slug: beyond-bank-scopes
source_filename: beyond-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/beyond-bank-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnotes: >-\n  OAuth2 authorisation scopes for Beyond Bank's CDR Banking surface. The harvested DSB\n  Consumer Data Standards contract does not declare formal OpenAPI securitySchemes; it\n  carries the scope requirement per operation on the CDR-specific `x-scopes` extension.\n  These five banking scopes were derived by aggregating every `x-scopes` value across the\n  spec's operations, and their descriptions follow the published DSB Consumer Data\n  Standards authorisation-scope definitions. Scopes apply ONLY to the consumer-authorised\n  (accredited Data Recipient) surface — the public Product Reference Data operations\n  (listBankingProducts / getBankingProductDetail) declare no `x-scopes` and require no\n  authorisation. Scopes are requested via the CDR OAuth2/OIDC FAPI authorization\
  \ request\n  (with the mandatory `openid` and `profile` OIDC scopes and the CDR `cdr:registration`\n  where applicable); the token, authorization, and PAR endpoints live on Beyond Bank's CDR\n  identity server (advertised via the CDR Register and the holder's OIDC discovery document),\n  not on the public PRD host, so their URLs are not asserted here.\nschemes:\n  - name: cdr-oauth2-fapi\n    type: oauth2\n    profile: FAPI 1.0 Advanced (CDR security profile)\n    flows:\n      - flow: authorizationCode\n        note: >-\n          OIDC hybrid/authorization-code with PAR (Pushed Authorization Requests),\n          request object signing, and mTLS-bound tokens per the CDR FAPI profile.\n    source: openapi/beyond-bank-cds-banking-products-openapi.yml (x-scopes)\nscopes:\n  - scope: bank:accounts.basic:read\n    description: >-\n      Read account identifiers and balances — the account list and balance endpoints.\n      Grants basic account data without masked account numbers or product\
  \ detail.\n    operations: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n  - scope: bank:accounts.detail:read\n    description: >-\n      Read detailed account information including masked account numbers, account terms,\n      features, addresses, and product-category detail.\n    operations: [getBankingAccountDetail]\n  - scope: bank:transactions:read\n    description: Read account transactions and transaction detail (with date/amount/text filters).\n    operations: [listBankingTransactions, getBankingTransactionDetail]\n  - scope: bank:regular_payments:read\n    description: >-\n      Read direct debits, scheduled payments, and instalment plans authorised against the\n      consumer's accounts.\n    operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n  - scope:\
  \ bank:payees:read\n    description: Read the consumer's saved payees (domestic, international, and BPAY payee types).\n    operations: [listBankingPayees, getBankingPayeeDetail]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-bank/refs/heads/main/scopes/beyond-bank-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Product Reference Data
token_urls: []
---
