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
