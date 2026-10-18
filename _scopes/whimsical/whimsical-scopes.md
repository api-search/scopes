---
api_specs:
- filename: whimsical-comments-list-api-openapi.yml
  format: yaml
  label: Whimsical Comments.list API
  slug: whimsical-comments-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/openapi/whimsical-comments-list-api-openapi.yml
- filename: whimsical-files-get-api-openapi.yml
  format: yaml
  label: Whimsical Files.get API
  slug: whimsical-files-get-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/openapi/whimsical-files-get-api-openapi.yml
- filename: whimsical-files-list-api-openapi.yml
  format: yaml
  label: Whimsical Files.list API
  slug: whimsical-files-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/openapi/whimsical-files-list-api-openapi.yml
- filename: whimsical-teams-list-api-openapi.yml
  format: yaml
  label: Whimsical Teams.list API
  slug: whimsical-teams-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/openapi/whimsical-teams-list-api-openapi.yml
- filename: whimsical-users-get-api-openapi.yml
  format: yaml
  label: Whimsical Users.get API
  slug: whimsical-users-get-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/openapi/whimsical-users-get-api-openapi.yml
authorization_urls:
- https://whimsical.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Whimsical Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Whimsical uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://whimsical.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Whimsical
provider_slug: whimsical
schemes:
- description: OAuth 2.1 authorization (contact Whimsical support for client credentials)
  flows:
  - authorizationUrl: https://whimsical.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://whimsical.com/oauth/token
  name: OAuth2
  source: openapi/whimsical-comments-list-api-openapi.yml
- description: OAuth 2.1 authorization (contact Whimsical support for client credentials)
  flows:
  - authorizationUrl: https://whimsical.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://whimsical.com/oauth/token
  name: OAuth2
  source: openapi/whimsical-files-get-api-openapi.yml
- description: OAuth 2.1 authorization (contact Whimsical support for client credentials)
  flows:
  - authorizationUrl: https://whimsical.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://whimsical.com/oauth/token
  name: OAuth2
  source: openapi/whimsical-files-list-api-openapi.yml
- description: OAuth 2.1 authorization (contact Whimsical support for client credentials)
  flows:
  - authorizationUrl: https://whimsical.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://whimsical.com/oauth/token
  name: OAuth2
  source: openapi/whimsical-teams-list-api-openapi.yml
- description: OAuth 2.1 authorization (contact Whimsical support for client credentials)
  flows:
  - authorizationUrl: https://whimsical.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://whimsical.com/oauth/token
  name: OAuth2
  source: openapi/whimsical-users-get-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: whimsical-scopes
source_filename: whimsical-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/whimsical-comments-list-api-openapi.yml, openapi/whimsical-files-get-api-openapi.yml,\n  openapi/whimsical-files-list-api-openapi.yml, openapi/whimsical-teams-list-api-openapi.yml,\n  openapi/whimsical-users-get-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/whimsical-comments-list-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://whimsical.com/oauth/authorize\n    tokenUrl: https://whimsical.com/oauth/token\n  description: OAuth 2.1 authorization (contact Whimsical support for client credentials)\n- name: OAuth2\n  source: openapi/whimsical-files-get-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://whimsical.com/oauth/authorize\n    tokenUrl: https://whimsical.com/oauth/token\n  description: OAuth 2.1 authorization (contact Whimsical support for client credentials)\n- name: OAuth2\n  source: openapi/whimsical-files-list-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://whimsical.com/oauth/authorize\n    tokenUrl: https://whimsical.com/oauth/token\n  description: OAuth 2.1 authorization (contact Whimsical support for client credentials)\n- name: OAuth2\n  source: openapi/whimsical-teams-list-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://whimsical.com/oauth/authorize\n    tokenUrl: https://whimsical.com/oauth/token\n  description: OAuth 2.1 authorization (contact Whimsical support for client credentials)\n- name: OAuth2\n  source: openapi/whimsical-users-get-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://whimsical.com/oauth/authorize\n    tokenUrl: https://whimsical.com/oauth/token\n  description: OAuth 2.1 authorization (contact Whimsical support for client credentials)\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/scopes/whimsical-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Collaboration
- Diagramming
- Flowcharts
- Wireframes
- Mind Maps
token_bound: false
token_urls:
- https://whimsical.com/oauth/token
---
