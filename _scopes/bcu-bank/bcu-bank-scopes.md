---
api_specs:
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Product Reference Data API
  slug: bcu-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Accounts & Balances API
  slug: bcu-bank-cdr-accounts-and-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Transactions API
  slug: bcu-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Direct Debits & Scheduled Payments API
  slug: bcu-bank-cdr-direct-debits-and-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
- filename: bcu-bank-cds-banking-products-openapi.yml
  format: yaml
  label: BCU Bank CDR Payees API
  slug: bcu-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/openapi/bcu-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Bcu Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BCU Bank publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BCU Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BCU Bank
provider_slug: bcu-bank
schemes:
- flows:
  - flow: authorizationCode
  name: OAuth2 (CDR authorization-code + PKCE, FAPI 1.0 Advanced)
  source: DSB Consumer Data Standards Security Profile
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Read basic account information (account list, product category, masked account number, balances).
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information including features, fees, terms and account-holder details.
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions and transaction detail.
  flows: []
  scope: bank:transactions:read
- description: Read regular payments - direct debits, scheduled payments and instalment plans.
  flows: []
  scope: bank:regular_payments:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
slug: bcu-bank-scopes
source_filename: bcu-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/bcu-bank-cds-banking-products-openapi.yml (per-operation x-scopes)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnotes: >-\n  The CDS Banking OpenAPI declares no components.securitySchemes, so the OAuth\n  scope surface is derived from the per-operation x-scopes extension in the spec\n  and enriched from the DSB Consumer Data Standards authorisation-scopes\n  reference. These are the standardised CDR banking data-cluster scopes granted\n  through the CDR consent flow to Accredited Data Recipients. The Product\n  Reference Data endpoints (listBankingProducts, getBankingProductDetail) are\n  public and require no scope.\nschemes:\n- name: OAuth2 (CDR authorization-code + PKCE, FAPI 1.0 Advanced)\n  source: DSB Consumer Data Standards Security Profile\n  flows:\n  - flow: authorizationCode\nscopes:\n- scope: bank:accounts.basic:read\n  description: Read basic account information\
  \ (account list, product category, masked account number, balances).\n  operations:\n  - listBankingAccounts\n  - listBankingBalancesBulk\n  - listBankingBalancesSpecificAccounts\n  - getBankingBalance\n- scope: bank:accounts.detail:read\n  description: Read detailed account information including features, fees, terms and account-holder details.\n  operations:\n  - getBankingAccountDetail\n- scope: bank:transactions:read\n  description: Read account transactions and transaction detail.\n  operations:\n  - listBankingTransactions\n  - getBankingTransactionDetail\n- scope: bank:regular_payments:read\n  description: Read regular payments - direct debits, scheduled payments and instalment plans.\n  operations:\n  - listDirectDebits\n  - listDirectDebitsBulk\n  - listDirectDebitsSpecificAccounts\n  - listScheduledPayments\n  - listScheduledPaymentsBulk\n  - listScheduledPaymentsSpecificAccounts\n  - listInstalmentPlans\n  - listInstalmentPlansBulk\n- scope: bank:payees:read\n  description:\
  \ Read saved payees.\n  operations:\n  - listBankingPayees\n  - getBankingPayeeDetail\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bcu-bank/refs/heads/main/scopes/bcu-bank-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Mutual Bank
- Australia
token_urls: []
---
