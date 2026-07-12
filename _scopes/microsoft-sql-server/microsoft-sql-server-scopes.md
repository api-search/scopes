---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Sql Server Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft SQL Server publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft SQL Server API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft SQL Server
provider_slug: microsoft-sql-server
schemes:
- description: For Azure SQL management endpoints, authenticate via Microsoft Entra ID against https://management.azure.com/.default. Data API Builder endpoints can be configured to use anonymous, EasyAuth, JWT, or Microsoft Entra ID authentication depending on deployment.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-sql-server-openapi.yml
scope_count: 1
scope_names:
- https://management.azure.com/.default
scopes:
- description: Manage Azure resources
  flows:
  - clientCredentials
  scope: https://management.azure.com/.default
slug: microsoft-sql-server-scopes
source_filename: microsoft-sql-server-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-sql-server-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-sql-server-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: For Azure SQL management endpoints, authenticate via Microsoft Entra ID against\n    https://management.azure.com/.default. Data API Builder endpoints can be configured to use\n    anonymous, EasyAuth, JWT, or Microsoft Entra ID authentication depending on deployment.\nscopes:\n- scope: https://management.azure.com/.default\n  description: Manage Azure resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-sql-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-sql-server/refs/heads/main/scopes/microsoft-sql-server-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Cloud
- Data Management
- Database
- Enterprise
- Relational Database
- SQL
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
