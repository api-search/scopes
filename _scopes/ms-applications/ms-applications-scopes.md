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
name: Ms Applications Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Applications APIs publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Applications APIs API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Applications APIs
provider_slug: ms-applications
schemes:
- description: Microsoft identity platform OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/ms-applications-openapi.yml
scope_count: 5
scope_names:
- Calendars.Read
- Files.Read
- Mail.Read
- User.Read
- https://graph.microsoft.com/.default
scopes:
- description: Read user calendars
  flows:
  - authorizationCode
  scope: Calendars.Read
- description: Read user files
  flows:
  - authorizationCode
  scope: Files.Read
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Sign in and read user profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Application permissions
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: ms-applications-scopes
source_filename: ms-applications-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ms-applications-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/ms-applications-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft identity platform OAuth 2.0\nscopes:\n- scope: Calendars.Read\n  description: Read user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ms-applications-openapi.yml\n- scope: Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ms-applications-openapi.yml\n- scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ms-applications-openapi.yml\n- scope: User.Read\n  description: Sign\
  \ in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ms-applications-openapi.yml\n- scope: https://graph.microsoft.com/.default\n  description: Application permissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ms-applications-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ms-applications/refs/heads/main/scopes/ms-applications-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Cloud
- Enterprise
- Microsoft
- Microsoft-365
- Office
- Productivity
- Saas
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
