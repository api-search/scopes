---
api_specs:
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Product Reference Data API
  slug: avenue-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Accounts & Balances API
  slug: avenue-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Transactions API
  slug: avenue-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Direct Debits & Scheduled Payments API
  slug: avenue-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Payees API
  slug: avenue-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
authorization_urls:
- https://consumerdatastandardsaustralia.github.io/standards/#security-profile
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Avenue Bank Scopes
name_suffix: OAuth Scopes
note: The harvested OpenAPI does not enumerate oauth2 scopes (bare DSB banking contract). These are the standardized CDR banking authorisation scopes the endpoints require per the Consumer Data Standards, mapped to the operations in this repo. Product Reference Data endpoints are public and require no scope. Live status unverified (API host returned HTTP 403 WAF on 2026-07-21).
overview: 'Avenue Bank publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Avenue Bank API on a user''s behalf.


  Tokens are issued from https://consumerdatastandardsaustralia.github.io/standards/#security-profile.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Avenue Bank
provider_slug: avenue-bank
schemes:
- flows:
  - authorizationUrl: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
    flow: authorizationCode
    tokenUrl: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  name: cdr-oauth2
  source: openapi/avenue-bank-cds-banking-openapi.json
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
scopes:
- description: Account name, type, balance and masked account number.
  flows: []
  scope: bank:accounts.basic:read
- description: Account numbers and full account details.
  flows: []
  scope: bank:accounts.detail:read
- description: Transactions on an account.
  flows: []
  scope: bank:transactions:read
- description: Saved payees.
  flows: []
  scope: bank:payees:read
- description: Direct debits, scheduled payments and instalment plans.
  flows: []
  scope: bank:regular_payments:read
slug: avenue-bank-scopes
source_filename: avenue-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/avenue-bank-cds-banking-openapi.json\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: The harvested OpenAPI does not enumerate oauth2 scopes (bare DSB banking contract). These are the\n  standardized CDR banking authorisation scopes the endpoints require per the Consumer Data Standards,\n  mapped to the operations in this repo. Product Reference Data endpoints are public and require no scope.\n  Live status unverified (API host returned HTTP 403 WAF on 2026-07-21).\nschemes:\n- name: cdr-oauth2\n  source: openapi/avenue-bank-cds-banking-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n    tokenUrl: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nscopes:\n- scope: bank:accounts.basic:read\n  description: Account name, type, balance and masked\
  \ account number.\n  operations:\n  - listBankingAccounts\n  - getBankingBalance\n  - listBankingBalancesBulk\n  - listBankingBalancesSpecificAccounts\n- scope: bank:accounts.detail:read\n  description: Account numbers and full account details.\n  operations:\n  - getBankingAccountDetail\n- scope: bank:transactions:read\n  description: Transactions on an account.\n  operations:\n  - listBankingTransactions\n  - getBankingTransactionDetail\n- scope: bank:payees:read\n  description: Saved payees.\n  operations:\n  - listBankingPayees\n  - getBankingPayeeDetail\n- scope: bank:regular_payments:read\n  description: Direct debits, scheduled payments and instalment plans.\n  operations:\n  - listDirectDebits\n  - listDirectDebitsBulk\n  - listDirectDebitsSpecificAccounts\n  - listScheduledPayments\n  - listScheduledPaymentsBulk\n  - listScheduledPaymentsSpecificAccounts\n  - listInstalmentPlans\n  - listInstalmentPlansBulk\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/scopes/avenue-bank-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Business Banking
- Bank Guarantees
- Australia
- ADI
token_urls:
- https://consumerdatastandardsaustralia.github.io/standards/#security-profile
---
