---
api_specs:
- filename: microsoft-graph-excel-api-openapi.yml
  format: yaml
  label: Microsoft Graph Excel API
  slug: microsoft-graph-excel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/openapi/microsoft-graph-excel-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Advanced Excel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Advanced Excel publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Advanced Excel API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Advanced Excel
provider_slug: advanced-excel
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-graph-excel-api-openapi.yml
scope_count: 2
scope_names:
- Files.ReadWrite
- Files.ReadWrite.All
scopes:
- description: Read and write user files
  flows:
  - authorizationCode
  scope: Files.ReadWrite
- description: Read and write all files
  flows:
  - authorizationCode
  scope: Files.ReadWrite.All
slug: advanced-excel-scopes
source_filename: advanced-excel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-graph-excel-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-graph-excel-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\nscopes:\n- scope: Files.ReadWrite\n  description: Read and write user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-excel-api-openapi.yml\n- scope: Files.ReadWrite.All\n  description: Read and write all files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-excel-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/scopes/advanced-excel-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
