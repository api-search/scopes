---
api_specs:
- filename: yorkshire-building-society-account-information-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Account Information API
  slug: ybs-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-account-information-api-openapi.yaml
- filename: yorkshire-building-society-payment-initiation-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Payment Initiation API
  slug: ybs-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-payment-initiation-api-openapi.yaml
- filename: yorkshire-building-society-confirmation-of-funds-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Confirmation of Funds API
  slug: ybs-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-confirmation-of-funds-api-openapi.yaml
- filename: yorkshire-building-society-event-subscriptions-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Event Subscriptions API
  slug: ybs-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-event-subscriptions-api-openapi.yaml
authorization_urls: []
description: ''
docs: https://api.ybs.co.uk/open-banking/v1.0/.well-known/ybs/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Yorkshire Building Society Scopes
name_suffix: OAuth Scopes
note: Scope set and endpoints upgraded from the live OBIE OpenID Provider discovery documents (well-known/*-openid-configuration.json). Production issuers are https://ob-ybs.api.ybs.co.uk (YBS/CBS) and https://ob-che.api.ybs.co.uk (Chelsea). The OpenAPI files ship placeholder authserver.example URLs; the real authorization/token endpoints are recorded below. All access tokens are mutual-TLS certificate-bound (tls_client_certificate_bound_access_tokens).
overview: 'Yorkshire Building Society publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Yorkshire Building Society API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yorkshire Building Society
provider_slug: yorkshire-building-society
schemes:
- authorizationUrl: https://authorisation.ybs.co.uk/public/authentication/pre_login.do
  flow: authorizationCode
  name: PSUOAuth2Security
  note: PSU-present flow requiring PSD2 strong customer authentication (SCA).
  tokenUrl: https://ob-ybs.api.ybs.co.uk/identity/open-banking/v3.1/token
  type: oauth2
- flow: clientCredentials
  name: TPPOAuth2Security
  note: TPP client-credentials flow for consent creation and non-PSU resources.
  tokenUrl: https://ob-ybs.api.ybs.co.uk/identity/open-banking/v3.1/token
  type: oauth2
scope_count: 4
scope_names:
- openid
- accounts
- payments
- fundsconfirmations
scopes:
- description: OpenID Connect authentication; returns an id_token binding the openbanking_intent_id.
  flows:
  - authorizationCode
  scope: openid
- description: Account Information (AIS) - read accounts, balances, transactions, beneficiaries, standing orders, direct debits, products, parties and statements.
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: Payment Initiation (PIS) - set up payment/standing-order/file-payment consents and initiate domestic, scheduled, standing-order and file payments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: Confirmation of Funds (CBPII) - set up a funds-confirmation consent and confirm available funds on a payment account.
  flows:
  - authorizationCode
  - clientCredentials
  scope: fundsconfirmations
slug: yorkshire-building-society-scopes
source_filename: yorkshire-building-society-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/yorkshire-building-society-account-information-api-openapi.yaml, openapi/yorkshire-building-society-payment-initiation-api-openapi.yaml, openapi/yorkshire-building-society-confirmation-of-funds-api-openapi.yaml, openapi/yorkshire-building-society-event-subscriptions-api-openapi.yaml\ndocs: https://api.ybs.co.uk/open-banking/v1.0/.well-known/ybs/openid-configuration\nnote: >-\n  Scope set and endpoints upgraded from the live OBIE OpenID Provider discovery\n  documents (well-known/*-openid-configuration.json). Production issuers are\n  https://ob-ybs.api.ybs.co.uk (YBS/CBS) and https://ob-che.api.ybs.co.uk\n  (Chelsea). The OpenAPI files ship placeholder authserver.example URLs; the\n  real authorization/token endpoints are recorded below. All access tokens are\n  mutual-TLS certificate-bound (tls_client_certificate_bound_access_tokens).\nstandard: OBIE Read/Write Data API Standard v3.1.2 (UK Open Banking / PSD2)\nschemes:\n\
  - name: PSUOAuth2Security\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://authorisation.ybs.co.uk/public/authentication/pre_login.do\n  tokenUrl: https://ob-ybs.api.ybs.co.uk/identity/open-banking/v3.1/token\n  note: PSU-present flow requiring PSD2 strong customer authentication (SCA).\n- name: TPPOAuth2Security\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://ob-ybs.api.ybs.co.uk/identity/open-banking/v3.1/token\n  note: TPP client-credentials flow for consent creation and non-PSU resources.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an id_token binding the openbanking_intent_id.\n  flows: [authorizationCode]\n- scope: accounts\n  description: Account Information (AIS) - read accounts, balances, transactions, beneficiaries, standing orders, direct debits, products, parties and statements.\n  flows: [authorizationCode, clientCredentials]\n- scope: payments\n  description: Payment Initiation (PIS) - set up payment/standing-order/file-payment\
  \ consents and initiate domestic, scheduled, standing-order and file payments.\n  flows: [authorizationCode, clientCredentials]\n- scope: fundsconfirmations\n  description: Confirmation of Funds (CBPII) - set up a funds-confirmation consent and confirm available funds on a payment account.\n  flows: [authorizationCode, clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/scopes/yorkshire-building-society-scopes.yml
summary_line: 4 scopes
tags:
- Financial Services
- Banking
- Building Society
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Fintech
token_urls: []
---
