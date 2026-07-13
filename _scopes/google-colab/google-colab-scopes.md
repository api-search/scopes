---
api_specs:
- filename: colab-drive-openapi.yml
  format: yaml
  label: Colab API via Google Drive API
  slug: colab-api-via-google-drive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-colab/refs/heads/main/openapi/colab-drive-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Colab Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Colab publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Colab API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Colab
provider_slug: google-colab
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/colab-drive-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/drive
- https://www.googleapis.com/auth/drive.file
scopes:
- description: Full Drive access
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive
- description: Per-file access
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/drive.file
slug: google-colab-scopes
source_filename: google-colab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/colab-drive-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/colab-drive-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/drive\n  description: Full Drive access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/colab-drive-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.file\n  description: Per-file access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/colab-drive-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-colab/refs/heads/main/scopes/google-colab-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Collaboration
- Data Science
- Google Cloud
- Jupyter
- Machine Learning
- Notebooks
- Python
token_urls:
- https://oauth2.googleapis.com/token
---
