---
api_specs:
- filename: newcastle-permanent-products-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Product Reference Data API
  slug: newcastle-permanent-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-products-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Accounts & Balances API
  slug: newcastle-permanent-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Transactions API
  slug: newcastle-permanent-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Direct Debits & Scheduled Payments API
  slug: newcastle-permanent-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Payees API
  slug: newcastle-permanent-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Common Customer API
  slug: newcastle-permanent-cdr-common-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
authorization_urls:
- https://openbank.newcastlepermanent.com.au/oauth2/authorize
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Newcastle Permanent Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Newcastle Permanent Building Society publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Newcastle Permanent Building Society API on a user''s behalf.


  Tokens are issued from https://openbank-secure.newcastlepermanent.com.au/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Newcastle Permanent Building Society
provider_slug: newcastle-permanent
schemes:
- flows:
  - authorizationUrl: https://openbank.newcastlepermanent.com.au/oauth2/authorize
    flow: authorizationCode
    jwksUri: https://openbank.newcastlepermanent.com.au/oauth2/jwks
    parEndpoint: https://openbank-secure.newcastlepermanent.com.au/api/openbanking/push-authorization/par
    registrationEndpoint: https://openbank-secure.newcastlepermanent.com.au/open-banking/0.2/register
    tokenEndpointAuthMethods:
    - private_key_jwt
    tokenUrl: https://openbank-secure.newcastlepermanent.com.au/oauth2/token
  issuer: https://openbank.newcastlepermanent.com.au
  name: cdr-oidc
  sources:
  - https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration
  type: openIdConnect
scope_count: 12
scope_names:
- openid
- profile
- common:customer.basic:read
- common:customer.detail:read
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
- admin:metrics.basic:read
- admin:metadata:update
- cdr:registration
scopes:
- description: OpenID Connect authentication
  flows: []
  scope: openid
- description: End-user profile claims
  flows: []
  scope: profile
- description: Read basic customer information (name
  flows: []
  scope: common:customer.basic:read
- description: Read detailed customer information (contact details)
  flows: []
  scope: common:customer.detail:read
- description: Read basic banking account information
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed banking account information
  flows: []
  scope: bank:accounts.detail:read
- description: Read banking account transactions
  flows: []
  scope: bank:transactions:read
- description: Read saved payees
  flows: []
  scope: bank:payees:read
- description: Read direct debits and scheduled/regular payments
  flows: []
  scope: bank:regular_payments:read
- description: CDR admin metrics (Get Metrics) for the data holder
  flows: []
  scope: admin:metrics.basic:read
- description: CDR admin metadata update (register metadata refresh)
  flows: []
  scope: admin:metadata:update
- description: Dynamic client registration for CDR software products
  flows: []
  scope: cdr:registration
slug: newcastle-permanent-scopes
source_filename: newcastle-permanent-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnotes: >-\n  OAuth2 / OpenID Connect scopes advertised by Newcastle Permanent's live CDR\n  authorization server, harvested verbatim from its OpenID Connect discovery\n  document (scopes_supported). These are the standardised CDR banking + common\n  scopes; they gate the accredited-data-recipient (ADR) consumer-data-sharing\n  surface, NOT the public Product Reference Data endpoints (which are\n  unauthenticated). token_endpoint_auth_methods_supported = private_key_jwt and a\n  pushed_authorization_request_endpoint are present, consistent with the FAPI\n  security profile the CDS mandates.\nschemes:\n  - name: cdr-oidc\n    type: openIdConnect\n    issuer: https://openbank.newcastlepermanent.com.au\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://openbank.newcastlepermanent.com.au/oauth2/authorize\n        tokenUrl: https://openbank-secure.newcastlepermanent.com.au/oauth2/token\n        parEndpoint: https://openbank-secure.newcastlepermanent.com.au/api/openbanking/push-authorization/par\n        registrationEndpoint: https://openbank-secure.newcastlepermanent.com.au/open-banking/0.2/register\n        jwksUri: https://openbank.newcastlepermanent.com.au/oauth2/jwks\n        tokenEndpointAuthMethods: [private_key_jwt]\n    sources: [https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration]\nscopes:\n  - {scope: openid, description: OpenID Connect authentication}\n  - {scope: profile, description: End-user profile claims}\n  - {scope: 'common:customer.basic:read', description: Read basic customer information (name, occupation)}\n  - {scope: 'common:customer.detail:read', description: Read detailed customer information (contact details)}\n  - {scope: 'bank:accounts.basic:read', description: Read basic banking\
  \ account information}\n  - {scope: 'bank:accounts.detail:read', description: Read detailed banking account information}\n  - {scope: 'bank:transactions:read', description: Read banking account transactions}\n  - {scope: 'bank:payees:read', description: Read saved payees}\n  - {scope: 'bank:regular_payments:read', description: Read direct debits and scheduled/regular payments}\n  - {scope: 'admin:metrics.basic:read', description: CDR admin metrics (Get Metrics) for the data holder}\n  - {scope: 'admin:metadata:update', description: CDR admin metadata update (register metadata refresh)}\n  - {scope: 'cdr:registration', description: Dynamic client registration for CDR software products}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/scopes/newcastle-permanent-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Building Society
- Mutual
- Australia
token_urls:
- https://openbank-secure.newcastlepermanent.com.au/oauth2/token
---
