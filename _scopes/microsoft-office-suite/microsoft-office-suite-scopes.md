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
name: Microsoft Office Suite Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Office Suite publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Office Suite API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Office Suite
provider_slug: microsoft-office-suite
schemes:
- description: Microsoft Entra ID (Azure AD) OAuth 2.0. Use the authorization code, client credentials, or device code flow depending on the scenario.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-office-suite-openapi.yml
scope_count: 7
scope_names:
- ChannelMessage.Send
- Files.Read
- Files.ReadWrite
- Mail.Read
- Mail.Send
- Team.ReadBasic.All
- User.Read
scopes:
- description: Send channel messages
  flows:
  - authorizationCode
  scope: ChannelMessage.Send
- description: Read user files
  flows:
  - authorizationCode
  scope: Files.Read
- description: Read and write user files
  flows:
  - authorizationCode
  scope: Files.ReadWrite
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Send mail as user
  flows:
  - authorizationCode
  scope: Mail.Send
- description: Read basic team info
  flows:
  - authorizationCode
  scope: Team.ReadBasic.All
- description: Sign in and read user profile
  flows:
  - authorizationCode
  scope: User.Read
slug: microsoft-office-suite-scopes
source_filename: microsoft-office-suite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-office-suite-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-office-suite-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0. Use the authorization code, client credentials,\n    or device code flow depending on the scenario.\nscopes:\n- scope: ChannelMessage.Send\n  description: Send channel messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-suite-openapi.yml\n- scope: Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-suite-openapi.yml\n- scope: Files.ReadWrite\n  description: Read and write user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-suite-openapi.yml\n\
  - scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-suite-openapi.yml\n- scope: Mail.Send\n  description: Send mail as user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-suite-openapi.yml\n- scope: Team.ReadBasic.All\n  description: Read basic team info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-suite-openapi.yml\n- scope: User.Read\n  description: Sign in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-suite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-suite/refs/heads/main/scopes/microsoft-office-suite-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Cloud
- Collaboration
- Documents
- Microsoft 365
- Office
- Productivity
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
