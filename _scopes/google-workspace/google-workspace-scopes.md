---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Workspace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Workspace publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Workspace API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Workspace
provider_slug: google-workspace
schemes:
- description: OAuth 2.0 authorization for Google Workspace Admin operations.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/admin-sdk-directory-api.yml
scope_count: 6
scope_names:
- https://www.googleapis.com/auth/admin.directory.group
- https://www.googleapis.com/auth/admin.directory.group.readonly
- https://www.googleapis.com/auth/admin.directory.orgunit
- https://www.googleapis.com/auth/admin.directory.orgunit.readonly
- https://www.googleapis.com/auth/admin.directory.user
- https://www.googleapis.com/auth/admin.directory.user.readonly
scopes:
- description: View and manage the provisioning of groups on your domain
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admin.directory.group
- description: View groups on your domain
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admin.directory.group.readonly
- description: View and manage organization units on your domain
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admin.directory.orgunit
- description: View organization units on your domain
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admin.directory.orgunit.readonly
- description: View and manage the provisioning of users on your domain
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admin.directory.user
- description: View users on your domain
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admin.directory.user.readonly
slug: google-workspace-scopes
source_filename: google-workspace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/admin-sdk-directory-api.yml\nschemes:\n- name: oauth2\n  source: openapi/admin-sdk-directory-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authorization for Google Workspace Admin operations.\nscopes:\n- scope: https://www.googleapis.com/auth/admin.directory.group\n  description: View and manage the provisioning of groups on your domain\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/admin-sdk-directory-api.yml\n- scope: https://www.googleapis.com/auth/admin.directory.group.readonly\n  description: View groups on your domain\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/admin-sdk-directory-api.yml\n- scope: https://www.googleapis.com/auth/admin.directory.orgunit\n  description: View and manage organization units on your domain\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/admin-sdk-directory-api.yml\n- scope: https://www.googleapis.com/auth/admin.directory.orgunit.readonly\n  description: View organization units on your domain\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/admin-sdk-directory-api.yml\n- scope: https://www.googleapis.com/auth/admin.directory.user\n  description: View and manage the provisioning of users on your domain\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/admin-sdk-directory-api.yml\n- scope: https://www.googleapis.com/auth/admin.directory.user.readonly\n  description: View users on your domain\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/admin-sdk-directory-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/scopes/google-workspace-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Calendar
- Collaboration
- Email
- Productivity
- Storage
- Video Conferencing
token_urls:
- https://oauth2.googleapis.com/token
---
