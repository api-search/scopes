---
api_specs:
- filename: rest
  format: yaml
  label: Google Slides API
  slug: google-slides-api
  spec_type: OpenAPI
  url: https://slides.googleapis.com/$discovery/rest?version=v1
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Slides Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Slides publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Slides API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Slides
provider_slug: google-slides
schemes:
- description: Google OAuth 2.0 authentication. Requires one of the following scopes depending on the operation.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-slides-api-openapi.yml
scope_count: 7
scope_names:
- https://www.googleapis.com/auth/drive
- https://www.googleapis.com/auth/drive.file
- https://www.googleapis.com/auth/drive.readonly
- https://www.googleapis.com/auth/presentations
- https://www.googleapis.com/auth/presentations.readonly
- https://www.googleapis.com/auth/spreadsheets
- https://www.googleapis.com/auth/spreadsheets.readonly
scopes:
- description: See, edit, create, and delete all of your Google Drive files
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive
- description: See, edit, create, and delete only the specific Google Drive files you use with this app
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.file
- description: See and download all your Google Drive files
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.readonly
- description: See, edit, create, and delete all your Google Slides presentations
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/presentations
- description: See all your Google Slides presentations
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/presentations.readonly
- description: See, edit, create, and delete all your Google Sheets spreadsheets
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/spreadsheets
- description: See all your Google Sheets spreadsheets
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/spreadsheets.readonly
slug: google-slides-scopes
source_filename: google-slides-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-slides-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-slides-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0 authentication. Requires one of the following scopes depending\n    on the operation.\nscopes:\n- scope: https://www.googleapis.com/auth/drive\n  description: See, edit, create, and delete all of your Google Drive files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-slides-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.file\n  description: See, edit, create, and delete only the specific Google Drive files you use with\n    this app\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-slides-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.readonly\n  description: See\
  \ and download all your Google Drive files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-slides-api-openapi.yml\n- scope: https://www.googleapis.com/auth/presentations\n  description: See, edit, create, and delete all your Google Slides presentations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-slides-api-openapi.yml\n- scope: https://www.googleapis.com/auth/presentations.readonly\n  description: See all your Google Slides presentations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-slides-api-openapi.yml\n- scope: https://www.googleapis.com/auth/spreadsheets\n  description: See, edit, create, and delete all your Google Sheets spreadsheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-slides-api-openapi.yml\n- scope: https://www.googleapis.com/auth/spreadsheets.readonly\n  description: See all your Google Sheets spreadsheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-slides-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/scopes/google-slides-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
token_urls:
- https://oauth2.googleapis.com/token
---
