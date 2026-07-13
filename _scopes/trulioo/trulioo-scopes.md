---
api_specs:
- filename: trulioo-verifications-api-openapi.yml
  format: yaml
  label: Trulioo Verifications API
  slug: trulioo-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-verifications-api-openapi.yml
- filename: trulioo-configuration-api-openapi.yml
  format: yaml
  label: Trulioo Configuration API
  slug: trulioo-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-configuration-api-openapi.yml
- filename: trulioo-connection-api-openapi.yml
  format: yaml
  label: Trulioo Connection API
  slug: trulioo-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-connection-api-openapi.yml
- filename: trulioo-business-verification-api-openapi.yml
  format: yaml
  label: Trulioo Business Verification API
  slug: trulioo-business-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-business-verification-api-openapi.yml
- filename: trulioo-person-fraud-api-openapi.yml
  format: yaml
  label: Trulioo Person Fraud API
  slug: trulioo-person-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-person-fraud-api-openapi.yml
- filename: trulioo-document-verification-api-openapi.yml
  format: yaml
  label: Trulioo Identity Document Verification API
  slug: trulioo-document-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-document-verification-api-openapi.yml
- filename: trulioo-platform-api-openapi.yml
  format: yaml
  label: Trulioo Platform API
  slug: trulioo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-platform-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.trulioo.com/reference/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Trulioo Scopes
name_suffix: OAuth Scopes
note: Trulioo uses the OAuth2 client_credentials flow with service- and region-scoped values (for example docv.api.us for DocV in the US region); only the scopes above are documented publicly, and no full scope catalog is published (https://developer.trulioo.com/reference/authorization-2).
overview: 'Trulioo publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Trulioo API on a user''s behalf.


  Tokens are issued from https://auth-api.trulioo.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Trulioo
provider_slug: trulioo
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth-api.trulioo.com/connect/token
  name: OAuth2
  source: openapi/trulioo-business-verification-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth-api.trulioo.com/connect/token
  name: OAuth2
  source: openapi/trulioo-configuration-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth-api.trulioo.com/connect/token
  name: OAuth2
  source: openapi/trulioo-connection-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth-api.trulioo.com/connect/token
  name: OAuth2
  source: openapi/trulioo-document-verification-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth-api.trulioo.com/connect/token
  name: OAuth2
  source: openapi/trulioo-person-fraud-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.trulioo.com/customer/v2/auth/customer
  name: OAuth2
  source: openapi/trulioo-platform-api-openapi.yml
- description: Two-legged client credentials OAuth2 flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth-api.trulioo.com/connect/token
  name: OAuth2
  source: openapi/trulioo-verifications-api-openapi.yml
scope_count: 3
scope_names:
- napi.api
- workflow.studio.api
- docv.api.us
scopes:
- description: Grants access to the Normalized API (NAPI v3 / GlobalGateway KYC verifications). Set as the scope value alongside grant_type=client_credentials when requesting a bearer token from https://auth-api.trulioo.com/connect/token.
  flows: []
  scope: napi.api
- description: Grants access to the Workflow Studio (Platform) API. Set as the scope value with grant_type=client_credentials in the client-credentials token request.
  flows: []
  scope: workflow.studio.api
- description: Authorizes Identity Document Verification (DocV) operations in the US region. Trulioo's DocV scope parameter specifies both the region and the service the token may access.
  flows: []
  scope: docv.api.us
slug: trulioo-scopes
source_filename: trulioo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://developer.trulioo.com/reference/authentication\nsource: openapi/trulioo-business-verification-api-openapi.yml, openapi/trulioo-configuration-api-openapi.yml,\n  openapi/trulioo-connection-api-openapi.yml, openapi/trulioo-document-verification-api-openapi.yml,\n  openapi/trulioo-person-fraud-api-openapi.yml, openapi/trulioo-platform-api-openapi.yml, openapi/trulioo-verifications-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/trulioo-business-verification-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-api.trulioo.com/connect/token\n- name: OAuth2\n  source: openapi/trulioo-configuration-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-api.trulioo.com/connect/token\n- name: OAuth2\n  source: openapi/trulioo-connection-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-api.trulioo.com/connect/token\n- name:\
  \ OAuth2\n  source: openapi/trulioo-document-verification-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-api.trulioo.com/connect/token\n- name: OAuth2\n  source: openapi/trulioo-person-fraud-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-api.trulioo.com/connect/token\n- name: OAuth2\n  source: openapi/trulioo-platform-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.trulioo.com/customer/v2/auth/customer\n- name: OAuth2\n  source: openapi/trulioo-verifications-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-api.trulioo.com/connect/token\n  description: Two-legged client credentials OAuth2 flow.\nscopes:\n- scope: napi.api\n  description: Grants access to the Normalized API (NAPI v3 / GlobalGateway KYC verifications).\n    Set as the scope value alongside grant_type=client_credentials when requesting\n    a bearer token from https://auth-api.trulioo.com/connect/token.\n\
  \  sources:\n  - https://developer.trulioo.com/reference/authentication\n  - https://developer.trulioo.com/reference/authentication-recipe\n- scope: workflow.studio.api\n  description: Grants access to the Workflow Studio (Platform) API. Set as the scope\n    value with grant_type=client_credentials in the client-credentials token request.\n  sources:\n  - https://developer.trulioo.com/reference/authentication-recipe\n- scope: docv.api.us\n  description: Authorizes Identity Document Verification (DocV) operations in the\n    US region. Trulioo's DocV scope parameter specifies both the region and the service\n    the token may access.\n  sources:\n  - https://developer.trulioo.com/reference/authorization-2\nnote: Trulioo uses the OAuth2 client_credentials flow with service- and region-scoped\n  values (for example docv.api.us for DocV in the US region); only the scopes above\n  are documented publicly, and no full scope catalog is published (https://developer.trulioo.com/reference/authorization-2).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/scopes/trulioo-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Identity Verification
- KYC
- KYB
- AML
- Watchlist Screening
- Biometrics
- Document Verification
- Fraud Prevention
- Compliance
- Global Identity
token_urls:
- https://auth-api.trulioo.com/connect/token
- https://api.trulioo.com/customer/v2/auth/customer
---
