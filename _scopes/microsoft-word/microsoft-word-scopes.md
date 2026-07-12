---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Word Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Word publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Word API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Word
provider_slug: microsoft-word
schemes:
- description: OAuth 2.0 authorization code flow with Microsoft Identity Platform.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-word-graph-api.yaml
- description: OAuth 2.0 via Microsoft Identity Platform for Office Add-ins.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-word-javascript-api.yaml
scope_count: 4
scope_names:
- Files.Read
- Files.Read.All
- Files.ReadWrite
- Files.ReadWrite.All
scopes:
- description: Read user files
  flows:
  - authorizationCode
  scope: Files.Read
- description: Read all files the user can access
  flows:
  - authorizationCode
  scope: Files.Read.All
- description: Read and write user files
  flows:
  - authorizationCode
  scope: Files.ReadWrite
- description: Read and write all files the user can access
  flows:
  - authorizationCode
  scope: Files.ReadWrite.All
slug: microsoft-word-scopes
source_filename: microsoft-word-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-word-graph-api.yaml, openapi/microsoft-word-javascript-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-word-graph-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization code flow with Microsoft Identity Platform.\n- name: oauth2\n  source: openapi/microsoft-word-javascript-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 via Microsoft Identity Platform for Office Add-ins.\nscopes:\n- scope: Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-word-graph-api.yaml\n\
  - scope: Files.Read.All\n  description: Read all files the user can access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-word-graph-api.yaml\n- scope: Files.ReadWrite\n  description: Read and write user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-word-graph-api.yaml\n  - openapi/microsoft-word-javascript-api.yaml\n- scope: Files.ReadWrite.All\n  description: Read and write all files the user can access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-word-graph-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/scopes/microsoft-word-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
