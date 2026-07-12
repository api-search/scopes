---
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
