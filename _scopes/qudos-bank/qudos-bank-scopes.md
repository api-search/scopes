---
api_specs:
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Product Reference Data API
  slug: qudos-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Accounts & Balances API
  slug: qudos-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Transactions API
  slug: qudos-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Direct Debits & Scheduled Payments API
  slug: qudos-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
- filename: qudos-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Qudos Bank CDR Payees API
  slug: qudos-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/openapi/qudos-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Qudos Bank Scopes
name_suffix: OAuth Scopes
note: The public Product Reference Data operations (listBankingProducts, getBankingProductDetail) are unauthenticated and carry no scope. All other CDR banking operations require an ACCC-accredited data recipient to hold the scope shown, granted via the customer's CDR consent under the Data Standards Body FAPI security profile (OAuth 2.0 authorization code + OIDC, PKCE/PAR, mutual TLS). Scopes and their consumer-facing data-language descriptions are standardized across all Australian ADIs by the Consumer Data Standards; they are not Qudos-specific. Discovery/trust is brokered by the ACCC CDR Register, not a per-holder /.well-known/openid-configuration.
overview: 'Qudos Bank publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Qudos Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Qudos Bank
provider_slug: qudos-bank
schemes:
- flow: authorizationCode
  name: cdr-fapi
  profile: FAPI 1.0 Advanced / FAPI 2.0
  register: https://consumerdatastandardsaustralia.github.io/register/
  source: openapi/qudos-bank-cds-banking-products-openapi.yml
  transport: mutualTLS
  type: oauth2
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
scopes:
- description: Account name, type, and balance. Grants the basic banking account list and balance surface.
  flows: []
  scope: bank:accounts.basic:read
- description: Account numbers and features (account balance and details, including account number, interest rates, fees, and features).
  flows: []
  scope: bank:accounts.detail:read
- description: Transaction details, including incoming and outgoing transactions, amounts, dates, descriptions, and other party details.
  flows: []
  scope: bank:transactions:read
- description: Saved payees, including names and account/BSB or PayID details of the member's saved payees.
  flows: []
  scope: bank:payees:read
- description: Direct debits and scheduled payments, including recurring-payment arrangements and instalment plans.
  flows: []
  scope: bank:regular_payments:read
slug: qudos-bank-scopes
source_filename: qudos-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/qudos-bank-cds-banking-products-openapi.yml (per-operation x-scopes)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  The public Product Reference Data operations (listBankingProducts,\n  getBankingProductDetail) are unauthenticated and carry no scope. All other\n  CDR banking operations require an ACCC-accredited data recipient to hold the\n  scope shown, granted via the customer's CDR consent under the Data Standards\n  Body FAPI security profile (OAuth 2.0 authorization code + OIDC, PKCE/PAR,\n  mutual TLS). Scopes and their consumer-facing data-language descriptions are\n  standardized across all Australian ADIs by the Consumer Data Standards; they\n  are not Qudos-specific. Discovery/trust is brokered by the ACCC CDR Register,\n  not a per-holder /.well-known/openid-configuration.\nschemes:\n- name: cdr-fapi\n  type: oauth2\n  flow: authorizationCode\n  profile:\
  \ FAPI 1.0 Advanced / FAPI 2.0\n  transport: mutualTLS\n  source: openapi/qudos-bank-cds-banking-products-openapi.yml\n  register: https://consumerdatastandardsaustralia.github.io/register/\nscopes:\n- scope: bank:accounts.basic:read\n  description: >-\n    Account name, type, and balance. Grants the basic banking account list and\n    balance surface.\n  operations: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n  sources: [openapi/qudos-bank-cds-banking-products-openapi.yml]\n- scope: bank:accounts.detail:read\n  description: >-\n    Account numbers and features (account balance and details, including\n    account number, interest rates, fees, and features).\n  operations: [getBankingAccountDetail]\n  sources: [openapi/qudos-bank-cds-banking-products-openapi.yml]\n- scope: bank:transactions:read\n  description: >-\n    Transaction details, including incoming and outgoing transactions, amounts,\n    dates, descriptions, and other\
  \ party details.\n  operations: [listBankingTransactions, getBankingTransactionDetail]\n  sources: [openapi/qudos-bank-cds-banking-products-openapi.yml]\n- scope: bank:payees:read\n  description: >-\n    Saved payees, including names and account/BSB or PayID details of the\n    member's saved payees.\n  operations: [listBankingPayees, getBankingPayeeDetail]\n  sources: [openapi/qudos-bank-cds-banking-products-openapi.yml]\n- scope: bank:regular_payments:read\n  description: >-\n    Direct debits and scheduled payments, including recurring-payment\n    arrangements and instalment plans.\n  operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n  sources: [openapi/qudos-bank-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qudos-bank/refs/heads/main/scopes/qudos-bank-scopes.yml
summary_line: 5 scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Mutual Bank
- Product Reference Data
token_urls: []
---
