---
api_specs:
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Product Reference Data API
  slug: ing-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Accounts & Balances API
  slug: ing-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Transactions API
  slug: ing-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Direct Debits & Scheduled Payments API
  slug: ing-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Payees API
  slug: ing-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
authorization_urls:
- https://id.ob.ing.com.au/authorize
description: OAuth2 / OIDC scopes advertised in ING Australia's live CDR OpenID Provider metadata (scopes_supported). These are the standard Consumer Data Standards (CDS) banking and common authorisation scopes granted to Accredited Data Recipients through the CDR consent flow. The public PRD endpoints require no scope; every other endpoint requires the mapped bank:* scope (see x-scopes in the OpenAPI). Descriptions and endpoint mappings are from the CDS authorisation scopes reference.
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ing Australia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ING Australia publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ING Australia API on a user''s behalf.


  Tokens are issued from https://secure.ob.ing.com.au/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ING Australia
provider_slug: ing-australia
schemes:
- flows:
  - authorizationUrl: https://id.ob.ing.com.au/authorize
    flow: authorizationCode
    tokenUrl: https://secure.ob.ing.com.au/token
  name: CDR-OAuth2
  source: well-known/ing-australia-openid-configuration.json
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
- description: OpenID Connect authentication; issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Basic OIDC profile claims (name, given_name, family_name).
  flows:
  - authorizationCode
  scope: profile
- description: Read basic account information and balances (list/detail without full account numbers).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account information including account numbers and features.
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read account transactions and transaction detail.
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read the customer's saved/registered payees.
  flows:
  - authorizationCode
  scope: bank:payees:read
- description: Read direct debits, scheduled payments and instalment plans.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
- description: Read basic customer information (name, occupation / organisation basics).
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read detailed customer information including contact details.
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: Dynamic client registration management for the Accredited Data Recipient's software product.
  flows:
  - clientCredentials
  scope: cdr:registration
slug: ing-australia-scopes
source_filename: ing-australia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://id.ob.ing.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\ndescription: >-\n  OAuth2 / OIDC scopes advertised in ING Australia's live CDR OpenID Provider\n  metadata (scopes_supported). These are the standard Consumer Data Standards\n  (CDS) banking and common authorisation scopes granted to Accredited Data\n  Recipients through the CDR consent flow. The public PRD endpoints require no\n  scope; every other endpoint requires the mapped bank:* scope (see x-scopes in\n  the OpenAPI). Descriptions and endpoint mappings are from the CDS authorisation\n  scopes reference.\nschemes:\n  - name: CDR-OAuth2\n    source: well-known/ing-australia-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://id.ob.ing.com.au/authorize\n        tokenUrl: https://secure.ob.ing.com.au/token\nscopes:\n  - scope:\
  \ openid\n    description: OpenID Connect authentication; issue an ID token for the customer.\n    flows: [authorizationCode]\n  - scope: profile\n    description: Basic OIDC profile claims (name, given_name, family_name).\n    flows: [authorizationCode]\n  - scope: bank:accounts.basic:read\n    description: Read basic account information and balances (list/detail without full account numbers).\n    operations: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n    flows: [authorizationCode]\n  - scope: bank:accounts.detail:read\n    description: Read detailed account information including account numbers and features.\n    operations: [getBankingAccountDetail]\n    flows: [authorizationCode]\n  - scope: bank:transactions:read\n    description: Read account transactions and transaction detail.\n    operations: [listBankingTransactions, getBankingTransactionDetail]\n    flows: [authorizationCode]\n  - scope: bank:payees:read\n    description:\
  \ Read the customer's saved/registered payees.\n    operations: [listBankingPayees, getBankingPayeeDetail]\n    flows: [authorizationCode]\n  - scope: bank:regular_payments:read\n    description: Read direct debits, scheduled payments and instalment plans.\n    operations: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts, listInstalmentPlans, listInstalmentPlansBulk]\n    flows: [authorizationCode]\n  - scope: common:customer.basic:read\n    description: Read basic customer information (name, occupation / organisation basics).\n    flows: [authorizationCode]\n  - scope: common:customer.detail:read\n    description: Read detailed customer information including contact details.\n    flows: [authorizationCode]\n  - scope: cdr:registration\n    description: Dynamic client registration management for the Accredited Data Recipient's software product.\n    flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/scopes/ing-australia-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
token_urls:
- https://secure.ob.ing.com.au/token
---
