---
api_specs:
- filename: brightspace-assignments-api-openapi.yml
  format: yaml
  label: D2L Brightspace Assignments API
  slug: brightspace-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-assignments-api-openapi.yml
- filename: brightspace-calendar-api-openapi.yml
  format: yaml
  label: D2L Brightspace Calendar API
  slug: brightspace-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-calendar-api-openapi.yml
- filename: brightspace-content-api-openapi.yml
  format: yaml
  label: D2L Brightspace Content API
  slug: brightspace-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-content-api-openapi.yml
- filename: brightspace-data-hub-api-openapi.yml
  format: yaml
  label: D2L Brightspace Data Hub API
  slug: brightspace-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-data-hub-api-openapi.yml
- filename: brightspace-discussions-api-openapi.yml
  format: yaml
  label: D2L Brightspace Discussions API
  slug: brightspace-discussions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-discussions-api-openapi.yml
- filename: brightspace-enrollments-api-openapi.yml
  format: yaml
  label: D2L Brightspace Enrollments API
  slug: brightspace-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-enrollments-api-openapi.yml
- filename: brightspace-grades-api-openapi.yml
  format: yaml
  label: D2L Brightspace Grades API
  slug: brightspace-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-grades-api-openapi.yml
- filename: brightspace-learning-outcomes-api-openapi.yml
  format: yaml
  label: D2L Brightspace Learning Outcomes API
  slug: brightspace-learning-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-learning-outcomes-api-openapi.yml
- filename: brightspace-news-api-openapi.yml
  format: yaml
  label: D2L Brightspace News API
  slug: brightspace-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-news-api-openapi.yml
- filename: brightspace-org-units-api-openapi.yml
  format: yaml
  label: D2L Brightspace Org Units API
  slug: brightspace-org-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-org-units-api-openapi.yml
- filename: brightspace-quizzes-api-openapi.yml
  format: yaml
  label: D2L Brightspace Quizzes API
  slug: brightspace-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-quizzes-api-openapi.yml
- filename: brightspace-users-api-openapi.yml
  format: yaml
  label: D2L Brightspace Users API
  slug: brightspace-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-users-api-openapi.yml
- filename: brightspace-versions-api-openapi.yml
  format: yaml
  label: D2L Brightspace Versions API
  slug: brightspace-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-versions-api-openapi.yml
authorization_urls:
- https://auth.brightspace.com/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Brightspace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'D2L Brightspace publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the D2L Brightspace API on a user''s behalf.


  Tokens are issued from https://auth.brightspace.com/core/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: D2L Brightspace
provider_slug: brightspace
schemes:
- description: OAuth 2 authorization code grant. Tokens are issued by the D2L auth service. Scopes take the form group:resource:action (for example users:userdata:read).
  flows:
  - authorizationUrl: https://auth.brightspace.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://auth.brightspace.com/core/connect/token
  name: oauth2
  source: openapi/brightspace-openapi.yml
scope_count: 4
scope_names:
- core:*:*
- datahub:dataexports:read
- enrollment:orgunit:read
- users:userdata:read
scopes:
- description: Full access consistent with the registered application
  flows:
  - authorizationCode
  scope: core:*:*
- description: Read Data Hub exports
  flows:
  - authorizationCode
  scope: datahub:dataexports:read
- description: Read enrollments
  flows:
  - authorizationCode
  scope: enrollment:orgunit:read
- description: Read user data
  flows:
  - authorizationCode
  scope: users:userdata:read
slug: brightspace-scopes
source_filename: brightspace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brightspace-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/brightspace-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.brightspace.com/oauth2/auth\n    tokenUrl: https://auth.brightspace.com/core/connect/token\n  description: OAuth 2 authorization code grant. Tokens are issued by the D2L auth service.\n    Scopes take the form group:resource:action (for example users:userdata:read).\nscopes:\n- scope: core:*:*\n  description: Full access consistent with the registered application\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/brightspace-openapi.yml\n- scope: datahub:dataexports:read\n  description: Read Data Hub exports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/brightspace-openapi.yml\n- scope: enrollment:orgunit:read\n  description: Read enrollments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/brightspace-openapi.yml\n- scope:\
  \ users:userdata:read\n  description: Read user data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/brightspace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/scopes/brightspace-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- LMS
- Learning Management System
- EdTech
- Education
- Valence
- D2L
- Brightspace
token_urls:
- https://auth.brightspace.com/core/connect/token
---
