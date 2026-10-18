---
api_specs:
- filename: schoology-assignments-api-openapi.yml
  format: yaml
  label: Schoology Assignments API
  slug: schoology-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-assignments-api-openapi.yml
- filename: schoology-courses-api-openapi.yml
  format: yaml
  label: Schoology Courses API
  slug: schoology-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-courses-api-openapi.yml
- filename: schoology-enrollments-api-openapi.yml
  format: yaml
  label: Schoology Enrollments API
  slug: schoology-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-enrollments-api-openapi.yml
- filename: schoology-grades-api-openapi.yml
  format: yaml
  label: Schoology Grades API
  slug: schoology-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-grades-api-openapi.yml
- filename: schoology-groups-api-openapi.yml
  format: yaml
  label: Schoology Groups API
  slug: schoology-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-groups-api-openapi.yml
- filename: schoology-multi-call-api-openapi.yml
  format: yaml
  label: Schoology Multi-Call API
  slug: schoology-multi-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-multi-call-api-openapi.yml
- filename: schoology-sections-api-openapi.yml
  format: yaml
  label: Schoology Sections API
  slug: schoology-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-sections-api-openapi.yml
- filename: schoology-submissions-api-openapi.yml
  format: yaml
  label: Schoology Submissions API
  slug: schoology-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-submissions-api-openapi.yml
- filename: schoology-subscriptions-api-openapi.yml
  format: yaml
  label: Schoology Subscriptions API
  slug: schoology-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-subscriptions-api-openapi.yml
- filename: schoology-targets-api-openapi.yml
  format: yaml
  label: Schoology Targets API
  slug: schoology-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-targets-api-openapi.yml
- filename: schoology-users-api-openapi.yml
  format: yaml
  label: Schoology Users API
  slug: schoology-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-users-api-openapi.yml
- filename: schoology-events-api-openapi.yml
  format: yaml
  label: Schoology Events API
  slug: schoology-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-events-api-openapi.yml
authorization_urls:
- https://api.schoology.com/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Schoology Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
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
  source: openapi/schoology-assignments-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-courses-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-enrollments-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-events-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-grades-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-groups-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-multi-call-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-sections-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-submissions-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-subscriptions-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-targets-api-openapi.yml
- description: OAuth 1.0a / 2.0 per Schoology Authentication docs.
  flows:
  - authorizationUrl: https://api.schoology.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schoology.com/v1/oauth/access_token
  name: OAuth
  source: openapi/schoology-users-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: schoology-scopes
source_filename: schoology-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/schoology-assignments-api-openapi.yml, openapi/schoology-courses-api-openapi.yml,\n  openapi/schoology-enrollments-api-openapi.yml, openapi/schoology-events-api-openapi.yml, openapi/schoology-grades-api-openapi.yml,\n  openapi/schoology-groups-api-openapi.yml, openapi/schoology-multi-call-api-openapi.yml, openapi/schoology-sections-api-openapi.yml,\n  openapi/schoology-submissions-api-openapi.yml, openapi/schoology-subscriptions-api-openapi.yml,\n  openapi/schoology-targets-api-openapi.yml, openapi/schoology-users-api-openapi.yml\nschemes:\n- name: OAuth\n  source: openapi/schoology-assignments-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-courses-api-openapi.yml\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-enrollments-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-events-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-grades-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n\
  \    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-groups-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-multi-call-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-sections-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description:\
  \ OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-submissions-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-subscriptions-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n  source: openapi/schoology-targets-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\n- name: OAuth\n \
  \ source: openapi/schoology-users-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schoology.com/v1/oauth/authorize\n    tokenUrl: https://api.schoology.com/v1/oauth/access_token\n  description: OAuth 1.0a / 2.0 per Schoology Authentication docs.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/scopes/schoology-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- EdTech
- LMS
- K-12
token_bound: false
token_urls:
- https://api.schoology.com/v1/oauth/access_token
---
