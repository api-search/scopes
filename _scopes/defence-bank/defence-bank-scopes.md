---
api_specs:
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Product Reference Data API
  slug: defence-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Accounts & Balances API
  slug: defence-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Transactions API
  slug: defence-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Direct Debits & Scheduled Payments API
  slug: defence-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
- filename: defence-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Defence Bank CDR Payees API
  slug: defence-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/openapi/defence-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: CDR authorization scopes govern the authenticated consumer-data-sharing endpoints. They are captured from the per-operation x-scopes extension in the OpenAPI plus the Consumer Data Standards authorisation-scopes reference. The public Product Reference Data endpoints require no scope (unauthenticated). Scopes are granted by the consumer during CDR consent to an Accredited Data Recipient.
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Defence Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Defence Bank publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Defence Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Defence Bank
provider_slug: defence-bank
schemes:
- flows:
  - flow: authorizationCode
    profile: FAPI / OIDC hybrid
  name: CDR-FAPI-OAuth2
  source: Consumer Data Standards security profile
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Read basic account information (account list, basic account detail).
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information (account terms, features, and identifiers).
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions and transaction detail.
  flows: []
  scope: bank:transactions:read
- description: Read direct debits, scheduled payments, and instalment plans.
  flows: []
  scope: bank:regular_payments:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
slug: defence-bank-scopes
source_filename: defence-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/defence-bank-cds-banking-products-openapi.yml (x-scopes per operation)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\ndescription: >-\n  CDR authorization scopes govern the authenticated consumer-data-sharing endpoints.\n  They are captured from the per-operation x-scopes extension in the OpenAPI plus the\n  Consumer Data Standards authorisation-scopes reference. The public Product Reference\n  Data endpoints require no scope (unauthenticated). Scopes are granted by the consumer\n  during CDR consent to an Accredited Data Recipient.\nschemes:\n- name: CDR-FAPI-OAuth2\n  source: Consumer Data Standards security profile\n  flows:\n  - flow: authorizationCode\n    profile: FAPI / OIDC hybrid\nscopes:\n- scope: bank:accounts.basic:read\n  description: Read basic account information (account list, basic account detail).\n  operations: [listBankingAccounts, getBankingAccountDetail,\
  \ listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n- scope: bank:accounts.detail:read\n  description: Read detailed account information (account terms, features, and identifiers).\n  operations: [getBankingAccountDetail]\n- scope: bank:transactions:read\n  description: Read account transactions and transaction detail.\n  operations: [listBankingTransactions, getBankingTransactionDetail]\n- scope: bank:regular_payments:read\n  description: Read direct debits, scheduled payments, and instalment plans.\n  operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n- scope: bank:payees:read\n  description: Read saved payees.\n  operations: [listBankingPayees, getBankingPayeeDetail]\nnotes:\n  - Product Reference Data endpoints (listBankingProducts, getBankingProductDetail) are public and require no\
  \ scope.\n  - CDR also defines the openid and (via the register) profile scopes for the OIDC layer; the bank:* scopes above are the data-cluster scopes declared in this spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defence-bank/refs/heads/main/scopes/defence-bank-scopes.yml
summary_line: 5 scopes · authorizationCode
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
