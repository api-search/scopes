---
api_specs:
- filename: xiaomi-access-control-api-openapi.yml
  format: yaml
  label: Xiaomi Access Control API
  slug: xiaomi-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-access-control-api-openapi.yml
- filename: xiaomi-authentication-api-openapi.yml
  format: yaml
  label: Xiaomi Authentication API
  slug: xiaomi-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-authentication-api-openapi.yml
- filename: xiaomi-cdn-api-openapi.yml
  format: yaml
  label: Xiaomi CDN API
  slug: xiaomi-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-cdn-api-openapi.yml
- filename: xiaomi-chat-api-openapi.yml
  format: yaml
  label: Xiaomi Chat API
  slug: xiaomi-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-chat-api-openapi.yml
- filename: xiaomi-models-api-openapi.yml
  format: yaml
  label: Xiaomi Models API
  slug: xiaomi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-models-api-openapi.yml
- filename: xiaomi-multipart-upload-api-openapi.yml
  format: yaml
  label: Xiaomi Multipart Upload API
  slug: xiaomi-multipart-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-multipart-upload-api-openapi.yml
- filename: xiaomi-objects-api-openapi.yml
  format: yaml
  label: Xiaomi Objects API
  slug: xiaomi-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-objects-api-openapi.yml
- filename: xiaomi-user-api-openapi.yml
  format: yaml
  label: Xiaomi User API
  slug: xiaomi-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/openapi/xiaomi-user-api-openapi.yml
authorization_urls:
- https://account.xiaomi.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Xiaomi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Xiaomi publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xiaomi API on a user''s behalf.


  Tokens are issued from https://account.xiaomi.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xiaomi
provider_slug: xiaomi
schemes:
- flows:
  - authorizationUrl: https://account.xiaomi.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://account.xiaomi.com/oauth2/token
  name: oauth2
  source: openapi/xiaomi-open-api-openapi.yml
scope_count: 5
scope_names:
- '1'
- '2'
- '3'
- '4'
- '6'
scopes:
- description: Access user profile (nickname, ID, avatar)
  flows:
  - authorizationCode
  scope: '1'
- description: Access user friend list (MiChat)
  flows:
  - authorizationCode
  scope: '2'
- description: Access user OpenID
  flows:
  - authorizationCode
  scope: '3'
- description: Access user phone number
  flows:
  - authorizationCode
  scope: '4'
- description: Access user email address
  flows:
  - authorizationCode
  scope: '6'
slug: xiaomi-scopes
source_filename: xiaomi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xiaomi-open-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/xiaomi-open-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.xiaomi.com/oauth2/authorize\n    tokenUrl: https://account.xiaomi.com/oauth2/token\nscopes:\n- scope: '1'\n  description: Access user profile (nickname, ID, avatar)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xiaomi-open-api-openapi.yml\n- scope: '2'\n  description: Access user friend list (MiChat)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xiaomi-open-api-openapi.yml\n- scope: '3'\n  description: Access user OpenID\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xiaomi-open-api-openapi.yml\n- scope: '4'\n  description: Access user phone number\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xiaomi-open-api-openapi.yml\n- scope: '6'\n  description: Access user email address\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/xiaomi-open-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaomi/refs/heads/main/scopes/xiaomi-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Consumer Electronics
- IoT
- Smart Home
- Mobile
- Artificial Intelligence
- Cloud Storage
- Machine-Learning
token_urls:
- https://account.xiaomi.com/oauth2/token
---
