---
api_specs:
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Product Reference Data API
  slug: bankvic-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Accounts & Balances API
  slug: bankvic-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Transactions API
  slug: bankvic-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Direct Debits & Scheduled Payments API
  slug: bankvic-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
- filename: bankvic-cds-banking-products-openapi.yml
  format: yaml
  label: BankVic CDR Payees API
  slug: bankvic-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/openapi/bankvic-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Bankvic Scopes
name_suffix: OAuth Scopes
note: The OpenAPI contract in this repo declares no oauth2 securitySchemes (it documents the public Product Reference Data surface, which is unauthenticated, alongside the consented consumer-data surface). BankVic's consented CDR banking surface is authorised through the shared DSB Consumer Data Standards OAuth 2.0 / OIDC + FAPI 2.0 profile, whose authorisation scopes are the canonical CDR banking + common scopes below (not bank-proprietary). Public PRD endpoints (listBankingProducts, getBankingProductDetail) require NO scope. Scopes are requested by an accredited Data Recipient (ADR); there is no self-service developer OAuth client for the public.
overview: 'BankVic publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BankVic API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BankVic
provider_slug: bankvic
schemes:
- flows:
  - flow: authorizationCode
    note: Authorization/token endpoints are published per Data Holder via the CDR Register / holder OIDC discovery; BankVic acts as Data Holder. Tokens are mTLS sender-constrained; consent is time-boxed and revocable.
  name: CDR OIDC / FAPI 2.0 (authorization code + PKCE + PAR + mTLS)
  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
scope_count: 9
scope_names:
- openid
- profile
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
- common:customer.basic:read
- common:customer.detail:read
scopes:
- description: OIDC subject identifier; required to initiate a CDR authorisation.
  flows:
  - authorizationCode
  scope: openid
- description: OIDC standard profile claims where consented.
  flows:
  - authorizationCode
  scope: profile
- description: Read basic account information (account list, type, balance summary).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account information (features, fees, account numbers).
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read account transactions and transaction detail.
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read direct debits, scheduled payments, and instalment plans.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
- description: Read saved payees (domestic, biller, international).
  flows:
  - authorizationCode
  scope: bank:payees:read
- description: Read basic customer profile (name, occupation / organisation basics).
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read detailed customer profile (contact details, address).
  flows:
  - authorizationCode
  scope: common:customer.detail:read
slug: bankvic-scopes
source_filename: bankvic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/bankvic-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  The OpenAPI contract in this repo declares no oauth2 securitySchemes (it documents\n  the public Product Reference Data surface, which is unauthenticated, alongside the\n  consented consumer-data surface). BankVic's consented CDR banking surface is\n  authorised through the shared DSB Consumer Data Standards OAuth 2.0 / OIDC + FAPI 2.0\n  profile, whose authorisation scopes are the canonical CDR banking + common scopes\n  below (not bank-proprietary). Public PRD endpoints (listBankingProducts,\n  getBankingProductDetail) require NO scope. Scopes are requested by an accredited\n  Data Recipient (ADR); there is no self-service developer OAuth client for the public.\nschemes:\n  - name: CDR OIDC / FAPI 2.0 (authorization code + PKCE + PAR + mTLS)\n    source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n\
  \    flows:\n      - flow: authorizationCode\n        note: >-\n          Authorization/token endpoints are published per Data Holder via the CDR\n          Register / holder OIDC discovery; BankVic acts as Data Holder. Tokens are\n          mTLS sender-constrained; consent is time-boxed and revocable.\nscopes:\n  - scope: openid\n    description: OIDC subject identifier; required to initiate a CDR authorisation.\n    flows: [authorizationCode]\n  - scope: profile\n    description: OIDC standard profile claims where consented.\n    flows: [authorizationCode]\n  - scope: bank:accounts.basic:read\n    description: Read basic account information (account list, type, balance summary).\n    operations: [listBankingAccounts, getBankingBalance, listBankingBalancesBulk, listBankingBalancesSpecificAccounts]\n    flows: [authorizationCode]\n  - scope: bank:accounts.detail:read\n    description: Read detailed account information (features, fees, account numbers).\n    operations: [getBankingAccountDetail]\n\
  \    flows: [authorizationCode]\n  - scope: bank:transactions:read\n    description: Read account transactions and transaction detail.\n    operations: [listBankingTransactions, getBankingTransactionDetail]\n    flows: [authorizationCode]\n  - scope: bank:regular_payments:read\n    description: Read direct debits, scheduled payments, and instalment plans.\n    operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n    flows: [authorizationCode]\n  - scope: bank:payees:read\n    description: Read saved payees (domestic, biller, international).\n    operations: [listBankingPayees, getBankingPayeeDetail]\n    flows: [authorizationCode]\n  - scope: common:customer.basic:read\n    description: Read basic customer profile (name, occupation / organisation basics).\n    flows: [authorizationCode]\n  - scope: common:customer.detail:read\n\
  \    description: Read detailed customer profile (contact details, address).\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankvic/refs/heads/main/scopes/bankvic-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
token_urls: []
---
