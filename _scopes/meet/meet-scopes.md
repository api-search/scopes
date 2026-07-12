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
name: Meet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Meet publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Meet API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Meet
provider_slug: meet
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/meet-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/meetings.space.created
- https://www.googleapis.com/auth/meetings.space.readonly
- https://www.googleapis.com/auth/meetings.space.settings
scopes:
- description: Create and manage meeting spaces created by the app
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/meetings.space.created
- description: Read meeting spaces
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/meetings.space.readonly
- description: Manage meeting space settings
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/meetings.space.settings
slug: meet-scopes
source_filename: meet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meet-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/meet-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/meetings.space.created\n  description: Create and manage meeting spaces created by the app\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meet-openapi.yml\n- scope: https://www.googleapis.com/auth/meetings.space.readonly\n  description: Read meeting spaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meet-openapi.yml\n- scope: https://www.googleapis.com/auth/meetings.space.settings\n  description: Manage meeting space settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meet/refs/heads/main/scopes/meet-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Video Conferencing
- Meetings
- Communication
- Collaboration
- Google Workspace
- Recordings
- Transcripts
token_urls:
- https://oauth2.googleapis.com/token
---
