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
name: Microsoft Excel Advanced Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Excel (Advanced) publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Excel (Advanced) API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Excel (Advanced)
provider_slug: microsoft-excel-advanced
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-excel-advanced-openapi.yml
scope_count: 4
scope_names:
- Files.Read
- Files.ReadWrite
- Sites.Read.All
- Sites.ReadWrite.All
scopes:
- description: Read user files
  flows:
  - authorizationCode
  scope: Files.Read
- description: Read and write user files
  flows:
  - authorizationCode
  scope: Files.ReadWrite
- description: Read items in all site collections
  flows:
  - authorizationCode
  scope: Sites.Read.All
- description: Read and write items in all site collections
  flows:
  - authorizationCode
  scope: Sites.ReadWrite.All
slug: microsoft-excel-advanced-scopes
source_filename: microsoft-excel-advanced-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-excel-advanced-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-excel-advanced-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\nscopes:\n- scope: Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-excel-advanced-openapi.yml\n- scope: Files.ReadWrite\n  description: Read and write user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-excel-advanced-openapi.yml\n- scope: Sites.Read.All\n  description: Read items in all site collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-excel-advanced-openapi.yml\n- scope: Sites.ReadWrite.All\n  description: Read and write items in all site\
  \ collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-excel-advanced-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel-advanced/refs/heads/main/scopes/microsoft-excel-advanced-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Automation
- Business Intelligence
- Data Analysis
- Office
- Spreadsheets
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
