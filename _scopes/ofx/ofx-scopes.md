---
api_specs:
- filename: ofx-authorization-code-api-openapi.yml
  format: yaml
  label: OFX Authorization Code API
  slug: ofx-authorization-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/ofx-authorization-code-api-openapi.yml
- filename: ofx-authorize-api-openapi.yml
  format: yaml
  label: OFX Authorize API
  slug: ofx-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/ofx-authorize-api-openapi.yml
- filename: ofx-business-api-openapi.yml
  format: yaml
  label: OFX Business API
  slug: ofx-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/ofx-business-api-openapi.yml
- filename: ofx-oauth-api-openapi.yml
  format: yaml
  label: OFX OAuth API
  slug: ofx-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/ofx-oauth-api-openapi.yml
- filename: ofx-ofxrates-api-openapi.yml
  format: yaml
  label: OFX Ofxrates API
  slug: ofx-ofxrates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/ofx-ofxrates-api-openapi.yml
- filename: ofx-open-banking-api-openapi.yml
  format: yaml
  label: OFX Open Banking API
  slug: ofx-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/ofx-open-banking-api-openapi.yml
- filename: ofx-refresh-token-api-openapi.yml
  format: yaml
  label: OFX Refresh Token API
  slug: ofx-refresh-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/ofx-refresh-token-api-openapi.yml
- filename: ofx-token-api-openapi.yml
  format: yaml
  label: OFX Token API
  slug: ofx-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/ofx-token-api-openapi.yml
authorization_urls:
- https://sandbox.api.ofx.com/v1/oauth/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Ofx Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OFX publishes 1 OAuth 2.0 scope via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the OFX API on a user''s behalf.


  Tokens are issued from https://sandbox.api.ofx.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OFX
provider_slug: ofx
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token
  - authorizationUrl: https://sandbox.api.ofx.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token
  name: OAuth_2.0
  source: openapi/ofx-aisp-openapi-generated.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token
  - authorizationUrl: https://sandbox.api.ofx.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token
  name: OAuth_2.0
  source: openapi/ofx-ncp-openapi-generated.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token
  - authorizationUrl: https://sandbox.api.ofx.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token
  name: OAuth_2.0
  source: openapi/ofx-pisp-openapi-generated.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token
  - authorizationUrl: https://sandbox.api.ofx.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token
  name: OAuth_2.0
  source: openapi/ofx-rates-openapi-generated.yml
scope_count: 1
scope_names:
- payments
scopes:
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
slug: ofx-scopes
source_filename: ofx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: derived\nsource: openapi/ofx-aisp-openapi-generated.yml, openapi/ofx-ncp-openapi-generated.yml, openapi/ofx-pisp-openapi-generated.yml,\n  openapi/ofx-rates-openapi-generated.yml\nschemes:\n- name: OAuth_2.0\n  source: openapi/ofx-aisp-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.api.ofx.com/v1/oauth/authorize\n    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token\n- name: OAuth_2.0\n  source: openapi/ofx-ncp-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.api.ofx.com/v1/oauth/authorize\n    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token\n- name: OAuth_2.0\n  source: openapi/ofx-pisp-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://sandbox.api.ofx.com/v1/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.api.ofx.com/v1/oauth/authorize\n    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token\n- name: OAuth_2.0\n  source: openapi/ofx-rates-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.api.ofx.com/v1/oauth/authorize\n    tokenUrl: https://sandbox.api.ofx.com/v1/oauth/token\nscopes:\n- scope: payments\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ofx-aisp-openapi-generated.yml\n  - openapi/ofx-ncp-openapi-generated.yml\n  - openapi/ofx-pisp-openapi-generated.yml\n  - openapi/ofx-rates-openapi-generated.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/scopes/ofx-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode
tags:
- Company
- Payments
- Money Transfer
- Fintech
- Banking
token_bound: false
token_urls:
- https://sandbox.api.ofx.com/v1/oauth/token
---
