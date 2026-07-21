---
api_specs:
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Product Reference Data API
  slug: banksa-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Accounts & Balances API
  slug: banksa-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Transactions API
  slug: banksa-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Direct Debits & Scheduled Payments API
  slug: banksa-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
- filename: banksa-cds-banking-products-openapi.yml
  format: yaml
  label: BankSA CDR Payees API
  slug: banksa-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/openapi/banksa-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Banksa Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BankSA publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BankSA API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BankSA
provider_slug: banksa
schemes:
- flows:
  - flow: authorizationCode
    note: Authorization/token endpoints are per-data-holder and discovered by accredited data recipients through the CDR Register, not published on a public BankSA host.
  name: CDRConsumerDataSharing
  profile: FAPI 1.0 Advanced (CDR Security Profile)
  source: openapi/banksa-cds-banking-products-openapi.yml
scope_count: 9
scope_names:
- openid
- profile
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
- common:customer.basic:read
- common:customer.detail:read
scopes:
- description: OpenID Connect authentication of the consumer.
  flows:
  - authorizationCode
  scope: openid
- description: Basic OpenID Connect profile claims for the consenting consumer.
  flows:
  - authorizationCode
  scope: profile
- description: Read the consumer's account list and basic account attributes.
  flows: []
  scope: bank:accounts.basic:read
- description: Read full detail for a specific account (features, rates, terms).
  flows: []
  scope: bank:accounts.detail:read
- description: Read transactions for the consumer's accounts.
  flows: []
  scope: bank:transactions:read
- description: Read direct debits, scheduled payments and instalment plans on the consumer's accounts.
  flows: []
  scope: bank:regular_payments:read
- description: Read the consumer's saved payees.
  flows: []
  scope: bank:payees:read
- description: Read the consumer's basic customer/contact information.
  flows: []
  scope: common:customer.basic:read
- description: Read the consumer's detailed customer information.
  flows: []
  scope: common:customer.detail:read
slug: banksa-scopes
source_filename: banksa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\n  — the Consumer Data Right banking authorisation scopes. The harvested spec\n  declares no oauth2 securitySchemes (auth is defined by the separate CDR\n  Security Profile), so scopes are captured from the DSB Consumer Data Standards\n  that BankSA's data-holder host conforms to. The public Product Reference Data\n  endpoints require NO scope; every other endpoint in the spec requires the CDR\n  scope mapped below, granted only through a consumer's consent to an accredited\n  data recipient.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nschemes:\n- name: CDRConsumerDataSharing\n  source: openapi/banksa-cds-banking-products-openapi.yml\n  profile: FAPI 1.0 Advanced (CDR Security Profile)\n  flows:\n  - flow: authorizationCode\n    note: >-\n      Authorization/token endpoints are per-data-holder\
  \ and discovered by\n      accredited data recipients through the CDR Register, not published on a\n      public BankSA host.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication of the consumer.\n  flows: [authorizationCode]\n- scope: profile\n  description: Basic OpenID Connect profile claims for the consenting consumer.\n  flows: [authorizationCode]\n- scope: bank:accounts.basic:read\n  description: Read the consumer's account list and basic account attributes.\n  endpoints:\n  - GET /banking/accounts\n  - GET /banking/accounts/balances\n  - GET /banking/accounts/{accountId}/balance\n- scope: bank:accounts.detail:read\n  description: Read full detail for a specific account (features, rates, terms).\n  endpoints:\n  - GET /banking/accounts/{accountId}\n- scope: bank:transactions:read\n  description: Read transactions for the consumer's accounts.\n  endpoints:\n  - GET /banking/accounts/{accountId}/transactions\n  - GET /banking/accounts/{accountId}/transactions/{transactionId}\n\
  - scope: bank:regular_payments:read\n  description: >-\n    Read direct debits, scheduled payments and instalment plans on the\n    consumer's accounts.\n  endpoints:\n  - GET /banking/accounts/{accountId}/direct-debits\n  - GET /banking/accounts/{accountId}/payments/scheduled\n  - GET /banking/accounts/{accountId}/payments/plans\n- scope: bank:payees:read\n  description: Read the consumer's saved payees.\n  endpoints:\n  - GET /banking/payees\n  - GET /banking/payees/{payeeId}\n- scope: common:customer.basic:read\n  description: Read the consumer's basic customer/contact information.\n- scope: common:customer.detail:read\n  description: Read the consumer's detailed customer information.\npublic_endpoints_no_scope:\n- GET /banking/products\n- GET /banking/products/{productId}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banksa/refs/heads/main/scopes/banksa-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
token_urls: []
---
