---
api_specs:
- filename: openapi
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://developer.microsoft.com/en-us/graph/docs/concepts/openapi
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
name: Microsoft 365 Copilot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft 365 Copilot publishes 7 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft 365 Copilot API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft 365 Copilot
provider_slug: microsoft-365-copilot
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-365-copilot-openapi.yml
scope_count: 7
scope_names:
- Calendars.Read
- ExternalConnection.ReadWrite.OwnedBy
- ExternalItem.ReadWrite.OwnedBy
- Files.Read.All
- Mail.Read
- User.Read
- https://graph.microsoft.com/.default
scopes:
- description: Read user calendars
  flows:
  - authorizationCode
  scope: Calendars.Read
- description: Manage owned Copilot connector connections
  flows:
  - authorizationCode
  scope: ExternalConnection.ReadWrite.OwnedBy
- description: Manage owned external items
  flows:
  - authorizationCode
  scope: ExternalItem.ReadWrite.OwnedBy
- description: Read all files
  flows:
  - authorizationCode
  scope: Files.Read.All
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Sign in and read user profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Use app-registered Graph permissions
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: microsoft-365-copilot-scopes
source_filename: microsoft-365-copilot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-365-copilot-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-365-copilot-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\nscopes:\n- scope: Calendars.Read\n  description: Read user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-copilot-openapi.yml\n- scope: ExternalConnection.ReadWrite.OwnedBy\n  description: Manage owned Copilot connector connections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-copilot-openapi.yml\n- scope: ExternalItem.ReadWrite.OwnedBy\n  description: Manage owned external items\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/microsoft-365-copilot-openapi.yml\n- scope: Files.Read.All\n  description: Read all files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-copilot-openapi.yml\n- scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-copilot-openapi.yml\n- scope: User.Read\n  description: Sign in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-365-copilot-openapi.yml\n- scope: https://graph.microsoft.com/.default\n  description: Use app-registered Graph permissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-365-copilot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-365-copilot/refs/heads/main/scopes/microsoft-365-copilot-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials
tags:
- Artificial Intelligence
- Copilot
- Enterprise
- LLM
- Microsoft 365
- Natural Language Processing
- Productivity
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
