---
api_specs:
- filename: natwest-account-transaction-openapi.yml
  format: yaml
  label: NatWest Account and Transaction API
  slug: natwest-account-and-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-account-transaction-openapi.yml
- filename: natwest-payment-initiation-openapi.yml
  format: yaml
  label: NatWest Payment Initiation API
  slug: natwest-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-payment-initiation-openapi.yml
- filename: natwest-confirmation-of-funds-openapi.yml
  format: yaml
  label: NatWest Confirmation of Funds API
  slug: natwest-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-confirmation-of-funds-openapi.yml
authorization_urls: []
description: ''
docs: https://www.bankofapis.com/documentation/security
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Natwest Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NatWest Group publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the NatWest Group API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NatWest Group
provider_slug: natwest
schemes:
- description: TPP client-credentials flow with the ASPSP.
  flow: clientCredentials
  name: TPPOAuth2Security
  tokenUrl: https://ob.sandbox.natwest.com/token
- authorizationUrl: https://api.sandbox.natwest.com/authorize
  description: PSU authorisation-code flow with PSD2 SCA.
  flow: authorizationCode
  name: PSUOAuth2Security
  tokenUrl: https://ob.sandbox.natwest.com/token
scope_count: 5
scope_names:
- openid
- accounts
- payments
- fundsconfirmations
- profile
scopes:
- description: OpenID Connect authentication (required for the PSU authorization_code flow).
  flows:
  - authorizationCode
  scope: openid
- description: Read account and transaction information (AISP).
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: Initiate payments (PISP).
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: Confirmation of funds entitlement (CBPII).
  flows:
  - authorizationCode
  - clientCredentials
  scope: fundsconfirmations
- description: PSU profile claims exposed via OIDC.
  flows:
  - authorizationCode
  scope: profile
slug: natwest-scopes
source_filename: natwest-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/*; https://api.sandbox.natwest.com/.well-known/openid-configuration\ndocs: https://www.bankofapis.com/documentation/security\nschemes:\n- name: TPPOAuth2Security\n  flow: clientCredentials\n  tokenUrl: https://ob.sandbox.natwest.com/token\n  description: TPP client-credentials flow with the ASPSP.\n- name: PSUOAuth2Security\n  flow: authorizationCode\n  authorizationUrl: https://api.sandbox.natwest.com/authorize\n  tokenUrl: https://ob.sandbox.natwest.com/token\n  description: PSU authorisation-code flow with PSD2 SCA.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (required for the PSU authorization_code flow).\n  flows: [authorizationCode]\n- scope: accounts\n  description: Read account and transaction information (AISP).\n  flows: [authorizationCode, clientCredentials]\n  sources: [openapi/natwest-account-transaction-openapi.yml]\n- scope: payments\n  description: Initiate payments (PISP).\n\
  \  flows: [authorizationCode, clientCredentials]\n  sources: [openapi/natwest-payment-initiation-openapi.yml]\n- scope: fundsconfirmations\n  description: Confirmation of funds entitlement (CBPII).\n  flows: [authorizationCode, clientCredentials]\n  sources: [openapi/natwest-confirmation-of-funds-openapi.yml]\n- scope: profile\n  description: PSU profile claims exposed via OIDC.\n  flows: [authorizationCode]\nnotes: >-\n  Scope list confirmed against the live sandbox OIDC discovery document\n  (scopes_supported: openid, payments, accounts, fundsconfirmations, profile). The\n  spec token/authorization URLs are OBIE placeholders (authserver.example); the real\n  sandbox endpoints are shown above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/scopes/natwest-scopes.yml
summary_line: 5 scopes
tags:
- Banking
- Open Banking
- Financial Services
- Payments
- PSD2
- FAPI
- Fintech
- Account Information
token_urls: []
---
