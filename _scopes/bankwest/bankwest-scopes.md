---
api_specs:
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Product Reference Data API
  slug: bankwest-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Accounts & Balances API
  slug: bankwest-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Transactions API
  slug: bankwest-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Direct Debits & Scheduled Payments API
  slug: bankwest-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
- filename: bankwest-cds-banking-products-openapi.yml
  format: yaml
  label: Bankwest CDR Payees API
  slug: bankwest-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/openapi/bankwest-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bankwest Scopes
name_suffix: OAuth Scopes
note: The public Product Reference Data (Get Products / Get Product Detail) endpoints Bankwest exposes are unauthenticated and carry NO scope. The consumer-authorised CDR Banking endpoints — served over Bankwest's accredited MTLS channel and callable only by ACCC-accredited Data Recipients with customer consent — are gated by the standard CDR banking authorisation scopes. These scope strings are declared per-operation as x-scopes in the harvested CDS-AU banking spec and are defined by the DSB Consumer Data Standards, not by Bankwest. Authorisation uses OAuth 2.0 / OpenID Connect under the FAPI 2.0 security profile with Pushed Authorization Requests (PAR), as mandated by the Consumer Data Standards.
overview: 'Bankwest publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bankwest API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bankwest
provider_slug: bankwest
schemes:
- authorization_flow: authorizationCode + PAR (pushed authorization requests)
  name: cdrConsumerAuthorisation
  note: Bankwest publishes no self-onboarding path; access requires ACCC accreditation.
  profile: FAPI 2.0
  source: DSB Consumer Data Standards security profile
  type: openIdConnect
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Basic bank account data — list of accounts and their balances (masked account numbers, product category, nickname, balance amounts). Does not include full account identifiers.
  flows: []
  scope: bank:accounts.basic:read
- description: Detailed bank account data — full account detail including unmasked account number/BSB, features, fees, terms and address data for a single account.
  flows: []
  scope: bank:accounts.detail:read
- description: Transactions for authorised accounts — list and detail of account transactions with amount, date and description filtering.
  flows: []
  scope: bank:transactions:read
- description: Regular payments data — authorised direct debits, scheduled/recurring payments and instalment plans for the customer's accounts.
  flows: []
  scope: bank:regular_payments:read
- description: Saved payees — the customer's saved domestic, international and BPAY payees.
  flows: []
  scope: bank:payees:read
slug: bankwest-scopes
source_filename: bankwest-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/bankwest-cds-banking-products-openapi.yml (x-scopes) + DSB Consumer Data Standards security profile\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  The public Product Reference Data (Get Products / Get Product Detail) endpoints\n  Bankwest exposes are unauthenticated and carry NO scope. The consumer-authorised\n  CDR Banking endpoints — served over Bankwest's accredited MTLS channel and\n  callable only by ACCC-accredited Data Recipients with customer consent — are\n  gated by the standard CDR banking authorisation scopes. These scope strings are\n  declared per-operation as x-scopes in the harvested CDS-AU banking spec and are\n  defined by the DSB Consumer Data Standards, not by Bankwest. Authorisation uses\n  OAuth 2.0 / OpenID Connect under the FAPI 2.0 security profile with Pushed\n  Authorization Requests (PAR), as mandated by the Consumer Data Standards.\n\
  schemes:\n- name: cdrConsumerAuthorisation\n  type: openIdConnect\n  profile: FAPI 2.0\n  authorization_flow: authorizationCode + PAR (pushed authorization requests)\n  source: DSB Consumer Data Standards security profile\n  note: Bankwest publishes no self-onboarding path; access requires ACCC accreditation.\nscopes:\n- scope: bank:accounts.basic:read\n  description: >-\n    Basic bank account data — list of accounts and their balances (masked account\n    numbers, product category, nickname, balance amounts). Does not include full\n    account identifiers.\n  operations:\n  - listBankingAccounts\n  - listBankingBalancesBulk\n  - listBankingBalancesSpecificAccounts\n  - getBankingBalance\n  sources: [openapi/bankwest-cds-banking-products-openapi.yml]\n- scope: bank:accounts.detail:read\n  description: >-\n    Detailed bank account data — full account detail including unmasked account\n    number/BSB, features, fees, terms and address data for a single account.\n  operations:\n  - getBankingAccountDetail\n\
  \  sources: [openapi/bankwest-cds-banking-products-openapi.yml]\n- scope: bank:transactions:read\n  description: >-\n    Transactions for authorised accounts — list and detail of account transactions\n    with amount, date and description filtering.\n  operations:\n  - listBankingTransactions\n  - getBankingTransactionDetail\n  sources: [openapi/bankwest-cds-banking-products-openapi.yml]\n- scope: bank:regular_payments:read\n  description: >-\n    Regular payments data — authorised direct debits, scheduled/recurring payments\n    and instalment plans for the customer's accounts.\n  operations:\n  - listDirectDebits\n  - listDirectDebitsBulk\n  - listDirectDebitsSpecificAccounts\n  - listScheduledPayments\n  - listScheduledPaymentsBulk\n  - listScheduledPaymentsSpecificAccounts\n  - listInstalmentPlans\n  - listInstalmentPlansBulk\n  sources: [openapi/bankwest-cds-banking-products-openapi.yml]\n- scope: bank:payees:read\n  description: >-\n    Saved payees — the customer's saved domestic,\
  \ international and BPAY payees.\n  operations:\n  - listBankingPayees\n  - getBankingPayeeDetail\n  sources: [openapi/bankwest-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankwest/refs/heads/main/scopes/bankwest-scopes.yml
summary_line: 5 scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Digital Bank
token_urls: []
---
