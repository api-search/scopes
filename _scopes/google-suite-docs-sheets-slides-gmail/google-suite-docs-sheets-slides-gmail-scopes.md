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
name: Google Suite Docs Sheets Slides Gmail Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Workspace Suite publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Workspace Suite API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Workspace Suite
provider_slug: google-suite-docs-sheets-slides-gmail
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: googleOAuth
  source: openapi/google-suite-docs-sheets-slides-gmail-openapi.yml
scope_count: 6
scope_names:
- https://www.googleapis.com/auth/documents
- https://www.googleapis.com/auth/gmail.modify
- https://www.googleapis.com/auth/gmail.readonly
- https://www.googleapis.com/auth/gmail.send
- https://www.googleapis.com/auth/presentations
- https://www.googleapis.com/auth/spreadsheets
scopes:
- description: Read/write Google Docs
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/documents
- description: Read/write Gmail (no permanent delete)
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.modify
- description: Read-only access to Gmail
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.readonly
- description: Send mail on behalf of user
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.send
- description: Read/write Google Slides
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/presentations
- description: Read/write Google Sheets
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/spreadsheets
slug: google-suite-docs-sheets-slides-gmail-scopes
source_filename: google-suite-docs-sheets-slides-gmail-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\nschemes:\n- name: googleOAuth\n  source: openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/documents\n  description: Read/write Google Docs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.modify\n  description: Read/write Gmail (no permanent delete)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.readonly\n  description: Read-only access to Gmail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/gmail.send\n  description: Send mail on behalf of user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\n- scope: https://www.googleapis.com/auth/presentations\n  description: Read/write Google Slides\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\n- scope: https://www.googleapis.com/auth/spreadsheets\n  description: Read/write Google Sheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-suite-docs-sheets-slides-gmail/refs/heads/main/scopes/google-suite-docs-sheets-slides-gmail-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Cloud
- Collaboration
- Documents
- Google
- Productivity
- Workspace
token_urls:
- https://oauth2.googleapis.com/token
---
