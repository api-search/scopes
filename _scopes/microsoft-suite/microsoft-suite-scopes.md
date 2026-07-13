---
api_specs:
- filename: openapi
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://developer.microsoft.com/graph/openapi
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
name: Microsoft Suite Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Suite publishes 8 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Suite API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Suite
provider_slug: microsoft-suite
schemes:
- description: Microsoft identity platform (Microsoft Entra ID) OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: OAuth2
  source: openapi/microsoft-suite-openapi.yml
scope_count: 8
scope_names:
- Calendars.ReadWrite
- Files.ReadWrite.All
- Group.ReadWrite.All
- Mail.Read
- Mail.Send
- User.Read
- User.ReadWrite.All
- https://graph.microsoft.com/.default
scopes:
- description: Read/write calendars
  flows:
  - authorizationCode
  scope: Calendars.ReadWrite
- description: Read/write all files
  flows:
  - authorizationCode
  scope: Files.ReadWrite.All
- description: Read/write all groups
  flows:
  - authorizationCode
  scope: Group.ReadWrite.All
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Send mail as user
  flows:
  - authorizationCode
  scope: Mail.Send
- description: Sign-in and read user profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Read and write all users
  flows:
  - authorizationCode
  scope: User.ReadWrite.All
- description: Default app permissions
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: microsoft-suite-scopes
source_filename: microsoft-suite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-suite-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/microsoft-suite-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft identity platform (Microsoft Entra ID) OAuth 2.0\nscopes:\n- scope: Calendars.ReadWrite\n  description: Read/write calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-suite-openapi.yml\n- scope: Files.ReadWrite.All\n  description: Read/write all files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-suite-openapi.yml\n- scope: Group.ReadWrite.All\n  description: Read/write all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-suite-openapi.yml\n\
  - scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-suite-openapi.yml\n- scope: Mail.Send\n  description: Send mail as user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-suite-openapi.yml\n- scope: User.Read\n  description: Sign-in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-suite-openapi.yml\n- scope: User.ReadWrite.All\n  description: Read and write all users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-suite-openapi.yml\n- scope: https://graph.microsoft.com/.default\n  description: Default app permissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-suite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/scopes/microsoft-suite-scopes.yml
summary_line: 8 scopes · authorizationCode/clientCredentials
tags:
- Cloud
- Enterprise
- Productivity
- SaaS
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
