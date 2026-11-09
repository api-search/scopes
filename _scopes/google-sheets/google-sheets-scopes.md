---
api_specs:
- filename: google-sheets-sheets-api-openapi.yml
  format: yaml
  label: Google Sheets API
  slug: google-sheets-sheets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-sheets/openapi/google-sheets-sheets-api-openapi.yml
- filename: google-sheets-spreadsheets-api-openapi.yml
  format: yaml
  label: Google Sheets Spreadsheets API
  slug: google-sheets-spreadsheets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-sheets/openapi/google-sheets-spreadsheets-api-openapi.yml
- filename: google-sheets-values-api-openapi.yml
  format: yaml
  label: Google Sheets Values API
  slug: google-sheets-values-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-sheets/openapi/google-sheets-values-api-openapi.yml
- filename: google-sheets-developer-metadata-api-openapi.yml
  format: yaml
  label: Google Sheets Developer Metadata API
  slug: google-sheets-developer-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-sheets/openapi/google-sheets-developer-metadata-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: https://developers.google.com/workspace/sheets/api/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Sheets Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Sheets publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Sheets API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Sheets
provider_slug: google-sheets
schemes: []
scope_count: 5
scope_names:
- https://www.googleapis.com/auth/drive.readonly
- https://www.googleapis.com/auth/spreadsheets
- https://www.googleapis.com/auth/drive.file
- https://www.googleapis.com/auth/spreadsheets.readonly
- https://www.googleapis.com/auth/drive
scopes:
- description: See and download all your Google Drive files
  flows: []
  scope: https://www.googleapis.com/auth/drive.readonly
- description: See, edit, create, and delete all your Google Sheets spreadsheets
  flows: []
  scope: https://www.googleapis.com/auth/spreadsheets
- description: See, edit, create, and delete only the specific Google Drive files you use with this app
  flows: []
  scope: https://www.googleapis.com/auth/drive.file
- description: See all your Google Sheets spreadsheets
  flows: []
  scope: https://www.googleapis.com/auth/spreadsheets.readonly
- description: See, edit, create, and delete all of your Google Drive files
  flows: []
  scope: https://www.googleapis.com/auth/drive
slug: google-sheets-scopes
source_filename: google-sheets-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Google Sheets OAuth scopes\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://developers.google.com/workspace/sheets/api/scopes; https://sheets.googleapis.com/$discovery/rest?version=v4 (auth.oauth2.scopes)\ndocs: https://developers.google.com/workspace/sheets/api/scopes\nauthorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\ntokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/drive.readonly\n  description: See and download all your Google Drive files\n- scope: https://www.googleapis.com/auth/spreadsheets\n  description: See, edit, create, and delete all your Google Sheets spreadsheets\n- scope: https://www.googleapis.com/auth/drive.file\n  description: See, edit, create, and delete only the specific Google Drive files you use with this app\n- scope: https://www.googleapis.com/auth/spreadsheets.readonly\n  description: See all your Google Sheets spreadsheets\n- scope: https://www.googleapis.com/auth/drive\n\
  \  description: See, edit, create, and delete all of your Google Drive files\n"
source_yaml_url: https://artifacts.apis.io/google-sheets/scopes/google-sheets-scopes.yml
summary_line: 5 scopes
tags:
- Google Workspace
- Productivity
- Spreadsheets
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
