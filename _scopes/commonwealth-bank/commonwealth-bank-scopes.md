---
api_specs:
- filename: commonwealth-bank-accounts-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Accounts API
  slug: commonwealth-bank-accounts-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-accounts-api-api-openapi.yml
- filename: commonwealth-bank-balances-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Balances API
  slug: commonwealth-bank-balances-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-balances-api-api-openapi.yml
- filename: commonwealth-bank-customer-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Customer API
  slug: commonwealth-bank-customer-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-customer-api-api-openapi.yml
- filename: commonwealth-bank-payees-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Payees API
  slug: commonwealth-bank-payees-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-payees-api-api-openapi.yml
- filename: commonwealth-bank-products-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Products API
  slug: commonwealth-bank-products-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-products-api-api-openapi.yml
- filename: commonwealth-bank-regular-payments-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Regular Payments API
  slug: commonwealth-bank-regular-payments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-regular-payments-api-api-openapi.yml
- filename: commonwealth-bank-transaction-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Transaction API
  slug: commonwealth-bank-transaction-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-transaction-api-api-openapi.yml
- filename: commonwealth-bank-accounts-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Accounts API
  slug: commonwealth-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-accounts-api-openapi.yml
- filename: commonwealth-bank-agreements-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Agreements API
  slug: commonwealth-bank-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-agreements-api-openapi.yml
- filename: commonwealth-bank-credit-transfer-initiations-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Credit Transfer Initiations API
  slug: commonwealth-bank-credit-transfer-initiations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-credit-transfer-initiations-api-openapi.yml
- filename: commonwealth-bank-discovery-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Discovery API
  slug: commonwealth-bank-discovery-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-discovery-api-api-openapi.yml
- filename: commonwealth-bank-partner-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Partner API
  slug: commonwealth-bank-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-partner-api-openapi.yml
- filename: commonwealth-bank-payments-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Payments API
  slug: commonwealth-bank-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-payments-api-openapi.yml
- filename: commonwealth-bank-utilities-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Utilities API
  slug: commonwealth-bank-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-utilities-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Commonwealth Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Commonwealth Bank publishes 18 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Commonwealth Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Commonwealth Bank
provider_slug: commonwealth-bank
schemes: []
scope_count: 18
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
- payments:namecheck:read
- payments:agreements:read
- payments:agreements:write
- payments:agreements:amend
- payments:payments:read
- payments:payments:write
- payment-initiation.core-payments.payment-order-initiation.write
- foreign-exchange.partner-quote.read-execute
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
- description: NameCheck scope listed in the OAuth API scopes table
  flows: []
  scope: payments:namecheck:read
- description: PayTo scope listed in the OAuth API scopes table
  flows: []
  scope: payments:agreements:read
- description: PayTo scope listed in the OAuth API scopes table
  flows: []
  scope: payments:agreements:write
- description: PayTo scope listed in the OAuth API scopes table
  flows: []
  scope: payments:agreements:amend
- description: PayTo scope listed in the OAuth API scopes table
  flows: []
  scope: payments:payments:read
- description: PayTo scope listed in the OAuth API scopes table
  flows: []
  scope: payments:payments:write
- description: Fast Payments scope listed in the OAuth API scopes table
  flows: []
  scope: payment-initiation.core-payments.payment-order-initiation.write
- description: FX API scope listed in the OAuth API scopes table
  flows: []
  scope: foreign-exchange.partner-quote.read-execute
