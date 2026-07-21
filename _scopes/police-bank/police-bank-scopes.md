---
api_specs:
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Product Reference Data API
  slug: police-bank-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Accounts & Balances API
  slug: police-bank-cds-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Transactions API
  slug: police-bank-cds-banking-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Direct Debits & Scheduled Payments API
  slug: police-bank-cds-banking-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
- filename: police-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Police Bank CDR Payees API
  slug: police-bank-cds-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/openapi/police-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Police Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Police Bank publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Police Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Police Bank
provider_slug: police-bank
schemes:
- flows:
  - authorizationUrl: null
    flow: authorizationCode
    tokenUrl: null
  name: CDR-OAuth2
  note: 'Consumer Data Right authorisation follows the CDS security profile (FAPI 1.0 Advanced): OpenID Connect authorization-code flow with PKCE, PAR, and MTLS-bound tokens. Authorization/token endpoints are per-data-holder and resolved from Police Bank''s OIDC discovery document at authorisation time; they are not published on the public PRD surface.'
  source: openapi/police-bank-cds-banking-products-openapi.yml
  type: oauth2
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Basic account information - the list of a member's accounts plus balances.
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Detailed account information - account numbers, features, fees, rates and other account detail beyond the basic list.
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Transactions - the ability to read a member's transactions for authorised accounts, including transaction detail.
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Regular payments - direct debits, scheduled payments and instalment plans configured on a member's accounts.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
- description: Saved payees - the member's stored domestic, international and BPAY payees.
  flows:
  - authorizationCode
  scope: bank:payees:read
slug: police-bank-scopes
source_filename: police-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/police-bank-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\n# CDR (Consumer Data Right) banking authorisation scopes required by Police Bank's\n# authenticated CDR Banking operations. Derived from the x-scopes extension attached\n# to each authenticated operation in the OpenAPI (the spec declares no formal\n# securitySchemes block; scopes are carried as x-scopes). These are the standard\n# Consumer Data Standards banking scopes - not Police Bank-proprietary. The public\n# Product Reference Data operations (listBankingProducts / getBankingProductDetail)\n# require NO scope and are unauthenticated.\nschemes:\n- name: CDR-OAuth2\n  type: oauth2\n  source: openapi/police-bank-cds-banking-products-openapi.yml\n  note: >-\n    Consumer Data Right authorisation follows the CDS security profile (FAPI 1.0\n    Advanced): OpenID Connect authorization-code\
  \ flow with PKCE, PAR, and\n    MTLS-bound tokens. Authorization/token endpoints are per-data-holder and\n    resolved from Police Bank's OIDC discovery document at authorisation time;\n    they are not published on the public PRD surface.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: null\n    tokenUrl: null\nscopes:\n- scope: bank:accounts.basic:read\n  description: >-\n    Basic account information - the list of a member's accounts plus balances.\n  flows: [authorizationCode]\n  operations: [listBankingAccounts, getBankingBalance, listBankingBalancesBulk, listBankingBalancesSpecificAccounts]\n  sources: [openapi/police-bank-cds-banking-products-openapi.yml]\n- scope: bank:accounts.detail:read\n  description: >-\n    Detailed account information - account numbers, features, fees, rates and\n    other account detail beyond the basic list.\n  flows: [authorizationCode]\n  operations: [getBankingAccountDetail]\n  sources: [openapi/police-bank-cds-banking-products-openapi.yml]\n\
  - scope: bank:transactions:read\n  description: >-\n    Transactions - the ability to read a member's transactions for authorised\n    accounts, including transaction detail.\n  flows: [authorizationCode]\n  operations: [listBankingTransactions, getBankingTransactionDetail]\n  sources: [openapi/police-bank-cds-banking-products-openapi.yml]\n- scope: bank:regular_payments:read\n  description: >-\n    Regular payments - direct debits, scheduled payments and instalment plans\n    configured on a member's accounts.\n  flows: [authorizationCode]\n  operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n  sources: [openapi/police-bank-cds-banking-products-openapi.yml]\n- scope: bank:payees:read\n  description: >-\n    Saved payees - the member's stored domestic, international and BPAY payees.\n  flows: [authorizationCode]\n  operations:\
  \ [listBankingPayees, getBankingPayeeDetail]\n  sources: [openapi/police-bank-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/police-bank/refs/heads/main/scopes/police-bank-scopes.yml
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
