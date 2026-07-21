---
api_specs:
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Product Reference Data API
  slug: great-southern-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank Business+ CDR Product Reference Data API
  slug: great-southern-bank-business-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Accounts & Balances API
  slug: great-southern-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Transactions API
  slug: great-southern-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Direct Debits & Scheduled Payments API
  slug: great-southern-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Payees API
  slug: great-southern-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Great Southern Bank Scopes
name_suffix: OAuth Scopes
note: These OAuth2 scopes govern AUTHENTICATED CDR banking resource sharing and apply only to ACCC-accredited data recipients (ADRs). The public Product Reference Data endpoints (listBankingProducts / getBankingProductDetail) require NO scope. The full scopes_supported list below was confirmed live from the bank's CDR InfoSec OpenID discovery document (secure.open-banking.greatsouthernbank.com.au); the banking:* scopes are also annotated per-operation in the shared DSB CDS Banking spec. Scopes are standardised nationally by the Data Standards Body.
overview: 'Great Southern Bank publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Great Southern Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Great Southern Bank
provider_slug: great-southern-bank
schemes:
- authorization_endpoint: https://secure.open-banking.greatsouthernbank.com.au/as/authorization.oauth2
  code_challenge_methods_supported:
  - S256
  flows:
  - flow: authorizationCode
    note: CDR / FAPI 1.0 Advanced authorization code flow with PAR + PKCE.
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  issuer: https://auth.open-banking.greatsouthernbank.com.au
  name: CDR-OAuth2
  pushed_authorization_request_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/par.oauth2
  registration_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/clients.oauth2
  require_pushed_authorization_requests: true
  source: https://secure.open-banking.greatsouthernbank.com.au/.well-known/openid-configuration
  tls_client_certificate_bound_access_tokens: true
  token_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/token.oauth2
scope_count: 13
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
- common:customer.basic:read
- common:customer.detail:read
- cdr:registration
- admin:metrics.basic:read
- admin:metadata:update
- openid
- profile
- offline_access
scopes:
- description: Read basic account information (account list, product category, open/closed status).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account information including account numbers and features.
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read account transaction history.
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
- description: Read basic customer information (name, occupation / organisation basics).
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read detailed customer information including contact details and addresses.
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: CDR dynamic client registration scope for accredited data recipient software products.
  flows:
  - client_credentials
  scope: cdr:registration
- description: CDR admin scope for the DSB Get Metrics reporting endpoint (register/admin use).
  flows:
  - client_credentials
  scope: admin:metrics.basic:read
- description: CDR admin scope for the Metadata Update endpoint (register/admin use).
  flows:
  - client_credentials
  scope: admin:metadata:update
- description: OpenID Connect base scope.
  flows:
  - authorizationCode
  scope: openid
- description: OpenID Connect profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Request a refresh token for ongoing consented data sharing.
  flows:
  - authorizationCode
  scope: offline_access
slug: great-southern-bank-scopes
source_filename: great-southern-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://secure.open-banking.greatsouthernbank.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  These OAuth2 scopes govern AUTHENTICATED CDR banking resource sharing and apply\n  only to ACCC-accredited data recipients (ADRs). The public Product Reference\n  Data endpoints (listBankingProducts / getBankingProductDetail) require NO scope.\n  The full scopes_supported list below was confirmed live from the bank's CDR\n  InfoSec OpenID discovery document (secure.open-banking.greatsouthernbank.com.au);\n  the banking:* scopes are also annotated per-operation in the shared DSB CDS\n  Banking spec. Scopes are standardised nationally by the Data Standards Body.\nschemes:\n- name: CDR-OAuth2\n  source: https://secure.open-banking.greatsouthernbank.com.au/.well-known/openid-configuration\n  issuer: https://auth.open-banking.greatsouthernbank.com.au\n\
  \  authorization_endpoint: https://secure.open-banking.greatsouthernbank.com.au/as/authorization.oauth2\n  token_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/token.oauth2\n  pushed_authorization_request_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/par.oauth2\n  registration_endpoint: https://auth.open-banking.greatsouthernbank.com.au/as/clients.oauth2\n  grant_types_supported: [authorization_code, client_credentials, refresh_token]\n  code_challenge_methods_supported: [S256]\n  require_pushed_authorization_requests: true\n  tls_client_certificate_bound_access_tokens: true\n  flows:\n  - flow: authorizationCode\n    note: CDR / FAPI 1.0 Advanced authorization code flow with PAR + PKCE.\nscopes:\n- scope: bank:accounts.basic:read\n  description: Read basic account information (account list, product category, open/closed status).\n  flows: [authorizationCode]\n  sources: [openapi/great-southern-bank-cds-banking-products-openapi.yml]\n- scope: bank:accounts.detail:read\n\
  \  description: Read detailed account information including account numbers and features.\n  flows: [authorizationCode]\n  sources: [openapi/great-southern-bank-cds-banking-products-openapi.yml]\n- scope: bank:transactions:read\n  description: Read account transaction history.\n  flows: [authorizationCode]\n  sources: [openapi/great-southern-bank-cds-banking-products-openapi.yml]\n- scope: bank:payees:read\n  description: Read saved payees.\n  flows: [authorizationCode]\n  sources: [openapi/great-southern-bank-cds-banking-products-openapi.yml]\n- scope: bank:regular_payments:read\n  description: Read direct debits and scheduled/regular payments.\n  flows: [authorizationCode]\n  sources: [openapi/great-southern-bank-cds-banking-products-openapi.yml]\n- scope: common:customer.basic:read\n  description: Read basic customer information (name, occupation / organisation basics).\n  flows: [authorizationCode]\n  sources: [well-known/great-southern-bank-openid-configuration.json]\n- scope: common:customer.detail:read\n\
  \  description: Read detailed customer information including contact details and addresses.\n  flows: [authorizationCode]\n  sources: [well-known/great-southern-bank-openid-configuration.json]\n- scope: cdr:registration\n  description: CDR dynamic client registration scope for accredited data recipient software products.\n  flows: [client_credentials]\n  sources: [well-known/great-southern-bank-openid-configuration.json]\n- scope: admin:metrics.basic:read\n  description: CDR admin scope for the DSB Get Metrics reporting endpoint (register/admin use).\n  flows: [client_credentials]\n  sources: [well-known/great-southern-bank-openid-configuration.json]\n- scope: admin:metadata:update\n  description: CDR admin scope for the Metadata Update endpoint (register/admin use).\n  flows: [client_credentials]\n  sources: [well-known/great-southern-bank-openid-configuration.json]\n- scope: openid\n  description: OpenID Connect base scope.\n  flows: [authorizationCode]\n  sources: [well-known/great-southern-bank-openid-configuration.json]\n\
  - scope: profile\n  description: OpenID Connect profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/great-southern-bank-openid-configuration.json]\n- scope: offline_access\n  description: Request a refresh token for ongoing consented data sharing.\n  flows: [authorizationCode]\n  sources: [well-known/great-southern-bank-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/scopes/great-southern-bank-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Product Reference Data
token_urls: []
---
