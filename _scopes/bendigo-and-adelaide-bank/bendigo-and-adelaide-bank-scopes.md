---
api_specs:
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Product Reference Data API
  slug: bendigo-and-adelaide-bank-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Accounts & Balances API
  slug: bendigo-and-adelaide-bank-cds-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Transactions API
  slug: bendigo-and-adelaide-bank-cds-banking-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Direct Debits & Scheduled Payments API
  slug: bendigo-and-adelaide-bank-cds-banking-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Payees API
  slug: bendigo-and-adelaide-bank-cds-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-up-developer-api-openapi.json
  format: json
  label: Up Developer API (Personal Banking)
  slug: up-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-up-developer-api-openapi.json
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up Banking CDR Product Reference Data API
  slug: up-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Adelaide Bank CDR Product Reference Data API
  slug: adelaide-bank-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
authorization_urls:
- https://api.up.com.au/oidc/authorize
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#end-points
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Bendigo And Adelaide Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bendigo and Adelaide Bank publishes 10 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bendigo and Adelaide Bank API on a user''s behalf.


  Tokens are issued from https://secure.api.up.com.au/oidc/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bendigo and Adelaide Bank
provider_slug: bendigo-and-adelaide-bank
schemes:
- flows:
  - authorizationUrl: https://api.up.com.au/oidc/authorize
    flow: authorizationCode
    pushed_authorization_request_endpoint: https://secure.api.up.com.au/oidc/authorize/push
    require_pushed_authorization_requests: true
    tokenUrl: https://secure.api.up.com.au/oidc/token
  - flow: clientCredentials
    tokenUrl: https://secure.api.up.com.au/oidc/token
  issuer: https://api.up.com.au
  name: OpenIDConnect
  source: well-known/bendigo-and-adelaide-bank-up-openid-configuration.json
  type: openIdConnect
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
- description: OIDC authentication; issue an ID token identifying the consumer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the consumer's basic OIDC profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Read basic banking account data (account list and basic attributes).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed banking account data (balances, account detail).
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
- description: Read basic customer data (name, type).
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read detailed customer data (contact details).
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: Dynamic client registration for accredited CDR data recipient software products.
  flows:
  - clientCredentials
  scope: cdr:registration
slug: bendigo-and-adelaide-bank-scopes
source_filename: bendigo-and-adelaide-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.up.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#end-points\nnotes: >-\n  Scopes captured verbatim from the live CDR OIDC discovery document of the Up brand\n  (owned by Bendigo and Adelaide Bank). These are the standardised Australian Consumer\n  Data Right (CDR) banking + common data-cluster scopes governed by the Consumer Data\n  Standards. They apply to the AUTHENTICATED CDR data-sharing surface (accredited data\n  recipients only, via FAPI 1.0 Advanced / MTLS). The public Product Reference Data API\n  (GET /banking/products) is unauthenticated and requires no scope.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  source: well-known/bendigo-and-adelaide-bank-up-openid-configuration.json\n  issuer: https://api.up.com.au\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.up.com.au/oidc/authorize\n    tokenUrl: https://secure.api.up.com.au/oidc/token\n\
  \    pushed_authorization_request_endpoint: https://secure.api.up.com.au/oidc/authorize/push\n    require_pushed_authorization_requests: true\n  - flow: clientCredentials\n    tokenUrl: https://secure.api.up.com.au/oidc/token\nscopes:\n- scope: openid\n  description: OIDC authentication; issue an ID token identifying the consumer.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the consumer's basic OIDC profile claims.\n  flows: [authorizationCode]\n- scope: bank:accounts.basic:read\n  description: Read basic banking account data (account list and basic attributes).\n  flows: [authorizationCode]\n- scope: bank:accounts.detail:read\n  description: Read detailed banking account data (balances, account detail).\n  flows: [authorizationCode]\n- scope: bank:transactions:read\n  description: Read banking account transactions.\n  flows: [authorizationCode]\n- scope: bank:payees:read\n  description: Read saved payees.\n  flows: [authorizationCode]\n- scope: bank:regular_payments:read\n\
  \  description: Read direct debits and scheduled/regular payments.\n  flows: [authorizationCode]\n- scope: common:customer.basic:read\n  description: Read basic customer data (name, type).\n  flows: [authorizationCode]\n- scope: common:customer.detail:read\n  description: Read detailed customer data (contact details).\n  flows: [authorizationCode]\n- scope: cdr:registration\n  description: Dynamic client registration for accredited CDR data recipient software products.\n  flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/scopes/bendigo-and-adelaide-bank-scopes.yml
summary_line: 10 scopes · authorizationCode/clientCredentials
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
token_urls:
- https://secure.api.up.com.au/oidc/token
---
