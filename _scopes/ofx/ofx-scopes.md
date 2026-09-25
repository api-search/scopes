---
api_specs:
- filename: ofx-aisp-openapi-generated.yml
  format: yaml
  label: OFX AISP API
  slug: aisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-aisp-openapi-generated.yml
- filename: ofx-ncp-openapi-generated.yml
  format: yaml
  label: OFX NCP API
  slug: ncp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-ncp-openapi-generated.yml
- filename: ofx-pisp-openapi-generated.yml
  format: yaml
  label: OFX PISP API
  slug: pisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-pisp-openapi-generated.yml
- filename: ofx-rates-openapi-generated.yml
  format: yaml
  label: OFX Rates API
  slug: rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-rates-openapi-generated.yml
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
token_urls:
- https://sandbox.api.ofx.com/v1/oauth/token
---
