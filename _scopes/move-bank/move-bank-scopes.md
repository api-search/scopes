---
api_specs:
- filename: move-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: MOVE Bank Banking Account Balances API
  slug: move-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-banking-account-balances-api-openapi.yml
- filename: move-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: MOVE Bank Banking Account Direct Debits API
  slug: move-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-banking-account-direct-debits-api-openapi.yml
- filename: move-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: MOVE Bank Banking Account Scheduled Payments API
  slug: move-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: move-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: MOVE Bank Banking Account Transactions API
  slug: move-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-banking-account-transactions-api-openapi.yml
- filename: move-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: MOVE Bank Banking Accounts API
  slug: move-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-banking-accounts-api-openapi.yml
- filename: move-bank-banking-payees-api-openapi.yml
  format: yaml
  label: MOVE Bank Banking Payees API
  slug: move-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-banking-payees-api-openapi.yml
- filename: move-bank-banking-products-api-openapi.yml
  format: yaml
  label: MOVE Bank Banking Products API
  slug: move-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/openapi/move-bank-banking-products-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Move Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MOVE Bank publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the MOVE Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MOVE Bank
provider_slug: move-bank
schemes: []
scope_count: 9
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
scopes:
- description: OpenID Connect authentication; required to establish the CDR authorisation.
  flows: []
  scope: openid
- description: Standard OIDC profile claims within the CDR identity assertion.
  flows: []
  scope: profile
- description: Read account name, type, and balance. Grants the bulk/specific balance operations and the account list without full account numbers.
  flows: []
  scope: bank:accounts.basic:read
- description: Read full account detail including account/BSB numbers and product features.
  flows: []
  scope: bank:accounts.detail:read
- description: Read transaction history and individual transaction detail for consented accounts.
  flows: []
  scope: bank:transactions:read
- description: Read the consumer's saved payees and payee detail.
  flows: []
  scope: bank:payees:read
- description: Read direct debit authorisations and scheduled/recurring payment arrangements.
  flows: []
  scope: bank:regular_payments:read
- description: Read the consumer's basic customer profile (name, occupation).
  flows: []
  scope: common:customer.basic:read
- description: Read the consumer's detailed contact information (address, phone, email).
  flows: []
  scope: common:customer.detail:read
slug: move-bank-scopes
source_filename: move-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nsource: >\n  Consumer Data Standards (Data Standards Body) authorisation-scopes registry +\n  CDR Security Profile. The harvested OpenAPI (shared DSB CDR Banking API v1.36.0)\n  declares no oauth2 securitySchemes, so derive-oauth-scopes.py yields nothing;\n  the scopes below are the standardised CDR data-cluster scopes that govern\n  MOVE Bank's consumer-data-sharing surface, mapped to the operations in\n  openapi/move-bank-cds-banking-products-openapi.yml. These are shared,\n  ecosystem-wide CDR scopes, not MOVE Bank-proprietary values.\nmodel: cdr-security-profile\nflow: >\n  OpenID Connect Hybrid flow under the CDR Security Profile (FAPI 1.0 Advanced-based)\n  with PAR, PKCE, private_key_jwt and mutual-TLS holder-of-key. Consent is captured\n  by data cluster; the resulting access token carries the scopes below. The public\n  Product Reference\
  \ Data operations (listBankingProducts, getBankingProductDetail)\n  require NO scope and NO token.\nscopes:\n- scope: openid\n  cluster: identity\n  description: OpenID Connect authentication; required to establish the CDR authorisation.\n  operations: []\n- scope: profile\n  cluster: identity\n  description: Standard OIDC profile claims within the CDR identity assertion.\n  operations: []\n- scope: bank:accounts.basic:read\n  cluster: Account balance and details (basic)\n  description: >\n    Read account name, type, and balance. Grants the bulk/specific balance\n    operations and the account list without full account numbers.\n  operations: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n- scope: bank:accounts.detail:read\n  cluster: Account balance and details\n  description: >\n    Read full account detail including account/BSB numbers and product features.\n  operations: [getBankingAccountDetail]\n- scope: bank:transactions:read\n\
  \  cluster: Transaction details\n  description: Read transaction history and individual transaction detail for consented accounts.\n  operations: [listBankingTransactions, getBankingTransactionDetail]\n- scope: bank:payees:read\n  cluster: Saved payees\n  description: Read the consumer's saved payees and payee detail.\n  operations: [listBankingPayees, getBankingPayeeDetail]\n- scope: bank:regular_payments:read\n  cluster: Direct debits and scheduled payments\n  description: >\n    Read direct debit authorisations and scheduled/recurring payment arrangements.\n  operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts]\n- scope: common:customer.basic:read\n  cluster: Name and occupation\n  description: Read the consumer's basic customer profile (name, occupation).\n  operations: []\n- scope: common:customer.detail:read\n  cluster: Contact details\n  description: Read the\
  \ consumer's detailed contact information (address, phone, email).\n  operations: []\nnotes: >\n  Product Reference Data (PRD) is public and scope-free. All scoped operations\n  require ACCC accreditation as a Data Recipient plus explicit consumer consent\n  under the CDR consent model; scope grants are bounded by the consent duration\n  and the data clusters the consumer selected. Instalment-plan operations\n  (listInstalmentPlans*) sit within the accounts data clusters. See\n  authentication/move-bank-authentication.yml for the transport/token profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/move-bank/refs/heads/main/scopes/move-bank-scopes.yml
summary_line: 9 scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Mutual Bank
- Australia
- Product Reference Data
token_urls: []
---
