---
api_specs:
- filename: openpayments-io-account-information-service-ais-api-openapi.yml
  format: yaml
  label: Open Payments Account Information Service (AIS) API
  slug: openpayments-io-account-information-service-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-account-information-service-ais-api-openapi.yml
- filename: openpayments-io-aspsp-information-service-api-openapi.yml
  format: yaml
  label: Open Payments ASPSP Information Service API
  slug: openpayments-io-aspsp-information-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-aspsp-information-service-api-openapi.yml
- filename: openpayments-io-bankgiro-lookup-api-openapi.yml
  format: yaml
  label: Open Payments Bankgiro Lookup API
  slug: openpayments-io-bankgiro-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-bankgiro-lookup-api-openapi.yml
- filename: openpayments-io-consent-service-api-openapi.yml
  format: yaml
  label: Open Payments Consent Service API
  slug: openpayments-io-consent-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-consent-service-api-openapi.yml
- filename: openpayments-io-fx-connect-api-openapi.yml
  format: yaml
  label: Open Payments FX Connect API
  slug: openpayments-io-fx-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-fx-connect-api-openapi.yml
- filename: openpayments-io-iso-payments-api-openapi.yml
  format: yaml
  label: Open Payments ISO Payments API
  slug: openpayments-io-iso-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-iso-payments-api-openapi.yml
- filename: openpayments-io-kyc-service-api-openapi.yml
  format: yaml
  label: Open Payments KYC Service API
  slug: openpayments-io-kyc-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-kyc-service-api-openapi.yml
- filename: openpayments-io-payment-initiation-service-pis-api-openapi.yml
  format: yaml
  label: Open Payments Payment Initiation Service (PIS) API
  slug: openpayments-io-payment-initiation-service-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-payment-initiation-service-pis-api-openapi.yml
- filename: openpayments-io-payout-service-api-openapi.yml
  format: yaml
  label: Open Payments Payout Service API
  slug: openpayments-io-payout-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-payout-service-api-openapi.yml
- filename: openpayments-io-sepa-direct-debit-api-openapi.yml
  format: yaml
  label: Open Payments SEPA Direct Debit API
  slug: openpayments-io-sepa-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-sepa-direct-debit-api-openapi.yml
- filename: openpayments-io-verification-of-payee-vop-api-openapi.yml
  format: yaml
  label: Open Payments Verification of Payee (VoP) API
  slug: openpayments-io-verification-of-payee-vop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-verification-of-payee-vop-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Openpayments Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Open Payments publishes 13 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Open Payments API on a user''s behalf.


  Tokens are issued from https://auth.sandbox.openbankingplatform.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Open Payments
provider_slug: openpayments-io
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sandbox.openbankingplatform.com/connect/token
  name: oAuth2Sandbox
  source: openapi/openpayments-io-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.openbankingplatform.com/connect/token
  name: oAuth2Production
  source: openapi/openpayments-io-openapi.yml
scope_count: 13
scope_names:
- accountinformation
- accountinformation bankgiroinformation corporate
- accountinformation corporate
- accountinformation private
- aspspinformation
- aspspinformation corporate
- aspspinformation private
- bankgiroinformation
- corporate
- paymentinitiation
- paymentinitiation corporate
- paymentinitiation private
- private
scopes:
- description: Account Information
  flows:
  - clientCredentials
  scope: accountinformation
- description: ''
  flows: []
  scope: accountinformation bankgiroinformation corporate
- description: ''
  flows: []
  scope: accountinformation corporate
- description: ''
  flows: []
  scope: accountinformation private
- description: ASPSP Information
  flows:
  - clientCredentials
  scope: aspspinformation
- description: ''
  flows: []
  scope: aspspinformation corporate
- description: ''
  flows: []
  scope: aspspinformation private
- description: Account Information Enrichment
  flows:
  - clientCredentials
  scope: bankgiroinformation
- description: Corporate accounts context
  flows:
  - clientCredentials
  scope: corporate
- description: Payment Initiation
  flows:
  - clientCredentials
  scope: paymentinitiation
- description: ''
  flows: []
  scope: paymentinitiation corporate
- description: ''
  flows: []
  scope: paymentinitiation private
- description: Private accounts context
  flows:
  - clientCredentials
  scope: private
slug: openpayments-io-scopes
source_filename: openpayments-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: derived\nsource: openapi/openpayments-io-openapi.yml\nschemes:\n- name: oAuth2Sandbox\n  source: openapi/openpayments-io-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sandbox.openbankingplatform.com/connect/token\n- name: oAuth2Production\n  source: openapi/openpayments-io-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.openbankingplatform.com/connect/token\nscopes:\n- scope: accountinformation\n  description: Account Information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: accountinformation bankgiroinformation corporate\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: accountinformation corporate\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: accountinformation private\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: aspspinformation\n  description: ASPSP Information\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: aspspinformation corporate\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: aspspinformation private\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: bankgiroinformation\n  description: Account Information Enrichment\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: corporate\n  description: Corporate accounts context\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: paymentinitiation\n  description: Payment Initiation\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: paymentinitiation corporate\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: paymentinitiation private\n  sources:\n  - openapi/openpayments-io-openapi.yml\n- scope: private\n  description: Private accounts context\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openpayments-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/scopes/openpayments-io-scopes.yml
summary_line: 13 scopes · clientCredentials
tags:
- Company
- Payments
- Banking
- Fintech
token_bound: false
token_urls:
- https://auth.sandbox.openbankingplatform.com/connect/token
- https://auth.openbankingplatform.com/connect/token
---
