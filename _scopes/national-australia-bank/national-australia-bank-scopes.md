---
api_specs:
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Product Reference Data API
  slug: national-australia-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Accounts & Balances API
  slug: national-australia-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Transactions API
  slug: national-australia-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Direct Debits & Scheduled Payments API
  slug: national-australia-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
- filename: national-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: National Australia Bank (NAB) CDR Payees API
  slug: national-australia-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/openapi/national-australia-bank-cds-banking-products-openapi.yml
authorization_urls:
- https://openbank.api.nab.com.au/v1/idp/cdr/nab/authorise
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: National Australia Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'National Australia Bank publishes 11 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the National Australia Bank API on a user''s behalf.


  Tokens are issued from https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: National Australia Bank
provider_slug: national-australia-bank
schemes:
- flows:
  - authorizationUrl: https://openbank.api.nab.com.au/v1/idp/cdr/nab/authorise
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pushed_authorization_request_endpoint: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/par
    require_pushed_authorization_requests: true
    require_signed_request_object: true
    tokenUrl: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/token
  - flow: clientCredentials
    tokenUrl: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/token
  - flow: refreshToken
    tokenUrl: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/token
  issuer: https://openbank.api.nab.com.au
  name: CDR OAuth2 / OIDC
  source: https://openbank.api.nab.com.au/.well-known/openid-configuration
scope_count: 11
scope_names:
- openid
- profile
- offline_access
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
- common:customer.basic:read
- common:customer.detail:read
- cdr:registration
scopes:
- description: OpenID Connect authentication (id_token issuance).
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token for ongoing data sharing within the arrangement.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read basic account data (account list and basic details).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account data.
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read account transactions.
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
- description: Read basic customer data.
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read detailed customer data.
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: Dynamic Client Registration under the CDR Register.
  flows:
  - clientCredentials
  scope: cdr:registration
slug: national-australia-bank-scopes
source_filename: national-australia-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://openbank.api.nab.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\n# CDR authorisation scopes advertised by NAB's live OIDC discovery document.\n# These govern the accredited consumer-data-sharing surface; the public Product\n# Reference Data endpoints require no scope. acr: urn:cds.au:cdr:2.\nschemes:\n  - name: CDR OAuth2 / OIDC\n    source: https://openbank.api.nab.com.au/.well-known/openid-configuration\n    issuer: https://openbank.api.nab.com.au\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://openbank.api.nab.com.au/v1/idp/cdr/nab/authorise\n        tokenUrl: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/token\n        pushed_authorization_request_endpoint: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/par\n        require_pushed_authorization_requests: true\n        require_signed_request_object:\
  \ true\n        code_challenge_methods: [S256]\n      - flow: clientCredentials\n        tokenUrl: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/token\n      - flow: refreshToken\n        tokenUrl: https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (id_token issuance).\n    flows: [authorizationCode]\n  - scope: profile\n    description: Basic profile claims.\n    flows: [authorizationCode]\n  - scope: offline_access\n    description: Issue a refresh token for ongoing data sharing within the arrangement.\n    flows: [authorizationCode]\n  - scope: bank:accounts.basic:read\n    description: Read basic account data (account list and basic details).\n    flows: [authorizationCode]\n  - scope: bank:accounts.detail:read\n    description: Read detailed account data.\n    flows: [authorizationCode]\n  - scope: bank:transactions:read\n    description: Read account transactions.\n    flows: [authorizationCode]\n\
  \  - scope: bank:payees:read\n    description: Read saved payees.\n    flows: [authorizationCode]\n  - scope: bank:regular_payments:read\n    description: Read direct debits and scheduled/regular payments.\n    flows: [authorizationCode]\n  - scope: common:customer.basic:read\n    description: Read basic customer data.\n    flows: [authorizationCode]\n  - scope: common:customer.detail:read\n    description: Read detailed customer data.\n    flows: [authorizationCode]\n  - scope: cdr:registration\n    description: Dynamic Client Registration under the CDR Register.\n    flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-australia-bank/refs/heads/main/scopes/national-australia-bank-scopes.yml
summary_line: 11 scopes · authorizationCode/clientCredentials/refreshToken
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
- https://openbank-secure.api.nab.com.au/v1/idp/cdr/nab/token
---
