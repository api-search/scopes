---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft 365 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft 365 publishes 8 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft 365 API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft 365
provider_slug: microsoft-365
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-365-openapi.yml
scope_count: 8
scope_names:
- Calendars.Read
- Channel.ReadBasic.All
- Files.Read.All
- Group.Read.All
- Mail.Read
- User.Read
- User.ReadWrite.All
- https://graph.microsoft.com/.default
scopes:
- description: Read user calendars
  flows:
  - authorizationCode
  scope: Calendars.Read
- description: Read basic channel info
  flows:
  - authorizationCode
  scope: Channel.ReadBasic.All
- description: Read all files
  flows:
  - authorizationCode
  scope: Files.Read.All
- description: Read all groups
  flows:
  - authorizationCode
  scope: Group.Read.All
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Sign in and read user profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Read and write all users' full profiles
  flows:
  - authorizationCode
  scope: User.ReadWrite.All
- description: Use app-registered Graph permissions
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: microsoft-365-scopes
source_filename: microsoft-365-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-365-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-365-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\nscopes:\n- scope: Calendars.Read\n  description: Read user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-openapi.yml\n- scope: Channel.ReadBasic.All\n  description: Read basic channel info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-openapi.yml\n- scope: Files.Read.All\n  description: Read all files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-openapi.yml\n- scope: Group.Read.All\n  description:\
  \ Read all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-openapi.yml\n- scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-openapi.yml\n- scope: User.Read\n  description: Sign in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-openapi.yml\n- scope: User.ReadWrite.All\n  description: Read and write all users' full profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-openapi.yml\n- scope: https://graph.microsoft.com/.default\n  description: Use app-registered Graph permissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-365-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-365/refs/heads/main/scopes/microsoft-365-scopes.yml
summary_line: 8 scopes · authorizationCode/clientCredentials
tags:
- Productivity
- Collaboration
- Email
- Calendar
- Files
- Identity
- Microsoft
- Microsoft Graph
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
