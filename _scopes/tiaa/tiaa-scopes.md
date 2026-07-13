---
api_specs:
- filename: tiaa-fdx-openapi.yml
  format: yaml
  label: TIAA Financial Data Exchange API
  slug: tiaa-fdx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-fdx-openapi.yml
- filename: tiaa-sia-openapi.yml
  format: yaml
  label: TIAA Secure Income Account API
  slug: tiaa-sia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-sia-openapi.yml
authorization_urls:
- https://auth.tiaa.org/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Tiaa Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TIAA publishes 8 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the TIAA API on a user''s behalf.


  Tokens are issued from https://auth.tiaa.org/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TIAA
provider_slug: tiaa
schemes:
- flows:
  - authorizationUrl: https://auth.tiaa.org/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tiaa.org/oauth2/token
  name: OAuth2
  source: openapi/tiaa-fdx-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tiaa.org/oauth2/token
  name: ClientCredentials
  source: openapi/tiaa-sia-openapi.yml
scope_count: 8
scope_names:
- accounts
- investments
- openid
- profile
- sia:read
- sia:write
- tax
- transactions
scopes:
- description: Account data access
  flows:
  - authorizationCode
  scope: accounts
- description: Investment data access
  flows:
  - authorizationCode
  scope: investments
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: Customer profile
  flows:
  - authorizationCode
  scope: profile
- description: Read SIA data
  flows:
  - clientCredentials
  scope: sia:read
- description: Write SIA data
  flows:
  - clientCredentials
  scope: sia:write
- description: Tax document access
  flows:
  - authorizationCode
  scope: tax
- description: Transaction data access
  flows:
  - authorizationCode
  scope: transactions
slug: tiaa-scopes
source_filename: tiaa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tiaa-fdx-openapi.yml, openapi/tiaa-sia-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/tiaa-fdx-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tiaa.org/oauth2/authorize\n    tokenUrl: https://auth.tiaa.org/oauth2/token\n- name: ClientCredentials\n  source: openapi/tiaa-sia-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tiaa.org/oauth2/token\nscopes:\n- scope: accounts\n  description: Account data access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tiaa-fdx-openapi.yml\n- scope: investments\n  description: Investment data access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tiaa-fdx-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tiaa-fdx-openapi.yml\n- scope: profile\n  description: Customer profile\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/tiaa-fdx-openapi.yml\n- scope: sia:read\n  description: Read SIA data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/tiaa-sia-openapi.yml\n- scope: sia:write\n  description: Write SIA data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/tiaa-sia-openapi.yml\n- scope: tax\n  description: Tax document access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tiaa-fdx-openapi.yml\n- scope: transactions\n  description: Transaction data access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tiaa-fdx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/scopes/tiaa-scopes.yml
summary_line: 8 scopes · authorizationCode/clientCredentials
tags:
- Finance
- Financial Data
- Fintech
- Insurance
- Investment Management
- Retirement
- Wealth Management
- Fortune 100
token_urls:
- https://auth.tiaa.org/oauth2/token
---
