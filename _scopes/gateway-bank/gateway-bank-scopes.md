---
api_specs:
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Product Reference Data API
  slug: gateway-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Accounts & Balances API
  slug: gateway-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Transactions API
  slug: gateway-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Direct Debits & Scheduled Payments API
  slug: gateway-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
- filename: gateway-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Gateway Bank CDR Payees API
  slug: gateway-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/openapi/gateway-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Gateway Bank Scopes
name_suffix: OAuth Scopes
note: Scopes are the standard CDR banking authorisation scopes carried on the CDS operations via the x-scopes extension (the DSB spec does not declare OpenAPI securitySchemes; it expresses authorisation via x-scopes). They apply only to the authenticated consumer-data surface; the public PRD endpoints require no scope.
overview: 'Gateway Bank publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gateway Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gateway Bank
provider_slug: gateway-bank
schemes:
- flows:
  - flow: authorizationCode
  name: CDR-security-profile
  profile: FAPI 2.0 (CDR)
  type: openIdConnect
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
scopes:
- description: Read basic account information (account list and basic detail).
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information.
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions.
  flows: []
  scope: bank:transactions:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
- description: Read direct debits and scheduled/regular payments.
  flows: []
  scope: bank:regular_payments:read
slug: gateway-bank-scopes
source_filename: gateway-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/gateway-bank-cds-banking-products-openapi.yml (x-scopes extensions)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: Scopes are the standard CDR banking authorisation scopes carried on the CDS\n  operations via the x-scopes extension (the DSB spec does not declare OpenAPI\n  securitySchemes; it expresses authorisation via x-scopes). They apply only to the\n  authenticated consumer-data surface; the public PRD endpoints require no scope.\nschemes:\n- name: CDR-security-profile\n  type: openIdConnect\n  profile: FAPI 2.0 (CDR)\n  flows:\n  - flow: authorizationCode\nscopes:\n- scope: bank:accounts.basic:read\n  description: Read basic account information (account list and basic detail).\n  operations: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts,\n    getBankingBalance]\n- scope: bank:accounts.detail:read\n  description: Read detailed account\
  \ information.\n  operations: [getBankingAccountDetail]\n- scope: bank:transactions:read\n  description: Read account transactions.\n  operations: [listBankingTransactions, getBankingTransactionDetail]\n- scope: bank:payees:read\n  description: Read saved payees.\n  operations: [listBankingPayees, getBankingPayeeDetail]\n- scope: bank:regular_payments:read\n  description: Read direct debits and scheduled/regular payments.\n  operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts,\n    listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gateway-bank/refs/heads/main/scopes/gateway-bank-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Mutual Bank
- Customer Owned
- Australia
- Product Reference Data
token_urls: []
---
