---
api_specs:
- filename: novopayment-accounts-openapi.yml
  format: yaml
  label: NovoPayment Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-accounts-openapi.yml
- filename: novopayment-alias-directory-openapi.yml
  format: yaml
  label: NovoPayment Alias Directory API
  slug: alias-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-alias-directory-openapi.yml
- filename: novopayment-cards-openapi.yml
  format: yaml
  label: NovoPayment Cards API
  slug: cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-cards-openapi.yml
- filename: novopayment-compliance-openapi.yml
  format: yaml
  label: NovoPayment Compliance API
  slug: compliance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-compliance-openapi.yml
- filename: novopayment-customers-openapi.yml
  format: yaml
  label: NovoPayment Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-customers-openapi.yml
- filename: novopayment-issuer-tokenization-openapi.yml
  format: yaml
  label: NovoPayment Issuer Tokenization API
  slug: issuer-tokenization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-issuer-tokenization-openapi.yml
- filename: novopayment-mastercard-issuer-tokenization-openapi.yml
  format: yaml
  label: NovoPayment MasterCard Tokenization API
  slug: mastercard-issuer-tokenization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-mastercard-issuer-tokenization-openapi.yml
- filename: novopayment-merchant-presented-qr-openapi.yml
  format: yaml
  label: NovoPayment Merchant Presented QR
  slug: merchant-presented-qr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-merchant-presented-qr-openapi.yml
- filename: novopayment-oauth2-data-encryption-openapi.yml
  format: yaml
  label: NovoPayment Security OAuth2 API
  slug: oauth2-data-encryption
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-oauth2-data-encryption-openapi.yml
- filename: novopayment-onboarding-openapi.yml
  format: yaml
  label: NovoPayment Onboarding API
  slug: onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-onboarding-openapi.yml
- filename: novopayment-operations-openapi.yml
  format: yaml
  label: NovoPayment Operations API
  slug: operations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-operations-openapi.yml
- filename: novopayment-payment-authorizer-openapi.yml
  format: yaml
  label: NovoPayment Payment Authorizer API
  slug: payment-authorizer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-payment-authorizer-openapi.yml
- filename: novopayment-profile-openapi.yml
  format: yaml
  label: NovoPayment Profile API
  slug: profile
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-profile-openapi.yml
- filename: novopayment-push-provisioning-openapi.yml
  format: yaml
  label: NovoPayment Push Provisioning API
  slug: push-provisioning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-push-provisioning-openapi.yml
- filename: novopayment-real-time-payments-openapi.yml
  format: yaml
  label: NovoPayment Real-Time Payments API
  slug: real-time-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-real-time-payments-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.novopayment.com/api/data-encryption/oauth2-data-encryption-api-v1.0
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Novopayment Scopes
name_suffix: OAuth Scopes
note: NovoPayment declares an OAuth2 clientCredentials flow with an EMPTY scopes map in all 12 specs that carry it, and publishes no scope or permission reference page. Access is partitioned by which APIs a project selects in the developer hub dashboard, not by scope on the token — so a token cannot be least-privileged within a project.
overview: 'NovoPayment uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox-api.novopayment.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NovoPayment
provider_slug: novopayment
schemes:
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-accounts-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-alias-directory-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-cards-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-compliance-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-customers-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-mastercard-issuer-tokenization-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-merchant-presented-qr-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-onboarding-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-operations-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-profile-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-push-provisioning-openapi.yml
- description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/novopayment-real-time-payments-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: novopayment-scopes
source_filename: novopayment-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: derived\nsource: openapi/novopayment-accounts-openapi.yml, openapi/novopayment-alias-directory-openapi.yml, openapi/novopayment-cards-openapi.yml,\n  openapi/novopayment-compliance-openapi.yml, openapi/novopayment-customers-openapi.yml, openapi/novopayment-mastercard-issuer-tokenization-openapi.yml,\n  openapi/novopayment-merchant-presented-qr-openapi.yml, openapi/novopayment-onboarding-openapi.yml, openapi/novopayment-operations-openapi.yml,\n  openapi/novopayment-profile-openapi.yml, openapi/novopayment-push-provisioning-openapi.yml, openapi/novopayment-real-time-payments-openapi.yml\nschemes:\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-accounts-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source:\
  \ openapi/novopayment-alias-directory-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-cards-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-compliance-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-customers-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-mastercard-issuer-tokenization-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-merchant-presented-qr-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-onboarding-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n\
  \  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-operations-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-profile-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n- name: oAuth2ClientCredentials\n  source: openapi/novopayment-push-provisioning-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\n\
  - name: oAuth2ClientCredentials\n  source: openapi/novopayment-real-time-payments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-api.novopayment.com/oauth2/token\n  description: See [Oauth2 API](https://developer.novopayment.com/api/authentication-method-and-encryption/oauth2-api)\nscopes: []\ndocs: https://developer.novopayment.com/api/data-encryption/oauth2-data-encryption-api-v1.0\nscope_count: 0\nnote: NovoPayment declares an OAuth2 clientCredentials flow with an EMPTY scopes map in all 12 specs that carry\n  it, and publishes no scope or permission reference page. Access is partitioned by which APIs a project selects\n  in the developer hub dashboard, not by scope on the token — so a token cannot be least-privileged within a project.\nsearched:\n- url: https://developer.novopayment.com/api/data-encryption/oauth2-data-encryption-api-v1.0\n  status: 200\n  result: token issuance documented; no scopes\n- url: https://developer.novopayment.com/guides/how-it-works/get-access-token\n\
  \  status: 200\n  result: no scope or permission reference\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/scopes/novopayment-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Payments
- Banking as a Service
- Embedded Finance
- Card Issuing
- Digital Wallet
- Tokenization
- Real-Time Payments
- Onboarding
- KYC
- Latin America
- Fintech
- Digital Banking
token_urls:
- https://sandbox-api.novopayment.com/oauth2/token
---
