---
authorization_urls:
- https://canvas.instructure.com/login/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Canvas Lms Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Canvas LMS publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Canvas LMS API on a user''s behalf.


  Tokens are issued from https://canvas.instructure.com/login/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Canvas LMS
provider_slug: canvas-lms
schemes:
- description: Canvas OAuth2 (RFC 6749) authorization code grant. Register a Developer Key in the target Canvas account to obtain a client_id and client_secret.
  flows:
  - authorizationUrl: https://canvas.instructure.com/login/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://canvas.instructure.com/login/oauth2/token
  name: OAuth2
  source: openapi/canvas-lms-rest-api-openapi.yml
scope_count: 3
scope_names:
- url:GET|/api/v1/accounts
- url:GET|/api/v1/courses
- url:GET|/api/v1/users/{user_id}
scopes:
- description: Read accounts
  flows:
  - authorizationCode
  scope: url:GET|/api/v1/accounts
- description: Read courses
  flows:
  - authorizationCode
  scope: url:GET|/api/v1/courses
- description: Read a user
  flows:
  - authorizationCode
  scope: url:GET|/api/v1/users/{user_id}
slug: canvas-lms-scopes
source_filename: canvas-lms-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canvas-lms-rest-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/canvas-lms-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://canvas.instructure.com/login/oauth2/auth\n    tokenUrl: https://canvas.instructure.com/login/oauth2/token\n  description: Canvas OAuth2 (RFC 6749) authorization code grant. Register a Developer Key in\n    the target Canvas account to obtain a client_id and client_secret.\nscopes:\n- scope: url:GET|/api/v1/accounts\n  description: Read accounts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canvas-lms-rest-api-openapi.yml\n- scope: url:GET|/api/v1/courses\n  description: Read courses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canvas-lms-rest-api-openapi.yml\n- scope: url:GET|/api/v1/users/{user_id}\n  description: Read a user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canvas-lms-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/scopes/canvas-lms-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Learning Management
- Education
- EdTech
- LMS
- LTI
- Higher Education
- K-12
- Open Source
- AGPL
- Canvas
token_urls:
- https://canvas.instructure.com/login/oauth2/token
---
