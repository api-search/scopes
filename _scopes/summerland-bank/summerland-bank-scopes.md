---
api_specs:
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Product Reference Data API
  slug: summerland-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Accounts & Balances API
  slug: summerland-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Transactions API
  slug: summerland-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Direct Debits & Scheduled Payments API
  slug: summerland-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
- filename: summerland-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Summerland Bank CDR Payees API
  slug: summerland-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-cds-banking-products-openapi.yml
authorization_urls:
- discovered-per-holder-via-oidc (/.well-known/openid-configuration on the CDR Resource/Auth base)
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Summerland Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Summerland Bank publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Summerland Bank API on a user''s behalf.


  Tokens are issued from discovered-per-holder-via-oidc.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Summerland Bank
provider_slug: summerland-bank
schemes:
- flows:
  - authorizationUrl: discovered-per-holder-via-oidc (/.well-known/openid-configuration on the CDR Resource/Auth base)
    flow: authorizationCode
    note: Endpoints served on the bank's authenticated CDR Resource Base URI (register-discovered by accredited data recipients). Authorization and token endpoints are resolved through the holder's OIDC discovery document, not published on the public PRD host.
    tokenUrl: discovered-per-holder-via-oidc
  name: CDR-InfoSec-OAuth2
  profile: CDR InfoSec profile (FAPI 1.0 Advanced, OIDC Hybrid/PKCE, PAR, MTLS-bound tokens)
  source: openapi/summerland-bank-cds-banking-products-openapi.yml
  type: oauth2
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Read basic account information — account name, type, balance and masked account number (Get Accounts, Get Account Balance, Get Bulk Balances, Get Balances For Specific Accounts).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account information including account numbers, features, fees, and specific account terms (Get Account Detail).
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read account transactions and transaction detail, with amount/date/text filters (Get Transactions For Account, Get Transaction Detail).
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read regular payments — direct debits, scheduled payments, and instalment plans (Get Direct Debits, Get Scheduled Payments, Get Instalment Plans and their bulk/specific-account variants).
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
- description: Read the consumer's saved payees — domestic, international, and BPAY (Get Payees, Get Payee Detail).
  flows:
  - authorizationCode
  scope: bank:payees:read
slug: summerland-bank-scopes
source_filename: summerland-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/summerland-bank-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnotes: >-\n  OAuth2 authorisation scopes for Summerland Bank's consumer-authorized CDR\n  banking endpoints. The harvested DSB Consumer Data Standards Banking OpenAPI\n  declares no `securitySchemes`, but each authenticated operation carries an\n  `x-scopes` extension naming the CDR banking scope it requires; those scopes are\n  the standard Consumer Data Right banking scopes defined by the Data Standards\n  Body. Authorisation is obtained through the CDR InfoSec profile (FAPI 1.0\n  Advanced OAuth2 authorization-code + OpenID Connect, MTLS-bound tokens),\n  discovered per data holder via OIDC — not a bank-published authorization/token\n  URL. The public Product Reference Data endpoints (listBankingProducts,\n  getBankingProductDetail) require no scope (unauthenticated).\nschemes:\n\
  \  - name: CDR-InfoSec-OAuth2\n    type: oauth2\n    source: openapi/summerland-bank-cds-banking-products-openapi.yml\n    profile: CDR InfoSec profile (FAPI 1.0 Advanced, OIDC Hybrid/PKCE, PAR, MTLS-bound tokens)\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: discovered-per-holder-via-oidc (/.well-known/openid-configuration on the CDR Resource/Auth base)\n        tokenUrl: discovered-per-holder-via-oidc\n        note: >-\n          Endpoints served on the bank's authenticated CDR Resource Base URI\n          (register-discovered by accredited data recipients). Authorization and\n          token endpoints are resolved through the holder's OIDC discovery\n          document, not published on the public PRD host.\nscopes:\n  - scope: bank:accounts.basic:read\n    description: >-\n      Read basic account information — account name, type, balance and masked\n      account number (Get Accounts, Get Account Balance, Get Bulk Balances,\n      Get Balances For Specific\
  \ Accounts).\n    flows: [authorizationCode]\n    operations:\n      - listBankingAccounts\n      - listBankingBalancesBulk\n      - listBankingBalancesSpecificAccounts\n      - getBankingBalance\n    sources: [openapi/summerland-bank-cds-banking-products-openapi.yml]\n  - scope: bank:accounts.detail:read\n    description: >-\n      Read detailed account information including account numbers, features,\n      fees, and specific account terms (Get Account Detail).\n    flows: [authorizationCode]\n    operations:\n      - getBankingAccountDetail\n    sources: [openapi/summerland-bank-cds-banking-products-openapi.yml]\n  - scope: bank:transactions:read\n    description: >-\n      Read account transactions and transaction detail, with amount/date/text\n      filters (Get Transactions For Account, Get Transaction Detail).\n    flows: [authorizationCode]\n    operations:\n      - listBankingTransactions\n      - getBankingTransactionDetail\n    sources: [openapi/summerland-bank-cds-banking-products-openapi.yml]\n\
  \  - scope: bank:regular_payments:read\n    description: >-\n      Read regular payments — direct debits, scheduled payments, and instalment\n      plans (Get Direct Debits, Get Scheduled Payments, Get Instalment Plans and\n      their bulk/specific-account variants).\n    flows: [authorizationCode]\n    operations:\n      - listDirectDebits\n      - listDirectDebitsBulk\n      - listDirectDebitsSpecificAccounts\n      - listScheduledPayments\n      - listScheduledPaymentsBulk\n      - listScheduledPaymentsSpecificAccounts\n      - listInstalmentPlans\n      - listInstalmentPlansBulk\n    sources: [openapi/summerland-bank-cds-banking-products-openapi.yml]\n  - scope: bank:payees:read\n    description: >-\n      Read the consumer's saved payees — domestic, international, and BPAY\n      (Get Payees, Get Payee Detail).\n    flows: [authorizationCode]\n    operations:\n      - listBankingPayees\n      - getBankingPayeeDetail\n    sources: [openapi/summerland-bank-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/scopes/summerland-bank-scopes.yml
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
token_urls:
- discovered-per-holder-via-oidc
---
