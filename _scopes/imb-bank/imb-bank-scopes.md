---
api_specs:
- filename: imb-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Account Balances API
  slug: imb-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-account-balances-api-openapi.yml
- filename: imb-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Account Direct Debits API
  slug: imb-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-account-direct-debits-api-openapi.yml
- filename: imb-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Account Scheduled Payments API
  slug: imb-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: imb-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Account Transactions API
  slug: imb-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-account-transactions-api-openapi.yml
- filename: imb-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Accounts API
  slug: imb-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-accounts-api-openapi.yml
- filename: imb-bank-banking-payees-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Payees API
  slug: imb-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-payees-api-openapi.yml
- filename: imb-bank-banking-products-api-openapi.yml
  format: yaml
  label: IMB Bank Banking Products API
  slug: imb-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/openapi/imb-bank-banking-products-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#end-points
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Imb Bank Scopes
name_suffix: OAuth Scopes
note: Scopes captured verbatim from IMB's live OIDC discovery document (scopes_supported). Descriptions follow the Australian Consumer Data Standards (CDS) authorisation scopes for the banking sector. Access to member banking data requires the CDR consent flow (PAR + private_key_jwt + mTLS); the public Product Reference Data API is unauthenticated and requires no scope.
overview: 'IMB Bank publishes 12 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the IMB Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IMB Bank
provider_slug: imb-bank
schemes:
- acr_values:
  - urn:cds.au:cdr:2
  authorization_endpoint: https://auth.openbanking.imb.com.au/oauth2/authorize
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  issuer: https://openbank.openbanking.imb.com.au
  name: OpenIDConnect
  pushed_authorization_request_endpoint: https://openbank-secure.openbanking.imb.com.au/api/openbanking/push-authorization/par
  registration_endpoint: https://openbank-secure.openbanking.imb.com.au/open-banking/0.2/register
  source: well-known/imb-bank-openid-configuration.json
  token_endpoint: https://openbank-secure.openbanking.imb.com.au/oauth2/token
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
- description: OpenID Connect authentication; issue an ID token for the CDR consumer.
  flows:
  - authorizationCode
  scope: openid
- description: End-user profile claims (name, given_name, family_name).
  flows:
  - authorizationCode
  scope: profile
- description: Read the basic customer record (name and occupation / organisation type).
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read customer contact details (address, phone, email).
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: Read basic account data (account name, type, balance, product category).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account data (account numbers, features, fees, rates).
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read account transactions (amounts, descriptions, timestamps).
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read the customer's saved payees.
  flows:
  - authorizationCode
  scope: bank:payees:read
- description: Read direct debits and scheduled/regular payments.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
- description: Data-holder admin scope for the CDR Get Metrics reporting endpoint.
  flows:
  - clientCredentials
  scope: admin:metrics.basic:read
- description: Data-holder admin scope for CDR Register metadata update notifications.
  flows:
  - clientCredentials
  scope: admin:metadata:update
- description: Dynamic Client Registration (DCR) scope for accredited data recipients.
  flows:
  - clientCredentials
  scope: cdr:registration
slug: imb-bank-scopes
source_filename: imb-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://openbank.openbanking.imb.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#end-points\nnote: Scopes captured verbatim from IMB's live OIDC discovery document (scopes_supported).\n  Descriptions follow the Australian Consumer Data Standards (CDS) authorisation scopes\n  for the banking sector. Access to member banking data requires the CDR consent flow\n  (PAR + private_key_jwt + mTLS); the public Product Reference Data API is unauthenticated\n  and requires no scope.\nschemes:\n- name: OpenIDConnect\n  source: well-known/imb-bank-openid-configuration.json\n  issuer: https://openbank.openbanking.imb.com.au\n  authorization_endpoint: https://auth.openbanking.imb.com.au/oauth2/authorize\n  token_endpoint: https://openbank-secure.openbanking.imb.com.au/oauth2/token\n  pushed_authorization_request_endpoint: https://openbank-secure.openbanking.imb.com.au/api/openbanking/push-authorization/par\n\
  \  registration_endpoint: https://openbank-secure.openbanking.imb.com.au/open-banking/0.2/register\n  grant_types: [authorization_code, client_credentials, refresh_token]\n  acr_values: [urn:cds.au:cdr:2]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the CDR consumer.\n  flows: [authorizationCode]\n- scope: profile\n  description: End-user profile claims (name, given_name, family_name).\n  flows: [authorizationCode]\n- scope: common:customer.basic:read\n  description: Read the basic customer record (name and occupation / organisation type).\n  flows: [authorizationCode]\n- scope: common:customer.detail:read\n  description: Read customer contact details (address, phone, email).\n  flows: [authorizationCode]\n- scope: bank:accounts.basic:read\n  description: Read basic account data (account name, type, balance, product category).\n  flows: [authorizationCode]\n- scope: bank:accounts.detail:read\n  description: Read detailed account data (account\
  \ numbers, features, fees, rates).\n  flows: [authorizationCode]\n- scope: bank:transactions:read\n  description: Read account transactions (amounts, descriptions, timestamps).\n  flows: [authorizationCode]\n- scope: bank:payees:read\n  description: Read the customer's saved payees.\n  flows: [authorizationCode]\n- scope: bank:regular_payments:read\n  description: Read direct debits and scheduled/regular payments.\n  flows: [authorizationCode]\n- scope: admin:metrics.basic:read\n  description: Data-holder admin scope for the CDR Get Metrics reporting endpoint.\n  flows: [clientCredentials]\n- scope: admin:metadata:update\n  description: Data-holder admin scope for CDR Register metadata update notifications.\n  flows: [clientCredentials]\n- scope: cdr:registration\n  description: Dynamic Client Registration (DCR) scope for accredited data recipients.\n  flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imb-bank/refs/heads/main/scopes/imb-bank-scopes.yml
summary_line: 12 scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
token_urls: []
---
