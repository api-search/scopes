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
name: Azure Ad Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Active Directory publishes 8 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Active Directory API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Active Directory
provider_slug: azure-ad
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-ad-openapi.yml
scope_count: 8
scope_names:
- Application.Read.All
- Directory.Read.All
- Group.Read.All
- Group.ReadWrite.All
- User.Read
- User.Read.All
- User.ReadWrite.All
- https://graph.microsoft.com/.default
scopes:
- description: Read applications
  flows:
  - authorizationCode
  scope: Application.Read.All
- description: Read directory data
  flows:
  - authorizationCode
  scope: Directory.Read.All
- description: Read all groups
  flows:
  - authorizationCode
  scope: Group.Read.All
- description: Read and write all groups
  flows:
  - authorizationCode
  scope: Group.ReadWrite.All
- description: Read the signed-in user's profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Read all users
  flows:
  - authorizationCode
  scope: User.Read.All
- description: Read and write all users
  flows:
  - authorizationCode
  scope: User.ReadWrite.All
- description: Application permissions configured for the app
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: azure-ad-scopes
source_filename: azure-ad-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-ad-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/azure-ad-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\nscopes:\n- scope: Application.Read.All\n  description: Read applications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-ad-openapi.yml\n- scope: Directory.Read.All\n  description: Read directory data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-ad-openapi.yml\n- scope: Group.Read.All\n  description: Read all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-ad-openapi.yml\n- scope: Group.ReadWrite.All\n  description: Read and write all\
  \ groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-ad-openapi.yml\n- scope: User.Read\n  description: Read the signed-in user's profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-ad-openapi.yml\n- scope: User.Read.All\n  description: Read all users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-ad-openapi.yml\n- scope: User.ReadWrite.All\n  description: Read and write all users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-ad-openapi.yml\n- scope: https://graph.microsoft.com/.default\n  description: Application permissions configured for the app\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-ad-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/scopes/azure-ad-scopes.yml
summary_line: 8 scopes · authorizationCode/clientCredentials
tags:
- Authentication
- Authorization
- Identity
- OAuth
- OpenID Connect
- Single Sign-On
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
