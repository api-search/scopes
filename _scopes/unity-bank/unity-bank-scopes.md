---
api_specs:
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Product Reference Data API
  slug: unity-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Accounts & Balances API
  slug: unity-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Transactions API
  slug: unity-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Direct Debits & Scheduled Payments API
  slug: unity-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
- filename: unity-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Unity Bank CDR Payees API
  slug: unity-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/openapi/unity-bank-cds-banking-products-openapi.yml
authorization_urls:
- discovered-via-cdr-register
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Unity Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Unity Bank publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unity Bank API on a user''s behalf.


  Tokens are issued from discovered-via-cdr-register.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unity Bank
provider_slug: unity-bank
schemes:
- flows:
  - authorizationUrl: discovered-via-cdr-register
    client_auth:
    - mtls
    - private_key_jwt
    consent: member-authorized
    flow: authorizationCode
    par: true
    tokenUrl: discovered-via-cdr-register
  name: CDR-OIDC-FAPI
  profile: FAPI 2.0 (CDR Security Profile)
  source: openapi/unity-bank-cds-banking-products-openapi.yml
  type: oauth2
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
scopes:
- description: Read basic account information - account name, type, balance and masked account number - for accounts the member has consented to share.
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account information - full account numbers, features, fees, deposit/lending rates, address and other account detail - for consented accounts.
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read transactions for consented accounts, with date, amount and text filtering.
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read the member's saved payees (name, type, and payee detail) for consented data.
  flows:
  - authorizationCode
  scope: bank:payees:read
- description: Read regular payment arrangements - direct debits and scheduled/recurring payments - for consented accounts.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
slug: unity-bank-scopes
source_filename: unity-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unity-bank-cds-banking-products-openapi.yml (x-scopes)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnotes: >-\n  Unity Bank is a CDR data holder. The public Product Reference Data surface is\n  unauthenticated, but the broader consumer-authorized CDR Banking surface\n  (Accounts, Balances, Transactions, Payees, Direct Debits & Scheduled Payments)\n  is protected by the CDR OIDC/FAPI 2.0 authorization model. The scopes below are\n  the standard DSB Consumer Data Right banking authorisation scopes carried as\n  x-scopes on the operations in the harvested shared CDR Banking API (v1.36.0) and\n  enriched from the published Consumer Data Standards authorisation-scopes\n  reference. Authorization and token endpoints are not fixed URLs: an Accredited\n  Data Recipient discovers the data holder's OIDC configuration dynamically via the\n  CDR Register, then completes a PAR + mTLS /\
  \ private_key_jwt FAPI authorization\n  flow after member consent. No public authorization-server metadata is exposed\n  (well-known probe returned 404, as expected for a data holder behind the Register).\nschemes:\n- name: CDR-OIDC-FAPI\n  type: oauth2\n  profile: FAPI 2.0 (CDR Security Profile)\n  source: openapi/unity-bank-cds-banking-products-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: discovered-via-cdr-register\n    tokenUrl: discovered-via-cdr-register\n    par: true\n    client_auth: [mtls, private_key_jwt]\n    consent: member-authorized\nscopes:\n- scope: bank:accounts.basic:read\n  description: >-\n    Read basic account information - account name, type, balance and masked\n    account number - for accounts the member has consented to share.\n  flows: [authorizationCode]\n  operations: [listBankingAccounts, getBankingBalance, listBankingBalancesBulk, listBankingBalancesSpecificAccounts]\n  sources: [openapi/unity-bank-cds-banking-products-openapi.yml]\n\
  - scope: bank:accounts.detail:read\n  description: >-\n    Read detailed account information - full account numbers, features, fees,\n    deposit/lending rates, address and other account detail - for consented accounts.\n  flows: [authorizationCode]\n  operations: [getBankingAccountDetail]\n  sources: [openapi/unity-bank-cds-banking-products-openapi.yml]\n- scope: bank:transactions:read\n  description: >-\n    Read transactions for consented accounts, with date, amount and text filtering.\n  flows: [authorizationCode]\n  operations: [listBankingTransactions, getBankingTransactionDetail]\n  sources: [openapi/unity-bank-cds-banking-products-openapi.yml]\n- scope: bank:payees:read\n  description: >-\n    Read the member's saved payees (name, type, and payee detail) for consented data.\n  flows: [authorizationCode]\n  operations: [listBankingPayees, getBankingPayeeDetail]\n  sources: [openapi/unity-bank-cds-banking-products-openapi.yml]\n- scope: bank:regular_payments:read\n  description:\
  \ >-\n    Read regular payment arrangements - direct debits and scheduled/recurring\n    payments - for consented accounts.\n  flows: [authorizationCode]\n  operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts]\n  sources: [openapi/unity-bank-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unity-bank/refs/heads/main/scopes/unity-bank-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
token_urls:
- discovered-via-cdr-register
---
