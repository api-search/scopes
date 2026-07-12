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
name: Spreadsheets Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Spreadsheets publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spreadsheets API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spreadsheets
provider_slug: spreadsheets
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-sheets-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/spreadsheets
- https://www.googleapis.com/auth/spreadsheets.readonly
scopes:
- description: Read and write access to Google Sheets
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/spreadsheets
- description: Read-only access to Google Sheets
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/spreadsheets.readonly
slug: spreadsheets-scopes
source_filename: spreadsheets-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-sheets-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-sheets-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/spreadsheets\n  description: Read and write access to Google Sheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-sheets-openapi.yml\n- scope: https://www.googleapis.com/auth/spreadsheets.readonly\n  description: Read-only access to Google Sheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-sheets-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spreadsheets/refs/heads/main/scopes/spreadsheets-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Spreadsheets
- Data
- Google Sheets
- Excel
- Productivity
- Automation
token_urls:
- https://oauth2.googleapis.com/token
---
