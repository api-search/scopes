---
api_specs:
- filename: eloqua-rest-openapi.yml
  format: yaml
  label: Eloqua REST API
  slug: eloqua-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/openapi/eloqua-rest-openapi.yml
- filename: eloqua-bulk-openapi.yml
  format: yaml
  label: Eloqua Bulk API
  slug: eloqua-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/openapi/eloqua-bulk-openapi.yml
authorization_urls:
- https://login.eloqua.com/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Eloqua Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Oracle Eloqua publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Oracle Eloqua API on a user''s behalf.


  Tokens are issued from https://login.eloqua.com/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oracle Eloqua
provider_slug: eloqua
schemes:
- description: OAuth 2.0 authorization code flow
  flows:
  - authorizationUrl: https://login.eloqua.com/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.eloqua.com/auth/oauth2/token
  name: oAuth2
  source: openapi/eloqua-bulk-openapi.yml
- description: OAuth 2.0 authorization code flow
  flows:
  - authorizationUrl: https://login.eloqua.com/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.eloqua.com/auth/oauth2/token
  name: oAuth2
  source: openapi/eloqua-rest-openapi.yml
scope_count: 1
scope_names:
- full
scopes:
- description: Full access to all Eloqua resources
  flows:
  - authorizationCode
  scope: full
slug: eloqua-scopes
source_filename: eloqua-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eloqua-bulk-openapi.yml, openapi/eloqua-rest-openapi.yml\nschemes:\n- name: oAuth2\n  source: openapi/eloqua-bulk-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.eloqua.com/auth/oauth2/authorize\n    tokenUrl: https://login.eloqua.com/auth/oauth2/token\n  description: OAuth 2.0 authorization code flow\n- name: oAuth2\n  source: openapi/eloqua-rest-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.eloqua.com/auth/oauth2/authorize\n    tokenUrl: https://login.eloqua.com/auth/oauth2/token\n  description: OAuth 2.0 authorization code flow\nscopes:\n- scope: full\n  description: Full access to all Eloqua resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/eloqua-bulk-openapi.yml\n  - openapi/eloqua-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/scopes/eloqua-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- CRM
- Email Marketing
- Lead Management
- Marketing Automation
token_urls:
- https://login.eloqua.com/auth/oauth2/token
---
