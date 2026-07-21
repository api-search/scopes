---
api_specs:
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Product Reference Data API
  slug: australian-unity-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Accounts & Balances API
  slug: australian-unity-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Transactions API
  slug: australian-unity-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Direct Debits & Scheduled Payments API
  slug: australian-unity-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
- filename: australian-unity-bank-cds-banking-openapi.json
  format: json
  label: Australian Unity Bank CDR Payees API
  slug: australian-unity-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/openapi/australian-unity-bank-cds-banking-openapi.json
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
- hybrid
kind: oauth-scopes
layout: scope
method: searched
name: Australian Unity Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Australian Unity Bank publishes 9 OAuth 2.0 scopes via the authorizationCode and hybrid flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Australian Unity Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Australian Unity Bank
provider_slug: australian-unity-bank
schemes:
- flows:
  - authorizationCode
  - hybrid
  name: CDR-OIDC
  profile: FAPI 1.0 Advanced (CDR Security Profile)
  type: openIdConnect
scope_count: 9
scope_names:
- openid
- profile
- common:customer.basic:read
- common:customer.detail:read
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: OpenID Connect authentication (required by the CDR flow).
  flows: []
  scope: openid
- description: Basic profile claims within the CDR consent.
  flows: []
  scope: profile
- description: Read basic customer/member identity data.
  flows: []
  scope: common:customer.basic:read
- description: Read detailed customer/member data (contact details).
  flows: []
  scope: common:customer.detail:read
- description: List accounts and read basic account and balance data.
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account data.
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions.
  flows: []
  scope: bank:transactions:read
- description: Read direct debits, scheduled payments, and instalment plans.
  flows: []
  scope: bank:regular_payments:read
- description: Read the member's saved payees.
  flows: []
  scope: bank:payees:read
slug: australian-unity-bank-scopes
source_filename: australian-unity-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnotes: >-\n  The DSB Consumer Data Standards define the fixed authorisation-scope set that\n  every Australian ADI (including Australian Unity Bank, as a CDR data holder)\n  must honour for consumer-authorised banking data. Scopes are not declared in the\n  harvested CDS Banking OpenAPI (auth lives in the separate CDR InfoSec profile),\n  so this scope list is captured from the DSB standard, mapped to the operations\n  in openapi/australian-unity-bank-cds-banking-openapi.json. Product Reference\n  Data endpoints are public and require no scope.\nschemes:\n  - name: CDR-OIDC\n    type: openIdConnect\n    profile: FAPI 1.0 Advanced (CDR Security Profile)\n    flows: [authorizationCode, hybrid]\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication\
  \ (required by the CDR flow).\n  - scope: profile\n    description: Basic profile claims within the CDR consent.\n  - scope: common:customer.basic:read\n    description: Read basic customer/member identity data.\n  - scope: common:customer.detail:read\n    description: Read detailed customer/member data (contact details).\n  - scope: bank:accounts.basic:read\n    description: List accounts and read basic account and balance data.\n    operations: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n  - scope: bank:accounts.detail:read\n    description: Read detailed account data.\n    operations: [getBankingAccountDetail]\n  - scope: bank:transactions:read\n    description: Read account transactions.\n    operations: [listBankingTransactions, getBankingTransactionDetail]\n  - scope: bank:regular_payments:read\n    description: Read direct debits, scheduled payments, and instalment plans.\n    operations: [listDirectDebits, listDirectDebitsBulk,\
  \ listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n  - scope: bank:payees:read\n    description: Read the member's saved payees.\n    operations: [listBankingPayees, getBankingPayeeDetail]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-unity-bank/refs/heads/main/scopes/australian-unity-bank-scopes.yml
summary_line: 9 scopes · authorizationCode/hybrid
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual
- Product Reference Data
token_urls: []
---
