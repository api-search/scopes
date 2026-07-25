---
api_specs:
- filename: commonwealth-bank-accounts-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Accounts API API
  slug: commonwealth-bank-accounts-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-accounts-api-api-openapi.yml
- filename: commonwealth-bank-balances-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Balances API API
  slug: commonwealth-bank-balances-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-balances-api-api-openapi.yml
- filename: commonwealth-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Balances API
  slug: commonwealth-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-balances-api-openapi.yml
- filename: commonwealth-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Direct Debits API
  slug: commonwealth-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-direct-debits-api-openapi.yml
- filename: commonwealth-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Scheduled Payments API
  slug: commonwealth-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: commonwealth-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Transactions API
  slug: commonwealth-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-transactions-api-openapi.yml
- filename: commonwealth-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Accounts API
  slug: commonwealth-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-accounts-api-openapi.yml
- filename: commonwealth-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Payees API
  slug: commonwealth-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-payees-api-openapi.yml
- filename: commonwealth-bank-banking-products-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Products API
  slug: commonwealth-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-products-api-openapi.yml
- filename: commonwealth-bank-customer-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Customer API API
  slug: commonwealth-bank-customer-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-customer-api-api-openapi.yml
- filename: commonwealth-bank-payees-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Payees API API
  slug: commonwealth-bank-payees-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-payees-api-api-openapi.yml
- filename: commonwealth-bank-products-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Products API API
  slug: commonwealth-bank-products-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-products-api-api-openapi.yml
- filename: commonwealth-bank-regular-payments-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Regular Payments API API
  slug: commonwealth-bank-regular-payments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-regular-payments-api-api-openapi.yml
- filename: commonwealth-bank-transaction-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Transaction API API
  slug: commonwealth-bank-transaction-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-transaction-api-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Commonwealth Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Commonwealth Bank publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Commonwealth Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Commonwealth Bank
provider_slug: commonwealth-bank
schemes: []
scope_count: 10
scope_names:
- openid
- profile
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
- common:customer.basic:read
- common:customer.detail:read
- cdr:registration
scopes:
- description: OpenID Connect authentication of the consumer during the CDR consent flow.
  flows: []
  scope: openid
- description: Standard OIDC profile claims.
  flows: []
  scope: profile
- description: Account name, type, and balance (basic account data cluster).
  flows: []
  scope: bank:accounts.basic:read
- description: Account numbers and detailed features (detailed account data cluster).
  flows: []
  scope: bank:accounts.detail:read
- description: Transactions and details for authorised accounts.
  flows: []
  scope: bank:transactions:read
- description: Saved payees (payee data cluster).
  flows: []
  scope: bank:payees:read
- description: Direct debits and scheduled/recurring payments.
  flows: []
  scope: bank:regular_payments:read
- description: Customer name and occupation (basic customer data cluster).
  flows: []
  scope: common:customer.basic:read
- description: Customer contact details (detailed customer data cluster).
  flows: []
  scope: common:customer.detail:read
- description: Dynamic client registration management for the ADR software product.
  flows: []
  scope: cdr:registration
slug: commonwealth-bank-scopes
source_filename: commonwealth-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  Consumer Data Standards Australia (DSB) — CDR Banking authorisation scopes.\n  CommBank, as a designated CDR Data Holder, implements the standardised CDR\n  scope set for consumer-consented data sharing. The harvested Swagger specs do\n  not declare oauth2 flows, so scopes are authored from the CDR standard.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nflow: authorizationCode\nnotes: >-\n  CDR scopes map to data clusters presented to the consumer during consent. The\n  public Product Reference Data surface needs no scope. openid is required for\n  the OIDC authorisation.\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication of the consumer during the CDR consent flow.\n    data_cluster: identity\n  - scope: profile\n    description: Standard OIDC profile claims.\n    data_cluster: identity\n  - scope: bank:accounts.basic:read\n    description: Account name,\
  \ type, and balance (basic account data cluster).\n    data_cluster: account-basic\n    operations: [listAccounts, listBankingAccounts]\n  - scope: bank:accounts.detail:read\n    description: Account numbers and detailed features (detailed account data cluster).\n    data_cluster: account-detail\n    operations: [getAccountDetail, getBankingAccountDetail]\n  - scope: bank:transactions:read\n    description: Transactions and details for authorised accounts.\n    data_cluster: transactions\n    operations: [getTransactions, getTransactionDetail, listBankingTransactions, getBankingTransactionDetail]\n  - scope: bank:payees:read\n    description: Saved payees (payee data cluster).\n    data_cluster: payees\n    operations: [listPayees, getPayeeDetail, listBankingPayees, getBankingPayeeDetail]\n  - scope: bank:regular_payments:read\n    description: Direct debits and scheduled/recurring payments.\n    data_cluster: regular-payments\n    operations: [listDirectDebits, listDirectDebitsBulk, listScheduledPayments,\
  \ listScheduledPaymentsBulk]\n  - scope: common:customer.basic:read\n    description: Customer name and occupation (basic customer data cluster).\n    data_cluster: customer-basic\n    operations: [getCustomer]\n  - scope: common:customer.detail:read\n    description: Customer contact details (detailed customer data cluster).\n    data_cluster: customer-detail\n    operations: [getCustomerDetail]\n  - scope: cdr:registration\n    description: Dynamic client registration management for the ADR software product.\n    data_cluster: registration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/scopes/commonwealth-bank-scopes.yml
summary_line: 10 scopes
tags:
- Financial
- Banks
- Consumer Banking
- Business Banking
- Open Banking
- CDR
- Product Reference Data
- ADI
- Australia
token_urls: []
---
