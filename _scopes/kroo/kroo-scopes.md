---
api_specs:
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Kroo Account and Transaction Information API
  slug: kroo-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Kroo Payment Initiation API
  slug: kroo-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Kroo Confirmation of Funds API
  slug: kroo-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
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
name: Kroo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kroo publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kroo API on a user''s behalf.


  Tokens are issued from https://authserver.example/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kroo
provider_slug: kroo
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  source: openapi/obie-account-info-openapi.yaml
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  source: openapi/obie-account-info-openapi.yaml
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  source: openapi/obie-confirmation-funds-openapi.yaml
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  source: openapi/obie-confirmation-funds-openapi.yaml
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  source: openapi/obie-payment-initiation-openapi.yaml
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  source: openapi/obie-payment-initiation-openapi.yaml
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
slug: kroo-scopes
source_filename: kroo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/obie-account-info-openapi.yaml, openapi/obie-confirmation-funds-openapi.yaml,\n  openapi/obie-payment-initiation-openapi.yaml\nschemes:\n- name: TPPOAuth2Security\n  source: openapi/obie-account-info-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n  description: TPP client credential authorisation flow with the ASPSP\n- name: PSUOAuth2Security\n  source: openapi/obie-account-info-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n- name: TPPOAuth2Security\n  source: openapi/obie-confirmation-funds-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n\
  \  description: TPP client credential authorisation flow with the ASPSP\n- name: PSUOAuth2Security\n  source: openapi/obie-confirmation-funds-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n- name: TPPOAuth2Security\n  source: openapi/obie-payment-initiation-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n  description: TPP client credential authorisation flow with the ASPSP\n- name: PSUOAuth2Security\n  source: openapi/obie-payment-initiation-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n  description: OAuth flow, it is required when the PSU needs\
  \ to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\nscopes:\n- scope: accounts\n  description: Ability to read Accounts information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/obie-account-info-openapi.yaml\n- scope: fundsconfirmations\n  description: Funds confirmation entitlement\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/obie-confirmation-funds-openapi.yaml\n- scope: payments\n  description: Generic payment scope\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/obie-payment-initiation-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/scopes/kroo-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech
token_urls:
- https://authserver.example/token
---
