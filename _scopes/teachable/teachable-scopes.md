---
api_specs:
- filename: teachable-admin-openapi.yml
  format: yaml
  label: Teachable Admin API
  slug: teachable-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-admin-openapi.yml
- filename: teachable-oauth-openapi.yml
  format: yaml
  label: Teachable OAuth API
  slug: teachable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-oauth-openapi.yml
authorization_urls:
- https://developers.teachable.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Teachable Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Teachable publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Teachable API on a user''s behalf.


  Tokens are issued from https://developers.teachable.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Teachable
provider_slug: teachable
schemes:
- flows:
  - authorizationUrl: https://developers.teachable.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://developers.teachable.com/oauth/token
  name: OAuth2
  source: openapi/teachable-oauth-openapi.yml
scope_count: 4
scope_names:
- courses:read
- courses:update
- email:read
- name:read
scopes:
- description: Read courses and course content
  flows:
  - authorizationCode
  scope: courses:read
- description: Update course progress
  flows:
  - authorizationCode
  scope: courses:update
- description: Read the current user's email address
  flows:
  - authorizationCode
  scope: email:read
- description: Read the current user's name
  flows:
  - authorizationCode
  scope: name:read
slug: teachable-scopes
source_filename: teachable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teachable-oauth-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/teachable-oauth-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developers.teachable.com/oauth/authorize\n    tokenUrl: https://developers.teachable.com/oauth/token\nscopes:\n- scope: courses:read\n  description: Read courses and course content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/teachable-oauth-openapi.yml\n- scope: courses:update\n  description: Update course progress\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/teachable-oauth-openapi.yml\n- scope: email:read\n  description: Read the current user's email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/teachable-oauth-openapi.yml\n- scope: name:read\n  description: Read the current user's name\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/teachable-oauth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/scopes/teachable-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Online Courses
- E-Learning
- Education
- Course Management
- Enrollments
- Coaching
- Memberships
- Transactions
token_urls:
- https://developers.teachable.com/oauth/token
---
