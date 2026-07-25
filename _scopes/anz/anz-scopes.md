---
api_specs:
- filename: anz-banking-account-balances-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Balances API
  slug: anz-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-balances-api-openapi.yml
- filename: anz-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Direct Debits API
  slug: anz-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-direct-debits-api-openapi.yml
- filename: anz-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Scheduled Payments API
  slug: anz-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-scheduled-payments-api-openapi.yml
- filename: anz-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Transactions API
  slug: anz-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-transactions-api-openapi.yml
- filename: anz-banking-accounts-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Accounts API
  slug: anz-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-accounts-api-openapi.yml
- filename: anz-banking-payees-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Payees API
  slug: anz-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-payees-api-openapi.yml
- filename: anz-banking-products-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Products API
  slug: anz-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-products-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Anz Scopes
name_suffix: OAuth Scopes
note: The public ANZ Product Reference Data endpoints require NO OAuth scope (they are unauthenticated). The scopes below govern the CDR consumer-data-sharing operations in the shared DSB Consumer Data Standards banking contract, which ANZ exposes only to CDR-accredited Data Recipients under consumer consent. Scope strings are captured verbatim from the spec's per-operation x-scopes extension and the Consumer Data Standards authorisation-scopes reference.
overview: 'Australia and New Zealand Banking Group (ANZ) publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Australia and New Zealand Banking Group (ANZ) API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Australia and New Zealand Banking Group (ANZ)
provider_slug: anz
schemes:
- flows:
  - flow: authorizationCode
  name: CDR-FAPI-OAuth2
  profile: FAPI 1.0 Advanced
  source: openapi/anz-cds-banking-products-openapi.yml
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Read basic account information (account list, masked numbers, product category).
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information including account numbers and features.
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions.
  flows: []
  scope: bank:transactions:read
- description: Read direct debits, scheduled payments and recurring/instalment payment arrangements.
  flows: []
  scope: bank:regular_payments:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
slug: anz-scopes
source_filename: anz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/anz-cds-banking-products-openapi.yml (x-scopes extension)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >\n  The public ANZ Product Reference Data endpoints require NO OAuth scope (they are\n  unauthenticated). The scopes below govern the CDR consumer-data-sharing operations\n  in the shared DSB Consumer Data Standards banking contract, which ANZ exposes only\n  to CDR-accredited Data Recipients under consumer consent. Scope strings are captured\n  verbatim from the spec's per-operation x-scopes extension and the Consumer Data\n  Standards authorisation-scopes reference.\nschemes:\n- name: CDR-FAPI-OAuth2\n  profile: FAPI 1.0 Advanced\n  source: openapi/anz-cds-banking-products-openapi.yml\n  flows:\n  - flow: authorizationCode\nscopes:\n- scope: bank:accounts.basic:read\n  description: Read basic account information (account list, masked numbers, product category).\n\
  \  operations: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n- scope: bank:accounts.detail:read\n  description: Read detailed account information including account numbers and features.\n  operations: [getBankingAccountDetail]\n- scope: bank:transactions:read\n  description: Read account transactions.\n  operations: [listBankingTransactions, getBankingTransactionDetail]\n- scope: bank:regular_payments:read\n  description: Read direct debits, scheduled payments and recurring/instalment payment arrangements.\n  operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n- scope: bank:payees:read\n  description: Read saved payees.\n  operations: [listBankingPayees, getBankingPayeeDetail]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/scopes/anz-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
token_urls: []
---
