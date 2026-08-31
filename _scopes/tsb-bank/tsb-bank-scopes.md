---
api_specs:
- filename: tsb-bank-atm-api-openapi.yml
  format: yaml
  label: TSB Bank ATM API
  slug: tsb-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-atm-api-openapi.yml
- filename: tsb-bank-authorization-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Authorization Server APIs API
  slug: tsb-bank-authorization-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-authorization-server-apis-api-openapi.yml
- filename: tsb-bank-bca-api-openapi.yml
  format: yaml
  label: TSB Bank BCA API
  slug: tsb-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-bca-api-openapi.yml
- filename: tsb-bank-branch-api-openapi.yml
  format: yaml
  label: TSB Bank Branch API
  slug: tsb-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-branch-api-openapi.yml
- filename: tsb-bank-ccc-api-openapi.yml
  format: yaml
  label: TSB Bank CCC API
  slug: tsb-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-ccc-api-openapi.yml
- filename: tsb-bank-pca-api-openapi.yml
  format: yaml
  label: TSB Bank PCA API
  slug: tsb-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-pca-api-openapi.yml
- filename: tsb-bank-resource-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Resource Server APIs API
  slug: tsb-bank-resource-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-resource-server-apis-api-openapi.yml
- filename: tsb-bank-sme-api-openapi.yml
  format: yaml
  label: TSB Bank SME API
  slug: tsb-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-sme-api-openapi.yml
- filename: tsb-bank-token-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Token Server APIs API
  slug: tsb-bank-token-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-token-server-apis-api-openapi.yml
authorization_urls:
- https://apis.tsb.co.uk/auth/oauth/v2/authorize
description: ''
docs: https://apis.tsb.co.uk/.well-known/openid-configuration
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Tsb Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TSB Bank publishes 9 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TSB Bank API on a user''s behalf.


  Tokens are issued from https://apis.tsb.co.uk/auth/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TSB Bank
provider_slug: tsb-bank
schemes:
- flows:
  - authorizationUrl: https://apis.tsb.co.uk/auth/oauth/v2/authorize
    flow: implicit
    registrationUrl: https://apis.tsb.co.uk/openid/connect/register
    tokenUrl: https://apis.tsb.co.uk/auth/oauth/v2/token
  name: OAuth2
  source: openapi/tsb-bank-oauth-server-openapi.json
scope_count: 9
scope_names:
- openid
- email
- profile
- phone
- address
- openid_client_registration
- accounts
- payments
- fundsconfirmations
scopes:
- description: For access to OpenID Connect endpoints (required for OIDC flows).
  flows:
  - implicit
  - authorizationCode
  scope: openid
- description: Access to the end-user email claim.
  flows:
  - implicit
  - authorizationCode
  scope: email
- description: Access to the end-user profile claims.
  flows:
  - implicit
  - authorizationCode
  scope: profile
- description: Access to the end-user phone claim.
  flows:
  - implicit
  scope: phone
- description: Access to the end-user address claim.
  flows:
  - implicit
  scope: address
- description: Dynamic client registration scope (OIDC/OBIE DCR at /openid/connect/register).
  flows:
  - authorizationCode
  scope: openid_client_registration
- description: OBIE Read/Write Account and Transaction Information (AIS) scope — read access to accounts, balances, transactions, beneficiaries, standing orders, direct debits, scheduled payments, and statements. OBIE standard scope; requires onboarding.
  flows:
  - authorizationCode
  scope: accounts
- description: OBIE Read/Write Payment Initiation (PIS) scope — initiate domestic and scheduled payments, standing orders, and file payments. OBIE standard scope; requires onboarding.
  flows:
  - authorizationCode
  scope: payments
- description: OBIE Read/Write Confirmation of Funds (CBPII) scope — confirm availability of funds on a customer account for a card-based payment instrument issuer. OBIE standard scope; requires onboarding.
  flows:
  - authorizationCode
  scope: fundsconfirmations
slug: tsb-bank-scopes
source_filename: tsb-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/tsb-bank-oauth-server-openapi.json\ndocs: https://apis.tsb.co.uk/.well-known/openid-configuration\nnotes: >-\n  OIDC/OAuth2 scopes enriched from TSB's live OpenID Provider discovery document\n  (apis.tsb.co.uk/.well-known/openid-configuration) and the OAuth Toolkit (OTK)\n  server OpenAPI. The OBIE Read/Write scopes (accounts, payments,\n  fundsconfirmations) are the standardized OBIE Open Banking scopes TSB's\n  FAPI-secured AIS/PIS/CBPII services require per the OBIE Security Profile; they\n  are not enumerated in the anonymous OTK discovery document and require\n  developer-portal onboarding with OBIE/eIDAS certificates to exercise.\nschemes:\n- name: OAuth2\n  source: openapi/tsb-bank-oauth-server-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://apis.tsb.co.uk/auth/oauth/v2/authorize\n    tokenUrl: https://apis.tsb.co.uk/auth/oauth/v2/token\n    registrationUrl: https://apis.tsb.co.uk/openid/connect/register\n\
  scopes:\n- scope: openid\n  description: For access to OpenID Connect endpoints (required for OIDC flows).\n  flows: [implicit, authorizationCode]\n  sources: [openapi/tsb-bank-oauth-server-openapi.json, well-known/tsb-bank-openid-configuration.json]\n- scope: email\n  description: Access to the end-user email claim.\n  flows: [implicit, authorizationCode]\n  sources: [openapi/tsb-bank-oauth-server-openapi.json, well-known/tsb-bank-openid-configuration.json]\n- scope: profile\n  description: Access to the end-user profile claims.\n  flows: [implicit, authorizationCode]\n  sources: [openapi/tsb-bank-oauth-server-openapi.json, well-known/tsb-bank-openid-configuration.json]\n- scope: phone\n  description: Access to the end-user phone claim.\n  flows: [implicit]\n  sources: [openapi/tsb-bank-oauth-server-openapi.json]\n- scope: address\n  description: Access to the end-user address claim.\n  flows: [implicit]\n  sources: [openapi/tsb-bank-oauth-server-openapi.json]\n- scope: openid_client_registration\n\
  \  description: Dynamic client registration scope (OIDC/OBIE DCR at /openid/connect/register).\n  flows: [authorizationCode]\n  sources: [well-known/tsb-bank-openid-configuration.json]\n- scope: accounts\n  description: >-\n    OBIE Read/Write Account and Transaction Information (AIS) scope — read access\n    to accounts, balances, transactions, beneficiaries, standing orders, direct\n    debits, scheduled payments, and statements. OBIE standard scope; requires\n    onboarding.\n  flows: [authorizationCode]\n  sources: [obie-security-profile]\n- scope: payments\n  description: >-\n    OBIE Read/Write Payment Initiation (PIS) scope — initiate domestic and\n    scheduled payments, standing orders, and file payments. OBIE standard scope;\n    requires onboarding.\n  flows: [authorizationCode]\n  sources: [obie-security-profile]\n- scope: fundsconfirmations\n  description: >-\n    OBIE Read/Write Confirmation of Funds (CBPII) scope — confirm availability of\n    funds on a customer account\
  \ for a card-based payment instrument issuer. OBIE\n    standard scope; requires onboarding.\n  flows: [authorizationCode]\n  sources: [obie-security-profile]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/scopes/tsb-bank-scopes.yml
summary_line: 9 scopes · implicit
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- FAPI
- Fintech
token_urls:
- https://apis.tsb.co.uk/auth/oauth/v2/token
---
