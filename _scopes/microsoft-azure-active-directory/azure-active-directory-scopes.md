---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: microsoft-graph-identity-api.yml
  format: yaml
  label: Microsoft Graph Identity and Access API
  slug: microsoft-graph-identity-and-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/openapi/microsoft-graph-identity-api.yml
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
name: Azure Active Directory Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure Active Directory publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure Active Directory API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schemes:
- description: Microsoft identity platform OAuth 2.0 authorization. Supports authorization code flow, client credentials flow, and on-behalf-of flow. All API calls require a valid access token obtained from the Microsoft identity platform.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-graph-identity-api.yml
scope_count: 12
scope_names:
- Application.Read.All
- Application.ReadWrite.All
- Directory.Read.All
- Directory.ReadWrite.All
- Group.Read.All
- Group.ReadWrite.All
- GroupMember.Read.All
- GroupMember.ReadWrite.All
- User.Read
- User.Read.All
- User.ReadWrite.All
- https://graph.microsoft.com/.default
scopes:
- description: Read all applications
  flows:
  - authorizationCode
  scope: Application.Read.All
- description: Read and write all applications
  flows:
  - authorizationCode
  scope: Application.ReadWrite.All
- description: Read directory data
  flows:
  - authorizationCode
  scope: Directory.Read.All
- description: Read and write directory data
  flows:
  - authorizationCode
  scope: Directory.ReadWrite.All
- description: Read all groups
  flows:
  - authorizationCode
  scope: Group.Read.All
- description: Read and write all groups
  flows:
  - authorizationCode
  scope: Group.ReadWrite.All
- description: Read group memberships
  flows:
  - authorizationCode
  scope: GroupMember.Read.All
- description: Read and write group memberships
  flows:
  - authorizationCode
  scope: GroupMember.ReadWrite.All
- description: Sign in and read user profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Read all users' full profiles
  flows:
  - authorizationCode
  scope: User.Read.All
- description: Read and write all users' full profiles
  flows:
  - authorizationCode
  scope: User.ReadWrite.All
- description: Default scope for client credentials
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: azure-active-directory-scopes
source_filename: azure-active-directory-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-graph-identity-api.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-graph-identity-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: Microsoft identity platform OAuth 2.0 authorization. Supports authorization code\n    flow, client credentials flow, and on-behalf-of flow. All API calls require a valid access\n    token obtained from the Microsoft identity platform.\nscopes:\n- scope: Application.Read.All\n  description: Read all applications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: Application.ReadWrite.All\n  description: Read and write all applications\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: Directory.Read.All\n  description: Read directory data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: Directory.ReadWrite.All\n  description: Read and write directory data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: Group.Read.All\n  description: Read all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: Group.ReadWrite.All\n  description: Read and write all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: GroupMember.Read.All\n  description: Read group memberships\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: GroupMember.ReadWrite.All\n  description: Read and write group memberships\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: User.Read\n  description: Sign in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: User.Read.All\n  description: Read all users' full profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: User.ReadWrite.All\n  description: Read and write all users' full profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n- scope: https://graph.microsoft.com/.default\n  description: Default scope for client credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/scopes/azure-active-directory-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Authentication
- Authorization
- Identity
- Microsoft
- Microsoft Entra
- OAuth
- OpenID Connect
- SAML
- SCIM
- Single Sign-On
- Zero Trust
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
