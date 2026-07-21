---
api_specs:
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Product Reference Data API
  slug: st-george-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Accounts & Balances API
  slug: st-george-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Transactions API
  slug: st-george-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Direct Debits & Scheduled Payments API
  slug: st-george-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
- filename: st-george-bank-cds-banking-products-openapi.yml
  format: yaml
  label: St.George Bank CDR Payees API
  slug: st-george-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/openapi/st-george-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#end-user-authorisation
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: St George Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'St.George Bank publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the St.George Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: St.George Bank
provider_slug: st-george-bank
schemes:
- detail: Scopes are granted through the CDR consent flow (accredited Data Recipients only) and bind a sharing arrangement. openid + profile are requested alongside the CDR data scopes.
  name: CDR-OAuth2
  profile: FAPI 1.0 Advanced
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
- description: OpenID Connect authentication (id_token).
  flows:
  - authorizationCode
  scope: openid
- description: OpenID Connect basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Read account identifiers, product association and basic account attributes (balances excluded).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account information (features, rates, addresses); additive to bank:accounts.basic:read.
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read transactions for consented accounts.
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read saved payees.
  flows:
  - authorizationCode
  scope: bank:payees:read
- description: Read direct debits, scheduled payments and instalment plans.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
- description: Read basic customer data (name / organisation).
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read detailed customer data (contact details); additive to common:customer.basic:read.
  flows:
  - authorizationCode
  scope: common:customer.detail:read
slug: st-george-bank-scopes
source_filename: st-george-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  The harvested OpenAPI declares no oauth2 securitySchemes (shared DSB \"CDR\n  Banking API\" doc), so scopes cannot be derived from the spec. The scope set\n  below is the standard Consumer Data Right banking authorisation scope\n  registry defined by the DSB Consumer Data Standards, which St.George (a\n  Westpac CDR Data Holder) accepts on consented data-sharing requests.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#end-user-authorisation\nreference: https://cdr-support.zendesk.com/hc/en-us/articles/900004582823-Requirement-for-Basic-and-Detailed-Scopes\nschemes:\n  - name: CDR-OAuth2\n    profile: FAPI 1.0 Advanced\n    detail: >-\n      Scopes are granted through the CDR consent flow (accredited Data\n      Recipients only) and bind a sharing arrangement. openid + profile are\n      requested alongside the CDR data scopes.\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication\
  \ (id_token).\n    flows: [authorizationCode]\n  - scope: profile\n    description: OpenID Connect basic profile claims.\n    flows: [authorizationCode]\n  - scope: bank:accounts.basic:read\n    description: Read account identifiers, product association and basic account attributes (balances excluded).\n    flows: [authorizationCode]\n    operations: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n  - scope: bank:accounts.detail:read\n    description: Read detailed account information (features, rates, addresses); additive to bank:accounts.basic:read.\n    flows: [authorizationCode]\n    operations: [getBankingAccountDetail]\n  - scope: bank:transactions:read\n    description: Read transactions for consented accounts.\n    flows: [authorizationCode]\n    operations: [listBankingTransactions, getBankingTransactionDetail]\n  - scope: bank:payees:read\n    description: Read saved payees.\n    flows: [authorizationCode]\n    operations:\
  \ [listBankingPayees, getBankingPayeeDetail]\n  - scope: bank:regular_payments:read\n    description: Read direct debits, scheduled payments and instalment plans.\n    flows: [authorizationCode]\n    operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n  - scope: common:customer.basic:read\n    description: Read basic customer data (name / organisation).\n    flows: [authorizationCode]\n  - scope: common:customer.detail:read\n    description: Read detailed customer data (contact details); additive to common:customer.basic:read.\n    flows: [authorizationCode]\nnotes: >-\n  Product Reference Data (listBankingProducts / getBankingProductDetail) is\n  public and requires no scope. detail:read scopes only take effect when the\n  matching basic:read scope is also granted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/st-george-bank/refs/heads/main/scopes/st-george-bank-scopes.yml
summary_line: 9 scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Westpac Group
token_urls: []
---
