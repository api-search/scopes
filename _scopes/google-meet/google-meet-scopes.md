---
api_specs:
- filename: google-meet-spaces-api-openapi.yml
  format: yaml
  label: Google Meet Spaces API
  slug: google-meet-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-meet/openapi/google-meet-spaces-api-openapi.yml
- filename: google-meet-conferencerecords-api-openapi.yml
  format: yaml
  label: Google Meet Conference Records API
  slug: google-meet-conferencerecords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-meet/openapi/google-meet-conferencerecords-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Meet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Meet publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Meet API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Meet
provider_slug: google-meet
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-meet-conference-records-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-meet-spaces-api-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/meetings.space.created
- https://www.googleapis.com/auth/meetings.space.readonly
- https://www.googleapis.com/auth/meetings.space.settings
scopes:
- description: Create, edit, and see information about your Google Meet conferences created by the app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/meetings.space.created
- description: Read information about any of your Google Meet conferences
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/meetings.space.readonly
- description: Edit, and see settings for all of your Google Meet calls.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/meetings.space.settings
slug: google-meet-scopes
source_filename: google-meet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-meet-conference-records-api-openapi.yml, openapi/google-meet-spaces-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-meet-conference-records-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-meet-spaces-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/meetings.space.created\n  description: Create, edit, and see information about your Google Meet conferences created\n    by the app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-meet-conference-records-api-openapi.yml\n  - openapi/google-meet-spaces-api-openapi.yml\n- scope: https://www.googleapis.com/auth/meetings.space.readonly\n\
  \  description: Read information about any of your Google Meet conferences\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-meet-conference-records-api-openapi.yml\n  - openapi/google-meet-spaces-api-openapi.yml\n- scope: https://www.googleapis.com/auth/meetings.space.settings\n  description: Edit, and see settings for all of your Google Meet calls.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-meet-conference-records-api-openapi.yml\n  - openapi/google-meet-spaces-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-meet/scopes/google-meet-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Google
- Google Workspace
- Meetings
- Recording
- Transcripts
- Video Conferencing
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
