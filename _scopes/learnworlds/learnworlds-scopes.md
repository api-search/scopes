---
api_specs:
- filename: learnworlds-courses-api-openapi.yml
  format: yaml
  label: LearnWorlds Courses API
  slug: learnworlds-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-courses-api-openapi.yml
- filename: learnworlds-enrollments-api-openapi.yml
  format: yaml
  label: LearnWorlds Enrollments API
  slug: learnworlds-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-enrollments-api-openapi.yml
- filename: learnworlds-payments-api-openapi.yml
  format: yaml
  label: LearnWorlds Payments API
  slug: learnworlds-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-payments-api-openapi.yml
- filename: learnworlds-progress-api-openapi.yml
  format: yaml
  label: LearnWorlds Progress API
  slug: learnworlds-progress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-progress-api-openapi.yml
- filename: learnworlds-tags-api-openapi.yml
  format: yaml
  label: LearnWorlds Tags API
  slug: learnworlds-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-tags-api-openapi.yml
- filename: learnworlds-users-api-openapi.yml
  format: yaml
  label: LearnWorlds Users API
  slug: learnworlds-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-users-api-openapi.yml
- filename: learnworlds-webhooks-api-openapi.yml
  format: yaml
  label: LearnWorlds Webhooks API
  slug: learnworlds-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Learnworlds Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'LearnWorlds uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://yourschool.learnworlds.com/admin/api/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LearnWorlds
provider_slug: learnworlds
schemes:
- description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for a bearer access token at the school token endpoint, then pass it as Authorization: Bearer ACCESS_TOKEN.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token
  name: oauth2ClientCredentials
  source: openapi/learnworlds-courses-api-openapi.yml
- description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for a bearer access token at the school token endpoint, then pass it as Authorization: Bearer ACCESS_TOKEN.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token
  name: oauth2ClientCredentials
  source: openapi/learnworlds-enrollments-api-openapi.yml
- description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for a bearer access token at the school token endpoint, then pass it as Authorization: Bearer ACCESS_TOKEN.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token
  name: oauth2ClientCredentials
  source: openapi/learnworlds-payments-api-openapi.yml
- description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for a bearer access token at the school token endpoint, then pass it as Authorization: Bearer ACCESS_TOKEN.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token
  name: oauth2ClientCredentials
  source: openapi/learnworlds-progress-api-openapi.yml
- description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for a bearer access token at the school token endpoint, then pass it as Authorization: Bearer ACCESS_TOKEN.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token
  name: oauth2ClientCredentials
  source: openapi/learnworlds-tags-api-openapi.yml
- description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for a bearer access token at the school token endpoint, then pass it as Authorization: Bearer ACCESS_TOKEN.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token
  name: oauth2ClientCredentials
  source: openapi/learnworlds-users-api-openapi.yml
- description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for a bearer access token at the school token endpoint, then pass it as Authorization: Bearer ACCESS_TOKEN.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token
  name: oauth2ClientCredentials
  source: openapi/learnworlds-webhooks-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: learnworlds-scopes
source_filename: learnworlds-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/learnworlds-courses-api-openapi.yml, openapi/learnworlds-enrollments-api-openapi.yml,\n  openapi/learnworlds-payments-api-openapi.yml, openapi/learnworlds-progress-api-openapi.yml,\n  openapi/learnworlds-tags-api-openapi.yml, openapi/learnworlds-users-api-openapi.yml, openapi/learnworlds-webhooks-api-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/learnworlds-courses-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token\n  description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for\n    a bearer access token at the school token endpoint, then pass it as Authorization: Bearer\n    ACCESS_TOKEN.'\n- name: oauth2ClientCredentials\n  source: openapi/learnworlds-enrollments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token\n\
  \  description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for\n    a bearer access token at the school token endpoint, then pass it as Authorization: Bearer\n    ACCESS_TOKEN.'\n- name: oauth2ClientCredentials\n  source: openapi/learnworlds-payments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token\n  description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for\n    a bearer access token at the school token endpoint, then pass it as Authorization: Bearer\n    ACCESS_TOKEN.'\n- name: oauth2ClientCredentials\n  source: openapi/learnworlds-progress-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token\n  description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for\n    a bearer access token at the school token endpoint, then pass it\
  \ as Authorization: Bearer\n    ACCESS_TOKEN.'\n- name: oauth2ClientCredentials\n  source: openapi/learnworlds-tags-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token\n  description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for\n    a bearer access token at the school token endpoint, then pass it as Authorization: Bearer\n    ACCESS_TOKEN.'\n- name: oauth2ClientCredentials\n  source: openapi/learnworlds-users-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token\n  description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for\n    a bearer access token at the school token endpoint, then pass it as Authorization: Bearer\n    ACCESS_TOKEN.'\n- name: oauth2ClientCredentials\n  source: openapi/learnworlds-webhooks-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token\n  description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for\n    a bearer access token at the school token endpoint, then pass it as Authorization: Bearer\n    ACCESS_TOKEN.'\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/scopes/learnworlds-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Online Courses
- LMS
- E-Learning
- Education
- Course Platform
- Creator Economy
token_bound: false
token_urls:
- https://yourschool.learnworlds.com/admin/api/oauth2/access_token
---
