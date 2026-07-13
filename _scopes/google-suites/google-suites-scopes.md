---
api_specs:
- filename: rest
  format: yaml
  label: Gmail API
  slug: gmail-api
  spec_type: OpenAPI
  url: https://gmail.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Calendar API
  slug: google-calendar-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/calendar/v3/rest
- filename: rest
  format: yaml
  label: Google Drive API
  slug: google-drive-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/drive/v3/rest
- filename: rest
  format: yaml
  label: Google Docs API
  slug: google-docs-api
  spec_type: OpenAPI
  url: https://docs.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Sheets API
  slug: google-sheets-api
  spec_type: OpenAPI
  url: https://sheets.googleapis.com/$discovery/rest?version=v4
- filename: rest
  format: yaml
  label: Google Slides API
  slug: google-slides-api
  spec_type: OpenAPI
  url: https://slides.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Admin SDK Directory API
  slug: admin-sdk-directory-api
  spec_type: OpenAPI
  url: https://admin.googleapis.com/$discovery/rest?version=directory_v1
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Suites Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Workspace APIs publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Workspace APIs API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Workspace APIs
provider_slug: google-suites
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: googleOAuth
  source: openapi/google-suites-openapi.yml
scope_count: 6
scope_names:
- https://www.googleapis.com/auth/calendar
- https://www.googleapis.com/auth/calendar.events
- https://www.googleapis.com/auth/drive
- https://www.googleapis.com/auth/drive.file
- https://www.googleapis.com/auth/gmail.modify
- https://www.googleapis.com/auth/gmail.send
scopes:
- description: Calendar full access
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar
- description: Calendar events
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.events
- description: Drive full access
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive
- description: Drive per-file access
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.file
- description: Gmail read/write
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.modify
- description: Gmail send
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.send
slug: google-suites-scopes
source_filename: google-suites-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-suites-openapi.yml\nschemes:\n- name: googleOAuth\n  source: openapi/google-suites-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/calendar\n  description: Calendar full access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suites-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.events\n  description: Calendar events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suites-openapi.yml\n- scope: https://www.googleapis.com/auth/drive\n  description: Drive full access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suites-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.file\n  description: Drive per-file access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suites-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/gmail.modify\n  description: Gmail read/write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suites-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.send\n  description: Gmail send\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suites-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-suites/refs/heads/main/scopes/google-suites-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Cloud Storage
- Collaboration
- Email
- Office Suite
- Productivity
token_urls:
- https://oauth2.googleapis.com/token
---
