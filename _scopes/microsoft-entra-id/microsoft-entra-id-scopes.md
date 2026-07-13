---
api_specs:
- filename: microsoft-entra-id-openapi.yml
  format: yaml
  label: Microsoft Entra ID
  slug: microsoft-entra-id
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/openapi/microsoft-entra-id-openapi.yml
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
name: Microsoft Entra Id Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Entra ID publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Entra ID API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Entra ID
provider_slug: microsoft-entra-id
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token via Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-entra-id-openapi.yml
scope_count: 6
scope_names:
- Application.ReadWrite.All
- Directory.ReadWrite.All
- Group.ReadWrite.All
- User.Read
- User.ReadWrite.All
- https://graph.microsoft.com/.default
scopes:
- description: Read and write all applications
  flows:
  - authorizationCode
  scope: Application.ReadWrite.All
- description: Read and write directory data
  flows:
  - authorizationCode
  scope: Directory.ReadWrite.All
- description: Read and write all groups
  flows:
  - authorizationCode
  scope: Group.ReadWrite.All
- description: Sign in and read user profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Read and write all users' full profiles
  flows:
  - authorizationCode
  scope: User.ReadWrite.All
- description: Microsoft Graph default scopes
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: microsoft-entra-id-scopes
source_filename: microsoft-entra-id-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-entra-id-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-entra-id-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token via Microsoft identity platform\nscopes:\n- scope: Application.ReadWrite.All\n  description: Read and write all applications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n- scope: Directory.ReadWrite.All\n  description: Read and write directory data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n- scope: Group.ReadWrite.All\n  description: Read and write all groups\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n- scope: User.Read\n  description: Sign in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n- scope: User.ReadWrite.All\n  description: Read and write all users' full profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n- scope: https://graph.microsoft.com/.default\n  description: Microsoft Graph default scopes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/scopes/microsoft-entra-id-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Authentication
- Identity Provider
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
