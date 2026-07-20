---
api_specs:
- filename: microsoft-excel-graph-api.yaml
  format: yaml
  label: Microsoft Graph Excel API
  slug: microsoft-graph-excel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-graph-api.yaml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: https://learn.microsoft.com/en-us/graph/permissions-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Excel Scopes
name_suffix: OAuth Scopes
note: Baseline (Files.Read, Files.ReadWrite) derived from the OpenAPI oauth2 flow; the .All and Sites.* scopes added from the Microsoft Graph permissions reference — they are the delegated permissions required to reach Excel workbooks beyond the signed-in user's own files (shared files and SharePoint-hosted workbooks).
overview: 'Microsoft Excel publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Excel API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Excel
provider_slug: microsoft-excel
schemes:
- description: OAuth 2.0 authorization using Microsoft Identity Platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-excel-graph-api.yaml
scope_count: 6
scope_names:
- Files.Read
- Files.ReadWrite
- Files.Read.All
- Files.ReadWrite.All
- Sites.Read.All
- Sites.ReadWrite.All
scopes:
- description: Read the signed-in user's files.
  flows:
  - authorizationCode
  scope: Files.Read
- description: Read, create, update and delete the signed-in user's files.
  flows:
  - authorizationCode
  scope: Files.ReadWrite
- description: Read all files the signed-in user can access.
  flows:
  - authorizationCode
  scope: Files.Read.All
- description: Read, create, update and delete all files the signed-in user can access.
  flows:
  - authorizationCode
  scope: Files.ReadWrite.All
- description: Read documents and list items in all site collections on behalf of the signed-in user (SharePoint-hosted workbooks).
  flows:
  - authorizationCode
  scope: Sites.Read.All
- description: Edit or delete documents and list items in all site collections on behalf of the signed-in user (SharePoint-hosted workbooks).
  flows:
  - authorizationCode
  scope: Sites.ReadWrite.All
slug: microsoft-excel-scopes
source_filename: microsoft-excel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/microsoft-excel-graph-api.yaml\ndocs: https://learn.microsoft.com/en-us/graph/permissions-reference\nnote: >-\n  Baseline (Files.Read, Files.ReadWrite) derived from the OpenAPI oauth2 flow; the .All and\n  Sites.* scopes added from the Microsoft Graph permissions reference — they are the\n  delegated permissions required to reach Excel workbooks beyond the signed-in user's own\n  files (shared files and SharePoint-hosted workbooks).\nschemes:\n- name: oauth2\n  source: openapi/microsoft-excel-graph-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization using Microsoft Identity Platform\nscopes:\n- scope: Files.Read\n  description: Read the signed-in user's files.\n  flows: [authorizationCode]\n  sources: [openapi/microsoft-excel-graph-api.yaml]\n\
  - scope: Files.ReadWrite\n  description: Read, create, update and delete the signed-in user's files.\n  flows: [authorizationCode]\n  sources: [openapi/microsoft-excel-graph-api.yaml]\n- scope: Files.Read.All\n  description: Read all files the signed-in user can access.\n  flows: [authorizationCode]\n  sources: [docs]\n- scope: Files.ReadWrite.All\n  description: Read, create, update and delete all files the signed-in user can access.\n  flows: [authorizationCode]\n  sources: [docs]\n- scope: Sites.Read.All\n  description: Read documents and list items in all site collections on behalf of the signed-in user (SharePoint-hosted workbooks).\n  flows: [authorizationCode]\n  sources: [docs]\n- scope: Sites.ReadWrite.All\n  description: Edit or delete documents and list items in all site collections on behalf of the signed-in user (SharePoint-hosted workbooks).\n  flows: [authorizationCode]\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/scopes/microsoft-excel-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
