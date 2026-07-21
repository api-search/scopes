---
api_specs:
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Product Reference Data API
  slug: alex-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Accounts & Balances API
  slug: alex-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Transactions API
  slug: alex-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Direct Debits & Scheduled Payments API
  slug: alex-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
- filename: alex-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Alex Bank CDR Payees API
  slug: alex-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/openapi/alex-bank-cds-banking-products-openapi.yml
authorization_urls:
- https://public.cdr.alex.com.au/connect/authorize
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#cdr-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Alex Bank Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by Alex Bank's CDR OpenID Provider (scopes_supported). These gate the ACCC-accredited-data-recipient (ADR) consumer-data-sharing surface; the public Product Reference Data endpoints require NO scope. Scope semantics are defined by the DSB Consumer Data Standards, not by Alex Bank.
overview: 'Alex Bank publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alex Bank API on a user''s behalf.


  Tokens are issued from https://secure.cdr.alex.com.au/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alex Bank
provider_slug: alex-bank
schemes:
- flows:
  - authorizationUrl: https://public.cdr.alex.com.au/connect/authorize
    flow: authorizationCode
    tokenUrl: https://secure.cdr.alex.com.au/connect/token
  name: CDR-OAuth2-OIDC
  source: https://public.cdr.alex.com.au/.well-known/openid-configuration
scope_count: 12
scope_names:
- openid
- profile
- common:customer.basic:read
- common:customer.detail:read
- cdr:registration
- admin:metrics.basic:read
- admin:metadata:update
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Basic end-user profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Read basic customer/organisation contact and identity details.
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read detailed customer/organisation identity and contact details.
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: Dynamic client registration for accredited data recipients (CDR register).
  flows:
  - clientCredentials
  scope: cdr:registration
- description: Read Get Metrics administrative endpoint (CDR reporting).
  flows:
  - clientCredentials
  scope: admin:metrics.basic:read
- description: Trigger a metadata refresh from the CDR Register (admin).
  flows:
  - clientCredentials
  scope: admin:metadata:update
- description: Read basic banking account data (account list, product category, nickname).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed banking account data (features, fees, address, holder detail).
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
slug: alex-bank-scopes
source_filename: alex-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://public.cdr.alex.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#cdr-scopes\nnote: >-\n  Scopes advertised by Alex Bank's CDR OpenID Provider (scopes_supported). These gate\n  the ACCC-accredited-data-recipient (ADR) consumer-data-sharing surface; the public\n  Product Reference Data endpoints require NO scope. Scope semantics are defined by the\n  DSB Consumer Data Standards, not by Alex Bank.\nschemes:\n- name: CDR-OAuth2-OIDC\n  source: https://public.cdr.alex.com.au/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://public.cdr.alex.com.au/connect/authorize\n    tokenUrl: https://secure.cdr.alex.com.au/connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  flows: [authorizationCode]\n- scope: profile\n  description: Basic end-user profile claims.\n  flows:\
  \ [authorizationCode]\n- scope: common:customer.basic:read\n  description: Read basic customer/organisation contact and identity details.\n  flows: [authorizationCode]\n- scope: common:customer.detail:read\n  description: Read detailed customer/organisation identity and contact details.\n  flows: [authorizationCode]\n- scope: cdr:registration\n  description: Dynamic client registration for accredited data recipients (CDR register).\n  flows: [clientCredentials]\n- scope: admin:metrics.basic:read\n  description: Read Get Metrics administrative endpoint (CDR reporting).\n  flows: [clientCredentials]\n- scope: admin:metadata:update\n  description: Trigger a metadata refresh from the CDR Register (admin).\n  flows: [clientCredentials]\n- scope: bank:accounts.basic:read\n  description: Read basic banking account data (account list, product category, nickname).\n  flows: [authorizationCode]\n- scope: bank:accounts.detail:read\n  description: Read detailed banking account data (features, fees,\
  \ address, holder detail).\n  flows: [authorizationCode]\n- scope: bank:transactions:read\n  description: Read banking account transactions.\n  flows: [authorizationCode]\n- scope: bank:payees:read\n  description: Read saved payees.\n  flows: [authorizationCode]\n- scope: bank:regular_payments:read\n  description: Read direct debits and scheduled/regular payments.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alex-bank/refs/heads/main/scopes/alex-bank-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Digital Bank
- Product Reference Data
token_urls:
- https://secure.cdr.alex.com.au/connect/token
---
