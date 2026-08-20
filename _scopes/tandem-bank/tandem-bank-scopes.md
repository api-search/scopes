---
api_specs:
- filename: obie-standard-account-info-openapi.yaml
  format: yaml
  label: Tandem Bank Account and Transaction Information API (AIS)
  slug: tandem-bank-account-transaction-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tandem-bank/refs/heads/main/openapi/obie-standard-account-info-openapi.yaml
- filename: obie-standard-payment-initiation-openapi.yaml
  format: yaml
  label: Tandem Bank Payment Initiation API (PIS)
  slug: tandem-bank-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tandem-bank/refs/heads/main/openapi/obie-standard-payment-initiation-openapi.yaml
- filename: obie-standard-confirmation-funds-openapi.yaml
  format: yaml
  label: Tandem Bank Confirmation of Funds API (CBPII)
  slug: tandem-bank-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tandem-bank/refs/heads/main/openapi/obie-standard-confirmation-funds-openapi.yaml
authorization_urls:
- https://authserver.example/authorization
description: ''
docs: https://openbankinguk.github.io/read-write-api-site3/v4.0/profiles/read-write-data-api-profile.html
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tandem Bank Scopes
name_suffix: OAuth Scopes
note: 'Scopes are the coarse-grained OAuth2 scopes defined by the OBIE Read/Write API Standard that Tandem Bank''s Token-provided dedicated interface conforms to. A TPP''s software statement must be permitted the relevant scope: "accounts" for the AIS/Account and Transaction API, "payments" for the PIS/Payment Initiation API, and "fundsconfirmations" for the CBPII/Confirmation of Funds API. Fine-grained permissions are expressed per-request through OBIE intents (account-access-consent, funds-confirmation-consent, and the payment-order consents) authorised by the PSU under PSD2 Strong Customer Authentication, not through additional OAuth scopes.'
overview: 'Tandem Bank publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tandem Bank API on a user''s behalf.


  Tokens are issued from https://authserver.example/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tandem Bank
provider_slug: tandem-bank
schemes:
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  source: openapi/obie-standard-account-info-openapi.yaml
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  source: openapi/obie-standard-account-info-openapi.yaml
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  source: openapi/obie-standard-confirmation-funds-openapi.yaml
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  source: openapi/obie-standard-confirmation-funds-openapi.yaml
- description: TPP client credential authorisation flow with the ASPSP
  flows:
  - flow: clientCredentials
    tokenUrl: https://authserver.example/token
  name: TPPOAuth2Security
  source: openapi/obie-standard-payment-initiation-openapi.yaml
- description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when a TPP wants to access an ASPSP resource owned by the PSU
  flows:
  - authorizationUrl: https://authserver.example/authorization
    flow: authorizationCode
    tokenUrl: https://authserver.example/token
  name: PSUOAuth2Security
  source: openapi/obie-standard-payment-initiation-openapi.yaml
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
slug: tandem-bank-scopes
source_filename: tandem-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/obie-standard-account-info-openapi.yaml, openapi/obie-standard-confirmation-funds-openapi.yaml,\n  openapi/obie-standard-payment-initiation-openapi.yaml\ndocs: https://openbankinguk.github.io/read-write-api-site3/v4.0/profiles/read-write-data-api-profile.html\nnote: >-\n  Scopes are the coarse-grained OAuth2 scopes defined by the OBIE Read/Write API\n  Standard that Tandem Bank's Token-provided dedicated interface conforms to.\n  A TPP's software statement must be permitted the relevant scope: \"accounts\"\n  for the AIS/Account and Transaction API, \"payments\" for the PIS/Payment\n  Initiation API, and \"fundsconfirmations\" for the CBPII/Confirmation of Funds\n  API. Fine-grained permissions are expressed per-request through OBIE intents\n  (account-access-consent, funds-confirmation-consent, and the payment-order\n  consents) authorised by the PSU under PSD2 Strong Customer Authentication,\n  not through additional\
  \ OAuth scopes.\nschemes:\n- name: TPPOAuth2Security\n  source: openapi/obie-standard-account-info-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n  description: TPP client credential authorisation flow with the ASPSP\n- name: PSUOAuth2Security\n  source: openapi/obie-standard-account-info-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n- name: TPPOAuth2Security\n  source: openapi/obie-standard-confirmation-funds-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n  description: TPP client credential authorisation flow with the ASPSP\n- name: PSUOAuth2Security\n  source: openapi/obie-standard-confirmation-funds-openapi.yaml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\n- name: TPPOAuth2Security\n  source: openapi/obie-standard-payment-initiation-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authserver.example/token\n  description: TPP client credential authorisation flow with the ASPSP\n- name: PSUOAuth2Security\n  source: openapi/obie-standard-payment-initiation-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.example/authorization\n    tokenUrl: https://authserver.example/token\n  description: OAuth flow, it is required when the PSU needs to perform SCA with the ASPSP when\n    a TPP wants to access an ASPSP resource owned by the PSU\nscopes:\n- scope: accounts\n  description:\
  \ Ability to read Accounts information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/obie-standard-account-info-openapi.yaml\n- scope: fundsconfirmations\n  description: Funds confirmation entitlement\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/obie-standard-confirmation-funds-openapi.yaml\n- scope: payments\n  description: Generic payment scope\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/obie-standard-payment-initiation-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tandem-bank/refs/heads/main/scopes/tandem-bank-scopes.yml
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
