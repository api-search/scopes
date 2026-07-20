---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/openapi.yaml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: https://learn.microsoft.com/en-us/graph/permissions-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Office Scopes
name_suffix: OAuth Scopes
note: The 7 scopes below the OpenAPI subset are supplemented by additional commonly used delegated Microsoft Graph permissions relevant to the Office 365 surface, taken from the Graph permissions reference. Microsoft Graph documents hundreds of delegated and application permissions; see docs for the full registry.
overview: 'Microsoft Office publishes 16 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Office API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Office
provider_slug: microsoft-office
schemes:
- description: Microsoft Entra ID (Azure AD) OAuth 2.0. Use the authorization code, client credentials, or device code flow depending on the scenario.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-office-openapi.yml
scope_count: 16
scope_names:
- ChannelMessage.Send
- Files.Read
- Files.ReadWrite
- Mail.Read
- Mail.Send
- Team.ReadBasic.All
- User.Read
- Mail.ReadWrite
- Calendars.ReadWrite
- Contacts.Read
- Files.ReadWrite.All
- Sites.Read.All
- Chat.Read
- ChannelMessage.Read.All
- offline_access
- openid
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
- description: Read and write access to user mail
  flows:
  - authorizationCode
  scope: Mail.ReadWrite
- description: Read and write user calendars
  flows:
  - authorizationCode
  scope: Calendars.ReadWrite
- description: Read user contacts
  flows:
  - authorizationCode
  scope: Contacts.Read
- description: Read and write all files the user can access
  flows:
  - authorizationCode
  scope: Files.ReadWrite.All
- description: Read items in all SharePoint site collections
  flows:
  - authorizationCode
  scope: Sites.Read.All
- description: Read the user's Teams chat messages
  flows:
  - authorizationCode
  scope: Chat.Read
- description: Read user's Teams channel messages
  flows:
  - authorizationCode
  scope: ChannelMessage.Read.All
- description: Maintain access to data via refresh tokens
  flows:
  - authorizationCode
  scope: offline_access
- description: Sign the user in with OpenID Connect
  flows:
  - authorizationCode
  scope: openid
slug: microsoft-office-scopes
source_filename: microsoft-office-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/microsoft-office-openapi.yml\ndocs: https://learn.microsoft.com/en-us/graph/permissions-reference\nnote: >-\n  The 7 scopes below the OpenAPI subset are supplemented by additional commonly\n  used delegated Microsoft Graph permissions relevant to the Office 365 surface,\n  taken from the Graph permissions reference. Microsoft Graph documents hundreds\n  of delegated and application permissions; see docs for the full registry.\nschemes:\n- name: oauth2\n  source: openapi/microsoft-office-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0. Use the authorization code, client credentials,\n    or device code flow depending on the scenario.\nscopes:\n- scope: ChannelMessage.Send\n  description: Send channel messages\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-openapi.yml\n- scope: Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-openapi.yml\n- scope: Files.ReadWrite\n  description: Read and write user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-openapi.yml\n- scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-openapi.yml\n- scope: Mail.Send\n  description: Send mail as user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-openapi.yml\n- scope: Team.ReadBasic.All\n  description: Read basic team info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-openapi.yml\n- scope: User.Read\n  description: Sign in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-office-openapi.yml\n- scope: Mail.ReadWrite\n  description:\
  \ Read and write access to user mail\n  flows:\n  - authorizationCode\n  sources:\n  - https://learn.microsoft.com/en-us/graph/permissions-reference\n- scope: Calendars.ReadWrite\n  description: Read and write user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - https://learn.microsoft.com/en-us/graph/permissions-reference\n- scope: Contacts.Read\n  description: Read user contacts\n  flows:\n  - authorizationCode\n  sources:\n  - https://learn.microsoft.com/en-us/graph/permissions-reference\n- scope: Files.ReadWrite.All\n  description: Read and write all files the user can access\n  flows:\n  - authorizationCode\n  sources:\n  - https://learn.microsoft.com/en-us/graph/permissions-reference\n- scope: Sites.Read.All\n  description: Read items in all SharePoint site collections\n  flows:\n  - authorizationCode\n  sources:\n  - https://learn.microsoft.com/en-us/graph/permissions-reference\n- scope: Chat.Read\n  description: Read the user's Teams chat messages\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - https://learn.microsoft.com/en-us/graph/permissions-reference\n- scope: ChannelMessage.Read.All\n  description: Read user's Teams channel messages\n  flows:\n  - authorizationCode\n  sources:\n  - https://learn.microsoft.com/en-us/graph/permissions-reference\n- scope: offline_access\n  description: Maintain access to data via refresh tokens\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n- scope: openid\n  description: Sign the user in with OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office/refs/heads/main/scopes/microsoft-office-scopes.yml
summary_line: 16 scopes · authorizationCode
tags:
- Collaboration
- Documents
- Microsoft
- Office
- Productivity
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
