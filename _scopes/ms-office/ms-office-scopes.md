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
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Ms Office Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Office APIs publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Office APIs API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Office APIs
provider_slug: ms-office
schemes:
- description: Microsoft identity platform OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/ms-office-openapi.yml
scope_count: 5
scope_names:
- Calendars.Read
- Files.Read
- Mail.Read
- Notes.Read
- User.Read
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
- description: Read user OneNote notebooks
  flows:
  - authorizationCode
  scope: Notes.Read
- description: Sign in and read user profile
  flows:
  - authorizationCode
  scope: User.Read
slug: ms-office-scopes
source_filename: ms-office-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ms-office-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/ms-office-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft identity platform OAuth 2.0\nscopes:\n- scope: Calendars.Read\n  description: Read user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ms-office-openapi.yml\n- scope: Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ms-office-openapi.yml\n- scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ms-office-openapi.yml\n- scope: Notes.Read\n  description: Read user OneNote notebooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ms-office-openapi.yml\n- scope: User.Read\n  description:\
  \ Sign in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ms-office-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ms-office/refs/heads/main/scopes/ms-office-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Collaboration
- Documents
- Microsoft
- Office
- Productivity
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
