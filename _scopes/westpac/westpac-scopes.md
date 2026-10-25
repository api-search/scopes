---
api_specs:
- filename: postman_collection.quickstreamapi.json
  format: json
  label: Westpac QuickStream REST API
  slug: westpac-quickstream-rest-api
  spec_type: Postman
  url: https://quickstream.westpac.com.au/docs/downloads/postman_collection.quickstreamapi.json
- filename: westpac-banking-account-balances-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Balances API
  slug: westpac-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-balances-api-openapi.yml
- filename: westpac-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Direct Debits API
  slug: westpac-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-direct-debits-api-openapi.yml
- filename: westpac-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Scheduled Payments API
  slug: westpac-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-scheduled-payments-api-openapi.yml
- filename: westpac-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Account Transactions API
  slug: westpac-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-account-transactions-api-openapi.yml
- filename: westpac-banking-accounts-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Accounts API
  slug: westpac-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-accounts-api-openapi.yml
- filename: westpac-banking-payees-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Payees API
  slug: westpac-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-payees-api-openapi.yml
- filename: westpac-banking-products-api-openapi.yml
  format: yaml
  label: Westpac Banking Corporation Banking Products API
  slug: westpac-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/openapi/westpac-banking-products-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Westpac Scopes
name_suffix: OAuth Scopes
note: Derived from the per-operation x-scopes extensions in the DSB CDR Banking API (v1.36.0) contract held for Westpac. The contract declares no securitySchemes, so derive-oauth-scopes.py found nothing; these scopes are the CDR consent scopes an Accredited Data Recipient obtains through the CDR OAuth 2.0 / FAPI consent flow. They are defined by the Data Standards Body, not by Westpac. listBankingProducts and getBankingProductDetail carry no scope and are public.
overview: 'Westpac publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Westpac API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Westpac
provider_slug: westpac
schemes: []
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: ''
  flows: []
  scope: bank:accounts.basic:read
- description: ''
  flows: []
  scope: bank:accounts.detail:read
- description: ''
  flows: []
  scope: bank:transactions:read
- description: ''
  flows: []
  scope: bank:regular_payments:read
- description: ''
  flows: []
  scope: bank:payees:read
slug: westpac-scopes
source_filename: westpac-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/_original/westpac-cds-banking-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/\nnote: >-\n  Derived from the per-operation x-scopes extensions in the DSB CDR Banking API\n  (v1.36.0) contract held for Westpac. The contract declares no\n  securitySchemes, so derive-oauth-scopes.py found nothing; these scopes are\n  the CDR consent scopes an Accredited Data Recipient obtains through the CDR\n  OAuth 2.0 / FAPI consent flow. They are defined by the Data Standards Body,\n  not by Westpac. listBankingProducts and getBankingProductDetail carry no\n  scope and are public.\nscopes:\n  - name: bank:accounts.basic:read\n    operations: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n  - name: bank:accounts.detail:read\n    operations: [getBankingAccountDetail]\n  - name: bank:transactions:read\n    operations: [listBankingTransactions, getBankingTransactionDetail]\n\
  \  - name: bank:regular_payments:read\n    operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n  - name: bank:payees:read\n    operations: [listBankingPayees, getBankingPayeeDetail]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westpac/refs/heads/main/scopes/westpac-scopes.yml
summary_line: 5 scopes
tags:
- Finance
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
token_bound: false
token_urls: []
---
