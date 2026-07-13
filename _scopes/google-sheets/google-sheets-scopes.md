---
api_specs:
- filename: google-sheets-openapi.yml
  format: yaml
  label: Google Sheets API v4
  slug: google-sheets-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/openapi/google-sheets-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Sheets Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Sheets publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Sheets API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Sheets
provider_slug: google-sheets
schemes:
- description: OAuth 2.0 authentication for accessing user spreadsheets.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-sheets-openapi.yml
scope_count: 5
scope_names:
- https://www.googleapis.com/auth/drive
- https://www.googleapis.com/auth/drive.file
- https://www.googleapis.com/auth/drive.readonly
- https://www.googleapis.com/auth/spreadsheets
- https://www.googleapis.com/auth/spreadsheets.readonly
scopes:
- description: Full access to Google Drive files.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive
- description: Access to files created or opened by the app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.file
- description: Read-only access to Google Drive files.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.readonly
- description: Read and write access to all spreadsheets.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/spreadsheets
- description: Read-only access to all spreadsheets.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/spreadsheets.readonly
slug: google-sheets-scopes
source_filename: google-sheets-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-sheets-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-sheets-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for accessing user spreadsheets.\nscopes:\n- scope: https://www.googleapis.com/auth/drive\n  description: Full access to Google Drive files.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-sheets-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.file\n  description: Access to files created or opened by the app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-sheets-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.readonly\n  description: Read-only access to Google Drive files.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-sheets-openapi.yml\n- scope: https://www.googleapis.com/auth/spreadsheets\n\
  \  description: Read and write access to all spreadsheets.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-sheets-openapi.yml\n- scope: https://www.googleapis.com/auth/spreadsheets.readonly\n  description: Read-only access to all spreadsheets.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-sheets-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/scopes/google-sheets-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Google Workspace
- Productivity
- Spreadsheets
token_urls:
- https://oauth2.googleapis.com/token
---
