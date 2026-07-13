---
api_specs:
- filename: microsoft-entra-graph-identity-openapi.yml
  format: yaml
  label: Microsoft Entra ID (Azure AD) API
  slug: graph-identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/openapi/microsoft-entra-graph-identity-openapi.yml
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
name: Microsoft Entra Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Entra publishes 13 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Entra API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schemes:
- description: OAuth 2.0 authorization using Microsoft identity platform. Supports authorization code flow for delegated permissions and client credentials flow for application permissions.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-entra-graph-identity-openapi.yml
scope_count: 13
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
- User.ReadWrite
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
- description: Read all group memberships
  flows:
  - authorizationCode
  scope: GroupMember.Read.All
- description: Read and write all group memberships
  flows:
  - authorizationCode
  scope: GroupMember.ReadWrite.All
- description: Read the signed-in user's profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Read all users' profiles
  flows:
  - authorizationCode
  scope: User.Read.All
- description: Read and update the signed-in user's profile
  flows:
  - authorizationCode
  scope: User.ReadWrite
- description: Read and write all users' profiles
  flows:
  - authorizationCode
  scope: User.ReadWrite.All
- description: Default scope for application permissions
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: microsoft-entra-scopes
source_filename: microsoft-entra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-entra-graph-identity-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-entra-graph-identity-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: OAuth 2.0 authorization using Microsoft identity platform. Supports authorization\n    code flow for delegated permissions and client credentials flow for application permissions.\nscopes:\n- scope: Application.Read.All\n  description: Read all applications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: Application.ReadWrite.All\n  description: Read and write all applications\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: Directory.Read.All\n  description: Read directory data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: Directory.ReadWrite.All\n  description: Read and write directory data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: Group.Read.All\n  description: Read all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: Group.ReadWrite.All\n  description: Read and write all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: GroupMember.Read.All\n  description: Read all group memberships\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: GroupMember.ReadWrite.All\n  description: Read and write all group memberships\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: User.Read\n  description: Read the signed-in user's profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: User.Read.All\n  description: Read all users' profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: User.ReadWrite\n  description: Read and update the signed-in user's profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: User.ReadWrite.All\n  description: Read and write all users' profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n- scope: https://graph.microsoft.com/.default\n  description: Default scope for application permissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/scopes/microsoft-entra-scopes.yml
summary_line: 13 scopes · authorizationCode/clientCredentials
tags:
- Access Management
- Authentication
- Azure AD
- Entra
- Identity
- Identity Governance
- Microsoft
- Network Security
- Security
- Zero Trust
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
