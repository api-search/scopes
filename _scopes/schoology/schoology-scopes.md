---
authorization_urls:
- https://api.schoology.com/v1/oauth/authorize
description: ''
docs: https://developers.schoology.com/api-documentation/authentication/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Schoology Scopes
name_suffix: OAuth Scopes
note: Schoology's API uses OAuth 1.0 (two-legged and three-legged) which does not implement scopes; access is governed by role-based permissions (the "Access Schoology API" role permission) rather than OAuth scopes, per https://developers.schoology.com/api-documentation/authentication/.
overview: 'Schoology uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.schoology.com/v1/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Schoology
provider_slug: schoology
schemes:
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-webhooks-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: schoology-scopes
source_filename: schoology-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/schoology-openapi.yml, openapi/schoology-webhooks-openapi.yml\ndocs: https://developers.schoology.com/api-documentation/authentication/\nnote: Schoology's API uses OAuth 1.0 (two-legged and three-legged) which does not implement\n  scopes; access is governed by role-based permissions (the \"Access Schoology API\" role\n  permission) rather than OAuth scopes, per https://developers.schoology.com/api-documentation/authentication/.\nschemes:\n- name: OAuth\n  source: openapi/schoology-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-webhooks-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n\
  \  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/scopes/schoology-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- EdTech
- LMS
- K-12
token_urls:
- https://api.schoology.com/v1/oauth/access_token
---
