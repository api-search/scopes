---
api_specs:
- filename: suncorp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Suncorp Bank CDR Product Reference Data API
  slug: suncorp-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-cds-banking-products-openapi.yml
- filename: suncorp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Suncorp Bank CDR Accounts & Balances API
  slug: suncorp-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-cds-banking-products-openapi.yml
- filename: suncorp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Suncorp Bank CDR Transactions API
  slug: suncorp-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-cds-banking-products-openapi.yml
- filename: suncorp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Suncorp Bank CDR Direct Debits & Scheduled Payments API
  slug: suncorp-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-cds-banking-products-openapi.yml
- filename: suncorp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Suncorp Bank CDR Payees API
  slug: suncorp-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/openapi/suncorp-bank-cds-banking-products-openapi.yml
authorization_urls:
- https://id-ob.suncorpbank.com.au/authorize
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#security-endpoints
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Suncorp Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Suncorp Bank publishes 10 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Suncorp Bank API on a user''s behalf.


  Tokens are issued from https://secure-id-ob.suncorpbank.com.au/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Suncorp Bank
provider_slug: suncorp-bank
schemes:
- flows:
  - authorizationUrl: https://id-ob.suncorpbank.com.au/authorize
    flow: authorizationCode
    tokenUrl: https://secure-id-ob.suncorpbank.com.au/token
  - flow: clientCredentials
    tokenUrl: https://secure-id-ob.suncorpbank.com.au/token
  name: CDR OpenID Connect
  source: well-known/suncorp-bank-openid-configuration.json
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
- description: OpenID Connect authentication; issue an ID token for the consumer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to basic profile claims (name, given_name, family_name).
  flows:
  - authorizationCode
  scope: profile
- description: Read basic banking account data (account list, masked identifiers, balances metadata).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed banking account data (account numbers, features, terms).
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read banking account transactions.
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read saved payees.
  flows:
  - authorizationCode
  scope: bank:payees:read
- description: Read direct debits and scheduled/regular payments.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
- description: Read basic customer data (name, contact type).
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read detailed customer data (contact details, organisation details).
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: Dynamic client registration for CDR Accredited Data Recipients.
  flows:
  - clientCredentials
  scope: cdr:registration
slug: suncorp-bank-scopes
source_filename: suncorp-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://id-ob.suncorpbank.com.au/.well-known/openid-configuration\n  (scopes_supported, live OIDC discovery, fetched 2026-07-20)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-endpoints\nnotes: >-\n  Scopes govern the CDR-accredited (authenticated) consumer-data-sharing tier.\n  The public Product Reference Data API is unauthenticated and requires no scope.\n  Scope semantics are defined by the Australian Consumer Data Standards (CDS).\nschemes:\n- name: CDR OpenID Connect\n  source: well-known/suncorp-bank-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id-ob.suncorpbank.com.au/authorize\n    tokenUrl: https://secure-id-ob.suncorpbank.com.au/token\n  - flow: clientCredentials\n    tokenUrl: https://secure-id-ob.suncorpbank.com.au/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the consumer.\n\
  \  flows: [authorizationCode]\n- scope: profile\n  description: Access to basic profile claims (name, given_name, family_name).\n  flows: [authorizationCode]\n- scope: bank:accounts.basic:read\n  description: Read basic banking account data (account list, masked identifiers, balances metadata).\n  flows: [authorizationCode]\n- scope: bank:accounts.detail:read\n  description: Read detailed banking account data (account numbers, features, terms).\n  flows: [authorizationCode]\n- scope: bank:transactions:read\n  description: Read banking account transactions.\n  flows: [authorizationCode]\n- scope: bank:payees:read\n  description: Read saved payees.\n  flows: [authorizationCode]\n- scope: bank:regular_payments:read\n  description: Read direct debits and scheduled/regular payments.\n  flows: [authorizationCode]\n- scope: common:customer.basic:read\n  description: Read basic customer data (name, contact type).\n  flows: [authorizationCode]\n- scope: common:customer.detail:read\n  description:\
  \ Read detailed customer data (contact details, organisation details).\n  flows: [authorizationCode]\n- scope: cdr:registration\n  description: Dynamic client registration for CDR Accredited Data Recipients.\n  flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suncorp-bank/refs/heads/main/scopes/suncorp-bank-scopes.yml
summary_line: 10 scopes · authorizationCode/clientCredentials
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- Consumer Data Right
token_urls:
- https://secure-id-ob.suncorpbank.com.au/token
---
