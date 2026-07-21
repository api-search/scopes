---
api_specs:
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Product Reference Data API
  slug: australian-military-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Accounts & Balances API
  slug: australian-military-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Transactions API
  slug: australian-military-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Direct Debits & Scheduled Payments API
  slug: australian-military-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
- filename: australian-military-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Australian Military Bank CDR Payees API
  slug: australian-military-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/openapi/australian-military-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: OAuth2 authorization scopes for the consumer-authorized surface of Australian Military Bank's CDR (Consumer Data Right) Banking API. The bank declares no formal OpenAPI securitySchemes; scopes are published per-operation as `x-scopes` extensions in the Data Standards Body CDR Banking API (v1.36.0) that the bank implements as a registered ADI / CDR data holder. These scopes are granted only to CDR-accredited data recipients (ADRs) through the FAPI-profiled OAuth2/OIDC consent flow over mutual-TLS; the public Product Reference Data endpoints (listBankingProducts, getBankingProductDetail) require no scope and no auth.
docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Australian Military Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Australian Military Bank uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Australian Military Bank
provider_slug: australian-military-bank
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: australian-military-bank-scopes
source_filename: australian-military-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/australian-military-bank-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndescription: >-\n  OAuth2 authorization scopes for the consumer-authorized surface of Australian\n  Military Bank's CDR (Consumer Data Right) Banking API. The bank declares no\n  formal OpenAPI securitySchemes; scopes are published per-operation as `x-scopes`\n  extensions in the Data Standards Body CDR Banking API (v1.36.0) that the bank\n  implements as a registered ADI / CDR data holder. These scopes are granted only\n  to CDR-accredited data recipients (ADRs) through the FAPI-profiled OAuth2/OIDC\n  consent flow over mutual-TLS; the public Product Reference Data endpoints\n  (listBankingProducts, getBankingProductDetail) require no scope and no auth.\nflow: authorization_code\ntoken_binding: mutualTLS\nprofile: FAPI 2.0 (AU-CDR)\nscopes:\n  - name: bank:accounts.basic:read\n\
  \    description: Read basic account information (account list and balances).\n    operations:\n      - listBankingAccounts\n      - listBankingBalancesBulk\n      - listBankingBalancesSpecificAccounts\n      - getBankingBalance\n  - name: bank:accounts.detail:read\n    description: Read detailed account information including account numbers and features.\n    operations:\n      - getBankingAccountDetail\n  - name: bank:transactions:read\n    description: Read transactions for authorized accounts.\n    operations:\n      - listBankingTransactions\n      - getBankingTransactionDetail\n  - name: bank:regular_payments:read\n    description: Read direct debits, scheduled payments, and instalment plans.\n    operations:\n      - listDirectDebits\n      - listDirectDebitsBulk\n      - listDirectDebitsSpecificAccounts\n      - listScheduledPayments\n      - listScheduledPaymentsBulk\n      - listScheduledPaymentsSpecificAccounts\n      - listInstalmentPlans\n      - listInstalmentPlansBulk\n\
  \  - name: bank:payees:read\n    description: Read saved payees.\n    operations:\n      - listBankingPayees\n      - getBankingPayeeDetail\n  - name: common:customer.basic:read\n    description: >-\n      Read basic customer identity information. Declared in the CDR common\n      standards for the customer endpoints; not present as an x-scopes value on\n      the banking paths in this spec but required in the CDR consent for\n      customer data.\n    operations: []\nnotes: >-\n  The public unauthenticated Product Reference Data surface (GET /banking/products\n  and GET /banking/products/{productId}) requires no OAuth scope. All scoped\n  operations are only exercisable by accredited data recipients registered with\n  the CDR Register; they are not callable from this public repo.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-military-bank/refs/heads/main/scopes/australian-military-bank-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual
- Defence
token_urls: []
---
