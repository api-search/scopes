---
api_specs:
- filename: iproov-enrol-api-openapi.yml
  format: yaml
  label: iProov Enrol API
  slug: iproov-enrol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-enrol-api-openapi.yml
- filename: iproov-management-api-openapi.yml
  format: yaml
  label: iProov Management API
  slug: iproov-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-management-api-openapi.yml
- filename: iproov-user-api-openapi.yml
  format: yaml
  label: iProov User API
  slug: iproov-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-user-api-openapi.yml
- filename: iproov-verify-api-openapi.yml
  format: yaml
  label: iProov Verify API
  slug: iproov-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-verify-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Iproov Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'iProov publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the iProov API on a user''s behalf.


  Tokens are issued from /{api_key}/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: iProov
provider_slug: iproov
schemes:
- description: OAuth2 is used for the Management and User APIs.
  flows:
  - flow: clientCredentials
    tokenUrl: /{api_key}/access_token
  name: oauth2
  source: openapi/iproov-openapi.yml
scope_count: 2
scope_names:
- user-read
- user-write
scopes:
- description: Read the information of users
  flows:
  - clientCredentials
  scope: user-read
- description: Update the user object
  flows:
  - clientCredentials
  scope: user-write
slug: iproov-scopes
source_filename: iproov-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/iproov-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/iproov-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /{api_key}/access_token\n  description: OAuth2 is used for the Management and User APIs.\nscopes:\n- scope: user-read\n  description: Read the information of users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/iproov-openapi.yml\n- scope: user-write\n  description: Update the user object\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/iproov-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/iproov/scopes/iproov-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Biometrics
- Identity Verification
- Authentication
- Liveness Detection
- Face Verification
- Fraud Prevention
- Deepfake Detection
token_bound: false
token_urls:
- /{api_key}/access_token
---
