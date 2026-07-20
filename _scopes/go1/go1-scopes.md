---
api_specs:
- filename: go1-openapi.yml
  format: yaml
  label: Go1 API
  slug: go1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-openapi.yml
authorization_urls:
- https://auth.go1.com/oauth/authorize
description: ''
docs: https://developers.go1.com/docs/developer-tools/auth/overview-auth
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Go1 Scopes
name_suffix: OAuth Scopes
note: Scopes recovered from the per-operation security requirements published in Go1's REST reference (developers.go1.com). Go1 does not publish a standalone scope-reference page; descriptions are derived from the resource each scope governs.
overview: 'Go1 publishes 8 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Go1 API on a user''s behalf.


  Tokens are issued from https://auth.go1.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Go1
provider_slug: go1
schemes:
- description: OAuth 2.0. Server-to-server integrations use the client_credentials flow; user-context integrations use the authorization_code flow. Access tokens are valid for 12 hours.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.go1.com/oauth/token
  - authorizationUrl: https://auth.go1.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.go1.com/oauth/token
  name: OAuth2
  source: openapi/go1-openapi.yml
scope_count: 8
scope_names:
- enrollment.read
- enrollment.write
- lo.read
- lo.write
- portal.read
- portal.write
- webhook.read
- webhook.write
scopes:
- description: Read enrollments and completion records.
  flows:
  - authorizationCode
  - clientCredentials
  scope: enrollment.read
- description: Create, update and delete enrollments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: enrollment.write
- description: Read learning objects (content catalog).
  flows:
  - authorizationCode
  - clientCredentials
  scope: lo.read
- description: Create, update and delete learning objects.
  flows:
  - authorizationCode
  - clientCredentials
  scope: lo.write
- description: Read customer portals.
  flows:
  - authorizationCode
  - clientCredentials
  scope: portal.read
- description: Create and update customer portals.
  flows:
  - authorizationCode
  - clientCredentials
  scope: portal.write
- description: Read webhook configurations.
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhook.read
- description: Create, update and delete webhook configurations.
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhook.write
slug: go1-scopes
source_filename: go1-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/go1-openapi.yml\ndocs: https://developers.go1.com/docs/developer-tools/auth/overview-auth\nnote: >-\n  Scopes recovered from the per-operation security requirements published in Go1's REST reference\n  (developers.go1.com). Go1 does not publish a standalone scope-reference page; descriptions are\n  derived from the resource each scope governs.\nschemes:\n- name: OAuth2\n  source: openapi/go1-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.go1.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.go1.com/oauth/authorize\n    tokenUrl: https://auth.go1.com/oauth/token\n  description: OAuth 2.0. Server-to-server integrations use the client_credentials flow; user-context\n    integrations use the authorization_code flow. Access tokens are valid for 12 hours.\nscopes:\n- scope: enrollment.read\n  description: Read enrollments and completion records.\n  flows:\n  -\
  \ authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: enrollment.write\n  description: Create, update and delete enrollments.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: lo.read\n  description: Read learning objects (content catalog).\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: lo.write\n  description: Create, update and delete learning objects.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: portal.read\n  description: Read customer portals.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: portal.write\n  description: Create and update customer portals.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: webhook.read\n  description: Read webhook configurations.\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: webhook.write\n  description: Create, update and delete webhook configurations.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/scopes/go1-scopes.yml
summary_line: 8 scopes · clientCredentials/authorizationCode
tags:
- Company
- Edtech
- Learning
- E-Learning
- Corporate Training
- Content
- Learning Management
- LMS
- Education
- Webhooks
token_urls:
- https://auth.go1.com/oauth/token
---
