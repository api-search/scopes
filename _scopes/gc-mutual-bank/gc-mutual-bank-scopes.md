---
api_specs:
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Product Reference Data API
  slug: gc-mutual-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Accounts & Balances API
  slug: gc-mutual-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Transactions API
  slug: gc-mutual-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Direct Debits & Scheduled Payments API
  slug: gc-mutual-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
- filename: gc-mutual-bank-cds-banking-products-openapi.yml
  format: yaml
  label: G&C Mutual Bank CDR Payees API
  slug: gc-mutual-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Gc Mutual Bank Scopes
name_suffix: OAuth Scopes
note: The public Product Reference Data surface requires NO scopes (unauthenticated). The scopes below are the DSB Consumer Data Standards CDR banking + common authorisation scopes that G&C Mutual Bank grants as a CDR Data Holder for the authenticated consumer-data surface. They are standard CDR scopes (not bank-proprietary) documented by the DSB; the harvested OpenAPI declares no oauth2 securitySchemes so these are captured from the standard, not derived.
overview: 'G&C Mutual Bank publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the G&C Mutual Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: G&C Mutual Bank
provider_slug: gc-mutual-bank
schemes:
- authorizationUrl: per Data Holder InfoSec (published via OIDC discovery)
  name: CDRConsumerDataAccess
  profile: FAPI 1.0 Advanced (OIDC hybrid)
  tokenUrl: per Data Holder InfoSec (published via OIDC discovery)
  type: oauth2
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
- description: OIDC authentication of the consumer.
  flows: []
  scope: openid
- description: Basic OIDC profile claims.
  flows: []
  scope: profile
- description: Read basic account information (account list, product category, balances).
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information (account terms, features, addresses).
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions.
  flows: []
  scope: bank:transactions:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
- description: Read direct debits and scheduled/recurring payments.
  flows: []
  scope: bank:regular_payments:read
- description: Read basic customer information (name, occupation / organisation type).
  flows: []
  scope: common:customer.basic:read
- description: Read detailed customer information (contact details, addresses).
  flows: []
  scope: common:customer.detail:read
slug: gc-mutual-bank-scopes
source_filename: gc-mutual-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  The public Product Reference Data surface requires NO scopes (unauthenticated).\n  The scopes below are the DSB Consumer Data Standards CDR banking + common\n  authorisation scopes that G&C Mutual Bank grants as a CDR Data Holder for the\n  authenticated consumer-data surface. They are standard CDR scopes (not\n  bank-proprietary) documented by the DSB; the harvested OpenAPI declares no\n  oauth2 securitySchemes so these are captured from the standard, not derived.\nschemes:\n  - name: CDRConsumerDataAccess\n    type: oauth2\n    profile: FAPI 1.0 Advanced (OIDC hybrid)\n    authorizationUrl: per Data Holder InfoSec (published via OIDC discovery)\n    tokenUrl: per Data Holder InfoSec (published via OIDC discovery)\nscopes:\n  - scope: openid\n\
  \    description: OIDC authentication of the consumer.\n  - scope: profile\n    description: Basic OIDC profile claims.\n  - scope: bank:accounts.basic:read\n    description: Read basic account information (account list, product category, balances).\n  - scope: bank:accounts.detail:read\n    description: Read detailed account information (account terms, features, addresses).\n  - scope: bank:transactions:read\n    description: Read account transactions.\n  - scope: bank:payees:read\n    description: Read saved payees.\n  - scope: bank:regular_payments:read\n    description: Read direct debits and scheduled/recurring payments.\n  - scope: common:customer.basic:read\n    description: Read basic customer information (name, occupation / organisation type).\n  - scope: common:customer.detail:read\n    description: Read detailed customer information (contact details, addresses).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/scopes/gc-mutual-bank-scopes.yml
summary_line: 9 scopes
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
