---
api_specs:
- filename: hampden-and-co-account-information-api-openapi.yml
  format: yaml
  label: Hampden & Co Account & Transaction Information API
  slug: hampden-and-co-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/openapi/hampden-and-co-account-information-api-openapi.yml
- filename: hampden-and-co-payment-initiation-api-openapi.yml
  format: yaml
  label: Hampden & Co Payment Initiation API
  slug: hampden-and-co-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/openapi/hampden-and-co-payment-initiation-api-openapi.yml
- filename: hampden-and-co-confirmation-of-funds-api-openapi.yml
  format: yaml
  label: Hampden & Co Confirmation of Funds API
  slug: hampden-and-co-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml
authorization_urls:
- https://authserver.example/authorization
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hampden And Co Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hampden & Co publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hampden & Co API on a user''s behalf.


  Tokens are issued from https://authserver.example/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hampden & Co
provider_slug: hampden-and-co
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  source: openapi/hampden-and-co-account-information-api-openapi.yml
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  source: openapi/hampden-and-co-account-information-api-openapi.yml
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  source: openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  source: openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  source: openapi/hampden-and-co-payment-initiation-api-openapi.yml
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  source: openapi/hampden-and-co-payment-initiation-api-openapi.yml
scope_count: 3
scope_names:
- accounts
- fundsconfirmations
- payments
scopes:
- description: Ability to read Accounts information
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: Funds confirmation entitlement
  flows:
  - authorizationCode
  - clientCredentials
  scope: fundsconfirmations
- description: Generic payment scope
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
slug: hampden-and-co-scopes
source_filename: hampden-and-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/hampden-and-co-account-information-api-openapi.yml, openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml,\n  openapi/hampden-and-co-payment-initiation-api-openapi.yml\nschemes:\n- name: TPPOAuth2Security\n  source: openapi/hampden-and-co-account-information-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n  description: TPP client credential authorisation flow with the ASPSP\n- name: PSUOAuth2Security\n  source: openapi/hampden-and-co-account-information-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n- name: TPPOAuth2Security\n  source: openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n  description: TPP client credential authorisation flow with the ASPSP\n- name: PSUOAuth2Security\n  source: openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n- name: TPPOAuth2Security\n  source: openapi/hampden-and-co-payment-initiation-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n  description: TPP client credential authorisation flow with the ASPSP\n- name: PSUOAuth2Security\n  source: openapi/hampden-and-co-payment-initiation-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n\
  \    tokenUrl: https://authserver.example/token\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\nscopes:\n- scope: accounts\n  description: Ability to read Accounts information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/hampden-and-co-account-information-api-openapi.yml\n- scope: fundsconfirmations\n  description: Funds confirmation entitlement\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml\n- scope: payments\n  description: Generic payment scope\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/hampden-and-co-payment-initiation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/scopes/hampden-and-co-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Financial-Services
- Banking
- Private Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
token_urls:
- https://authserver.example/token
---
