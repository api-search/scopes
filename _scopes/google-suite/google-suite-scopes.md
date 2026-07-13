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
  label: Google Chat API
  slug: google-chat-api
  spec_type: OpenAPI
  url: https://chat.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Admin SDK
  slug: google-admin-sdk
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
name: Google Suite Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Workspace (G Suite) publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Workspace (G Suite) API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Workspace (G Suite)
provider_slug: google-suite
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-suite-openapi.yml
scope_count: 5
scope_names:
- gmail.compose
- gmail.labels
- gmail.modify
- gmail.readonly
- gmail.send
scopes:
- description: Create, read, update, and delete drafts; send messages and drafts
  flows:
  - authorizationCode
  scope: gmail.compose
- description: Manage mailbox labels
  flows:
  - authorizationCode
  scope: gmail.labels
- description: All read/write operations except immediate, permanent deletion
  flows:
  - authorizationCode
  scope: gmail.modify
- description: Read all resources and metadata
  flows:
  - authorizationCode
  scope: gmail.readonly
- description: Send messages only
  flows:
  - authorizationCode
  scope: gmail.send
slug: google-suite-scopes
source_filename: google-suite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-suite-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-suite-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: gmail.compose\n  description: Create, read, update, and delete drafts; send messages and drafts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-openapi.yml\n- scope: gmail.labels\n  description: Manage mailbox labels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-openapi.yml\n- scope: gmail.modify\n  description: All read/write operations except immediate, permanent deletion\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-openapi.yml\n- scope: gmail.readonly\n  description: Read all resources and metadata\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-openapi.yml\n\
  - scope: gmail.send\n  description: Send messages only\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-suite/refs/heads/main/scopes/google-suite-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Cloud
- Collaboration
- Enterprise
- Google
- Productivity
- Workspace
token_urls:
- https://oauth2.googleapis.com/token
---
