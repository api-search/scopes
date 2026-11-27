---
api_specs:
- filename: google-keep-notes-api-openapi.yml
  format: yaml
  label: Google Keep Notes API
  slug: google-keep-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-keep/openapi/google-keep-notes-api-openapi.yml
- filename: google-keep-media-api-openapi.yml
  format: yaml
  label: Google Keep Keep Media API
  slug: google-keep-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-keep/openapi/google-keep-media-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: https://developers.google.com/workspace/keep/api/guides/java
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Keep Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Keep publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Keep API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Keep
provider_slug: google-keep
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-keep-media-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-keep-notes-api-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/keep
- https://www.googleapis.com/auth/keep.readonly
scopes:
- description: See, edit, create and permanently delete all your Google Keep data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/keep
- description: View all your Google Keep data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/keep.readonly
slug: google-keep-scopes
source_filename: google-keep-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://developers.google.com/workspace/keep/api/guides/java\nschemes:\n- name: oauth2\n  source: openapi/google-keep-media-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-keep-notes-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/keep\n  description: See, edit, create and permanently delete all your Google Keep data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-keep-media-api-openapi.yml\n  - openapi/google-keep-notes-api-openapi.yml\n- scope: https://www.googleapis.com/auth/keep.readonly\n  description: View all your Google Keep data\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/google-keep-media-api-openapi.yml\n  - openapi/google-keep-notes-api-openapi.yml\ndocs: https://developers.google.com/workspace/keep/api/guides/java\n"
source_yaml_url: https://artifacts.apis.io/google-keep/scopes/google-keep-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Google
- Google Workspace
- Notes
- Organization
- Productivity
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
