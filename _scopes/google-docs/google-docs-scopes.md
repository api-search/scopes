---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Docs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Docs publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Docs API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Docs
provider_slug: google-docs
schemes:
- description: OAuth 2.0 authentication for Google APIs.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-docs-api-v1-openapi.yml
scope_count: 5
scope_names:
- https://www.googleapis.com/auth/documents
- https://www.googleapis.com/auth/documents.readonly
- https://www.googleapis.com/auth/drive
- https://www.googleapis.com/auth/drive.file
- https://www.googleapis.com/auth/drive.readonly
scopes:
- description: View and manage your Google Docs documents
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/documents
- description: View your Google Docs documents
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/documents.readonly
- description: See, edit, create, and delete all of your Google Drive files
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive
- description: View and manage Google Drive files and folders that you have opened or created with this app
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.file
- description: See and download all your Google Drive files
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.readonly
slug: google-docs-scopes
source_filename: google-docs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-docs-api-v1-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-docs-api-v1-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for Google APIs.\nscopes:\n- scope: https://www.googleapis.com/auth/documents\n  description: View and manage your Google Docs documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-docs-api-v1-openapi.yml\n- scope: https://www.googleapis.com/auth/documents.readonly\n  description: View your Google Docs documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-docs-api-v1-openapi.yml\n- scope: https://www.googleapis.com/auth/drive\n  description: See, edit, create, and delete all of your Google Drive files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-docs-api-v1-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/drive.file\n  description: View and manage Google Drive files and folders that you have opened or created\n    with this app\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-docs-api-v1-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.readonly\n  description: See and download all your Google Drive files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-docs-api-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/scopes/google-docs-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
token_urls:
- https://oauth2.googleapis.com/token
---
