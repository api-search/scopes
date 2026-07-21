---
api_specs:
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Product Reference Data API
  slug: teachers-mutual-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Accounts & Balances API
  slug: teachers-mutual-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Transactions API
  slug: teachers-mutual-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Direct Debits & Scheduled Payments API
  slug: teachers-mutual-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
- filename: teachers-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Teachers Mutual Bank CDR Payees API
  slug: teachers-mutual-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/openapi/teachers-mutual-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Teachers Mutual Bank Scopes
name_suffix: OAuth Scopes
note: The public Product Reference Data (PRD) surface is unauthenticated and carries no scopes. The consumer data-sharing channel (accounts, balances, transactions, direct debits, scheduled payments, payees) is authorised via the CDR OAuth2 / OpenID Connect FAPI 1.0 profile. Each protected operation declares its required authorisation scope through the CDR `x-scopes` OpenAPI extension in the captured contract. The five banking scopes below are the standard DSB Consumer Data Standards authorisation scopes; scope strings and per-operation requirements are taken verbatim from the harvested spec, and descriptions follow the published Consumer Data Standards. Teachers Mutual Bank does not define custom scopes beyond the shared DSB banking scope set.
overview: 'Teachers Mutual Bank publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Teachers Mutual Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Teachers Mutual Bank
provider_slug: teachers-mutual-bank
schemes: []
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Account name, type, account holder(s), and balance. Basic account information used to list a consumer's banking accounts and read account and bulk balances.
  flows: []
  scope: bank:accounts.basic:read
- description: Detailed account information including account numbers, features, rates, fees, and other account-specific detail beyond the basic profile.
  flows: []
  scope: bank:accounts.detail:read
- description: Transaction details for authorised accounts, including amounts, dates, descriptions, and per-transaction detail.
  flows: []
  scope: bank:transactions:read
- description: Direct debits, scheduled payments, and instalment plans configured against a consumer's authorised accounts.
  flows: []
  scope: bank:regular_payments:read
- description: Saved payees stored by the consumer, returned only where the consumer has authorised sharing of their payee list.
  flows: []
  scope: bank:payees:read
slug: teachers-mutual-bank-scopes
source_filename: teachers-mutual-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\ngenerated: '2026-07-21'\nmethod: derived\nprovider: Teachers Mutual Bank\nproviderId: teachers-mutual-bank\nsource: openapi/teachers-mutual-bank-cds-banking-products-openapi.yml (x-scopes) + Consumer Data Standards authorisation scopes\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  The public Product Reference Data (PRD) surface is unauthenticated and carries no\n  scopes. The consumer data-sharing channel (accounts, balances, transactions, direct\n  debits, scheduled payments, payees) is authorised via the CDR OAuth2 / OpenID Connect\n  FAPI 1.0 profile. Each protected operation declares its required authorisation scope\n  through the CDR `x-scopes` OpenAPI extension in the captured contract. The five banking\n  scopes below are the standard DSB Consumer Data Standards authorisation scopes; scope\n  strings and per-operation requirements are taken verbatim\
  \ from the harvested spec, and\n  descriptions follow the published Consumer Data Standards. Teachers Mutual Bank does not\n  define custom scopes beyond the shared DSB banking scope set.\ntags:\n- CDR\n- Open Banking\n- OAuth2\n- FAPI\n- Authorisation Scopes\nflow: authorizationCode\nscopes:\n- scope: bank:accounts.basic:read\n  description: >-\n    Account name, type, account holder(s), and balance. Basic account information used\n    to list a consumer's banking accounts and read account and bulk balances.\n  operations:\n  - listBankingAccounts\n  - getBankingBalance\n  - listBankingBalancesBulk\n  - listBankingBalancesSpecificAccounts\n- scope: bank:accounts.detail:read\n  description: >-\n    Detailed account information including account numbers, features, rates, fees, and\n    other account-specific detail beyond the basic profile.\n  operations:\n  - getBankingAccountDetail\n- scope: bank:transactions:read\n  description: >-\n    Transaction details for authorised accounts, including\
  \ amounts, dates, descriptions,\n    and per-transaction detail.\n  operations:\n  - listBankingTransactions\n  - getBankingTransactionDetail\n- scope: bank:regular_payments:read\n  description: >-\n    Direct debits, scheduled payments, and instalment plans configured against a\n    consumer's authorised accounts.\n  operations:\n  - listDirectDebits\n  - listDirectDebitsBulk\n  - listDirectDebitsSpecificAccounts\n  - listScheduledPayments\n  - listScheduledPaymentsBulk\n  - listScheduledPaymentsSpecificAccounts\n  - listInstalmentPlans\n  - listInstalmentPlansBulk\n- scope: bank:payees:read\n  description: >-\n    Saved payees stored by the consumer, returned only where the consumer has authorised\n    sharing of their payee list.\n  operations:\n  - listBankingPayees\n  - getBankingPayeeDetail\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachers-mutual-bank/refs/heads/main/scopes/teachers-mutual-bank-scopes.yml
summary_line: 5 scopes
tags:
- CDR
- Open Banking
- OAuth2
- FAPI
- Authorisation Scopes
token_urls: []
---
