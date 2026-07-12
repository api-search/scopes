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
name: Google Forms Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Forms publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Forms API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Forms
provider_slug: google-forms
schemes:
- description: OAuth 2.0 authentication for Google Forms API.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-forms-api.yaml
scope_count: 6
scope_names:
- https://www.googleapis.com/auth/drive
- https://www.googleapis.com/auth/drive.file
- https://www.googleapis.com/auth/drive.readonly
- https://www.googleapis.com/auth/forms.body
- https://www.googleapis.com/auth/forms.body.readonly
- https://www.googleapis.com/auth/forms.responses.readonly
scopes:
- description: See, edit, create, and delete all of your Google Drive files
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive
- description: View and manage Google Drive files created with this app
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.file
- description: View files in your Google Drive
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.readonly
- description: View and manage your forms in Google Drive
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/forms.body
- description: View your forms in Google Drive
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/forms.body.readonly
- description: View responses to your Google Forms
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/forms.responses.readonly
slug: google-forms-scopes
source_filename: google-forms-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-forms-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/google-forms-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for Google Forms API.\nscopes:\n- scope: https://www.googleapis.com/auth/drive\n  description: See, edit, create, and delete all of your Google Drive files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-forms-api.yaml\n- scope: https://www.googleapis.com/auth/drive.file\n  description: View and manage Google Drive files created with this app\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-forms-api.yaml\n- scope: https://www.googleapis.com/auth/drive.readonly\n  description: View files in your Google Drive\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-forms-api.yaml\n- scope: https://www.googleapis.com/auth/forms.body\n\
  \  description: View and manage your forms in Google Drive\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-forms-api.yaml\n- scope: https://www.googleapis.com/auth/forms.body.readonly\n  description: View your forms in Google Drive\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-forms-api.yaml\n- scope: https://www.googleapis.com/auth/forms.responses.readonly\n  description: View responses to your Google Forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-forms-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/scopes/google-forms-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Data Collection
- Forms
- Google
- Google Workspace
- Questionnaires
- Responses
- Surveys
token_urls:
- https://oauth2.googleapis.com/token
---