slug: commonwealth-bank-scopes
source_filename: commonwealth-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: Consumer Data Standards Australia (DSB) — CDR Banking authorisation scopes. CommBank, as a designated CDR\n  Data Holder, implements the standardised CDR scope set for consumer-consented data sharing. The harvested Swagger\n  specs do not declare oauth2 flows, so scopes are authored from the CDR standard.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nflow: authorizationCode\nnotes: CDR scopes map to data clusters presented to the consumer during consent. The public Product Reference Data\n  surface needs no scope. openid is required for the OIDC authorisation.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication of the consumer during the CDR consent flow.\n  data_cluster: identity\n- scope: profile\n  description: Standard OIDC profile claims.\n  data_cluster: identity\n- scope: bank:accounts.basic:read\n  description: Account name, type, and balance (basic account\
  \ data cluster).\n  data_cluster: account-basic\n  operations:\n  - listAccounts\n  - listBankingAccounts\n- scope: bank:accounts.detail:read\n  description: Account numbers and detailed features (detailed account data cluster).\n  data_cluster: account-detail\n  operations:\n  - getAccountDetail\n  - getBankingAccountDetail\n- scope: bank:transactions:read\n  description: Transactions and details for authorised accounts.\n  data_cluster: transactions\n  operations:\n  - getTransactions\n  - getTransactionDetail\n  - listBankingTransactions\n  - getBankingTransactionDetail\n- scope: bank:payees:read\n  description: Saved payees (payee data cluster).\n  data_cluster: payees\n  operations:\n  - listPayees\n  - getPayeeDetail\n  - listBankingPayees\n  - getBankingPayeeDetail\n- scope: bank:regular_payments:read\n  description: Direct debits and scheduled/recurring payments.\n  data_cluster: regular-payments\n  operations:\n  - listDirectDebits\n  - listDirectDebitsBulk\n  - listScheduledPayments\n\
  \  - listScheduledPaymentsBulk\n- scope: common:customer.basic:read\n  description: Customer name and occupation (basic customer data cluster).\n  data_cluster: customer-basic\n  operations:\n  - getCustomer\n- scope: common:customer.detail:read\n  description: Customer contact details (detailed customer data cluster).\n  data_cluster: customer-detail\n  operations:\n  - getCustomerDetail\n- scope: cdr:registration\n  description: Dynamic client registration management for the ADR software product.\n  data_cluster: registration\n- scope: payments:namecheck:read\n  api: NameCheck\n  flow: clientCredentials\n  description: NameCheck scope listed in the OAuth API scopes table\n  source: https://docs.commbank.com.au/learners/security-and-getting-access/authentication\n- scope: payments:agreements:read\n  api: PayTo\n  flow: clientCredentials\n  description: PayTo scope listed in the OAuth API scopes table\n  source: https://docs.commbank.com.au/learners/security-and-getting-access/authentication\n\
  - scope: payments:agreements:write\n  api: PayTo\n  flow: clientCredentials\n  description: PayTo scope listed in the OAuth API scopes table\n  source: https://docs.commbank.com.au/learners/security-and-getting-access/authentication\n- scope: payments:agreements:amend\n  api: PayTo\n  flow: clientCredentials\n  description: PayTo scope listed in the OAuth API scopes table\n  source: https://docs.commbank.com.au/learners/security-and-getting-access/authentication\n- scope: payments:payments:read\n  api: PayTo\n  flow: clientCredentials\n  description: PayTo scope listed in the OAuth API scopes table\n  source: https://docs.commbank.com.au/learners/security-and-getting-access/authentication\n- scope: payments:payments:write\n  api: PayTo\n  flow: clientCredentials\n  description: PayTo scope listed in the OAuth API scopes table\n  source: https://docs.commbank.com.au/learners/security-and-getting-access/authentication\n- scope: payment-initiation.core-payments.payment-order-initiation.write\n\
  \  api: Fast Payments\n  flow: clientCredentials\n  description: Fast Payments scope listed in the OAuth API scopes table\n  source: https://docs.commbank.com.au/learners/security-and-getting-access/authentication\n- scope: foreign-exchange.partner-quote.read-execute\n  api: FX API\n  flow: clientCredentials\n  description: FX API scope listed in the OAuth API scopes table\n  source: https://docs.commbank.com.au/learners/security-and-getting-access/authentication\nbusiness_api_docs: https://docs.commbank.com.au/learners/security-and-getting-access/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/scopes/commonwealth-bank-scopes.yml
summary_line: 18 scopes · authorizationCode
tags:
- Finance
- Banks
- Consumer Banking
- Business Banking
- Open Banking
- CDR
- Product Reference Data
- ADI
- Australia
token_bound: false
token_urls: []
---
