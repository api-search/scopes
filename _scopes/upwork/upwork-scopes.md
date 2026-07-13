---
api_specs:
- filename: upwork-graphql-api-openapi.yml
  format: yaml
  label: Upwork GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-graphql-api-openapi.yml
- filename: upwork-rest-api-openapi.yml
  format: yaml
  label: Upwork REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-rest-api-openapi.yml
authorization_urls:
- https://www.upwork.com/ab/account-security/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Upwork Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Upwork publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Upwork API on a user''s behalf.


  Tokens are issued from https://www.upwork.com/api/v3/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Upwork
provider_slug: upwork
schemes:
- description: OAuth 2.0 authorization code flow for Upwork API access. Obtain an authorization code by redirecting users to the Upwork OAuth consent page, then exchange for access and refresh tokens.
  flows:
  - authorizationUrl: https://www.upwork.com/ab/account-security/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.upwork.com/api/v3/oauth2/token
  name: oauth2AuthCode
  source: openapi/upwork-graphql-api-openapi.yml
- description: OAuth 2.0 authorization code flow
  flows:
  - authorizationUrl: https://www.upwork.com/ab/account-security/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.upwork.com/api/v3/oauth2/token
  name: oauth2AuthCode
  source: openapi/upwork-rest-api-openapi.yml
scope_count: 9
scope_names:
- contracts:read
- email
- jobs:read
- messages:read
- messages:write
- openid
- profile
- profiles:read
- reports:read
scopes:
- description: Read contract data
  flows:
  - authorizationCode
  scope: contracts:read
- description: Access to user email
  flows:
  - authorizationCode
  scope: email
- description: Read job postings
  flows:
  - authorizationCode
  scope: jobs:read
- description: Read messages
  flows:
  - authorizationCode
  scope: messages:read
- description: Send messages
  flows:
  - authorizationCode
  scope: messages:write
- description: Access to user identity information
  flows:
  - authorizationCode
  scope: openid
- description: Access to user profile data
  flows:
  - authorizationCode
  scope: profile
- description: Read freelancer profiles
  flows:
  - authorizationCode
  scope: profiles:read
- description: Read financial reports
  flows:
  - authorizationCode
  scope: reports:read
slug: upwork-scopes
source_filename: upwork-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/upwork-graphql-api-openapi.yml, openapi/upwork-rest-api-openapi.yml\nschemes:\n- name: oauth2AuthCode\n  source: openapi/upwork-graphql-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.upwork.com/ab/account-security/oauth2/authorize\n    tokenUrl: https://www.upwork.com/api/v3/oauth2/token\n  description: OAuth 2.0 authorization code flow for Upwork API access. Obtain an authorization\n    code by redirecting users to the Upwork OAuth consent page, then exchange for access and\n    refresh tokens.\n- name: oauth2AuthCode\n  source: openapi/upwork-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.upwork.com/ab/account-security/oauth2/authorize\n    tokenUrl: https://www.upwork.com/api/v3/oauth2/token\n  description: OAuth 2.0 authorization code flow\nscopes:\n- scope: contracts:read\n  description: Read contract data\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n  - openapi/upwork-rest-api-openapi.yml\n- scope: email\n  description: Access to user email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n- scope: jobs:read\n  description: Read job postings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n- scope: messages:read\n  description: Read messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n- scope: messages:write\n  description: Send messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n- scope: openid\n  description: Access to user identity information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n  - openapi/upwork-rest-api-openapi.yml\n- scope: profile\n  description: Access to user profile data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n\
  - scope: profiles:read\n  description: Read freelancer profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n- scope: reports:read\n  description: Read financial reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n  - openapi/upwork-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/scopes/upwork-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Freelancing
- Jobs
- Talent
- Marketplace
- Contracts
- Hiring
token_urls:
- https://www.upwork.com/api/v3/oauth2/token
---
