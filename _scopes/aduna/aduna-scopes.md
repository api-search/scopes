---
authorization_urls: []
description: ''
docs: https://docs.adunaglobal.com/how-to-enable-an-api/number-verification-api-v-2.1-landing-page
flows:
- authorizationCode
- urn:ietf:params:oauth:grant-type:jwt-bearer
- ciba
kind: oauth-scopes
layout: scope
method: searched
name: Aduna Scopes
name_suffix: OAuth Scopes
note: Aduna publishes no OpenAPI and its scope reference sits behind the portal login wall. These scopes are read verbatim from the default values in Aduna's own source-available Java SDK configuration class and are restated in the SDK README configuration table. They follow the CAMARA convention of pairing an OIDC scope with a W3C DPV purpose and a per-operation API scope. Only the Number Verification API's scopes are publicly visible; the SIM Swap, KYC Match and roadmap APIs will have their own CAMARA scopes but none are published.
overview: 'Aduna publishes 4 OAuth 2.0 scopes via the authorizationCode, urn:ietf:params:oauth:grant-type:jwt-bearer, and ciba flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aduna API on a user''s behalf.


  Tokens are issued from {baseURL}/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aduna
provider_slug: aduna
schemes:
- flows:
  - flow: authorizationCode
    tokenUrl: '{baseURL}/auth/token'
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: '{baseURL}/auth/token'
  - backchannelAuthorizationUrl: '{baseURL}/auth/bc-authorize'
    flow: ciba
    tokenUrl: '{baseURL}/auth/token'
  name: Aduna authorization (network- and SIM-based)
  source: authentication/aduna-authentication.yml
scope_count: 4
scope_names:
- openid
- dpv:FraudPreventionAndDetection
- number-verification:verify
- number-verification:device-phone-number:read
scopes:
- description: OpenID Connect authentication; required on every Aduna Number Verification request.
  flows: []
  scope: openid
- description: W3C Data Privacy Vocabulary purpose scope declaring that the personal data is processed for fraud prevention and detection. CAMARA requires a dpv purpose alongside the API scope.
  flows: []
  scope: dpv:FraudPreventionAndDetection
- description: Verify that a supplied phone number matches the phone number of the device holding the authenticated SIM. Backs POST /number-verification/v2/verify.
  flows: []
  scope: number-verification:verify
- description: Retrieve the phone number of the device holding the authenticated SIM (number share). Backs GET /number-verification/v2/device-phone-number.
  flows: []
  scope: number-verification:device-phone-number:read
slug: aduna-scopes
source_filename: aduna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://github.com/adunaglobal/nv2-asp-server-java-aduna-sdk/blob/main/backend/src/main/java/com/adunaglobal/sdk/backend/configuration/NumberVerificationProperties.java\ndocs: https://docs.adunaglobal.com/how-to-enable-an-api/number-verification-api-v-2.1-landing-page\ndocs_gated: true\nnote: >-\n  Aduna publishes no OpenAPI and its scope reference sits behind the portal login wall. These\n  scopes are read verbatim from the default values in Aduna's own source-available Java SDK\n  configuration class and are restated in the SDK README configuration table. They follow the\n  CAMARA convention of pairing an OIDC scope with a W3C DPV purpose and a per-operation API scope.\n  Only the Number Verification API's scopes are publicly visible; the SIM Swap, KYC Match and\n  roadmap APIs will have their own CAMARA scopes but none are published.\nschemes:\n- name: Aduna authorization (network- and SIM-based)\n  source: authentication/aduna-authentication.yml\n\
  \  flows:\n  - flow: authorizationCode\n    tokenUrl: '{baseURL}/auth/token'\n  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer\n    tokenUrl: '{baseURL}/auth/token'\n  - flow: ciba\n    backchannelAuthorizationUrl: '{baseURL}/auth/bc-authorize'\n    tokenUrl: '{baseURL}/auth/token'\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; required on every Aduna Number Verification request.\n  kind: oidc\n  operations: [verify, read]\n- scope: dpv:FraudPreventionAndDetection\n  description: >-\n    W3C Data Privacy Vocabulary purpose scope declaring that the personal data is processed for\n    fraud prevention and detection. CAMARA requires a dpv purpose alongside the API scope.\n  kind: purpose\n  operations: [verify, read]\n- scope: number-verification:verify\n  description: >-\n    Verify that a supplied phone number matches the phone number of the device holding the\n    authenticated SIM. Backs POST /number-verification/v2/verify.\n  kind: api\n  operations: [verify]\n\
  - scope: number-verification:device-phone-number:read\n  description: >-\n    Retrieve the phone number of the device holding the authenticated SIM (number share). Backs\n    GET /number-verification/v2/device-phone-number.\n  kind: api\n  operations: [read]\nscope_sets:\n- operation: verify\n  property: com.adunaglobal.sdk.backend.api.numberVerification.verifyScopes\n  value: openid dpv:FraudPreventionAndDetection number-verification:verify\n- operation: read\n  property: com.adunaglobal.sdk.backend.api.numberVerification.readScopes\n  value: openid dpv:FraudPreventionAndDetection number-verification:device-phone-number:read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aduna/refs/heads/main/scopes/aduna-scopes.yml
summary_line: 4 scopes · authorizationCode/urn:ietf:params:oauth:grant-type:jwt-bearer/ciba
tags:
- Telecommunications
- Sweden
- Network APIs
- CAMARA
- Open Gateway
- API Aggregator
- Identity Verification
- SIM Swap
- Number Verification
- Fraud Prevention
- Quality on Demand
- Device Location
- Ericsson
token_urls:
- '{baseURL}/auth/token'
---
