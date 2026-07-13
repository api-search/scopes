---
api_specs:
- filename: active-directory-users-openapi.yaml
  format: yaml
  label: Microsoft Graph Users API
  slug: microsoft-graph-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-users-openapi.yaml
- filename: active-directory-groups-openapi.yaml
  format: yaml
  label: Microsoft Graph Groups API
  slug: microsoft-graph-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-groups-openapi.yaml
- filename: active-directory-applications-openapi.yaml
  format: yaml
  label: Microsoft Graph Applications and Service Principals API
  slug: microsoft-graph-applications-and-service-principals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-applications-openapi.yaml
authorization_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Active Directory Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Active Directory publishes 11 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Active Directory API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Active Directory
provider_slug: active-directory
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/active-directory-applications-openapi.yaml
- description: OAuth2 with Microsoft identity platform (Azure AD)
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/active-directory-groups-openapi.yaml
- description: OAuth2 with Microsoft identity platform (Azure AD)
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/active-directory-users-openapi.yaml
scope_count: 11
scope_names:
- Application.Read.All
- Application.ReadWrite.All
- Directory.Read.All
- Directory.ReadWrite.All
- Group.Read.All
- Group.ReadWrite.All
- User.Read
- User.Read.All
- User.ReadBasic.All
- User.ReadWrite
- User.ReadWrite.All
scopes:
- description: Read all applications
  flows:
  - authorizationCode
  - clientCredentials
  scope: Application.Read.All
- description: Read and write all applications
  flows:
  - authorizationCode
  - clientCredentials
  scope: Application.ReadWrite.All
- description: Read directory data
  flows:
  - authorizationCode
  - clientCredentials
  scope: Directory.Read.All
- description: Read and write directory data
  flows:
  - authorizationCode
  - clientCredentials
  scope: Directory.ReadWrite.All
- description: Read all groups
  flows:
  - authorizationCode
  - clientCredentials
  scope: Group.Read.All
- description: Read and write all groups
  flows:
  - authorizationCode
  - clientCredentials
  scope: Group.ReadWrite.All
- description: Read signed-in user's profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Read all users' full profiles
  flows:
  - authorizationCode
  - clientCredentials
  scope: User.Read.All
- description: Read all users' basic profiles
  flows:
  - authorizationCode
  scope: User.ReadBasic.All
- description: Read and write signed-in user's profile
  flows:
  - authorizationCode
  scope: User.ReadWrite
- description: Read and write all users' full profiles
  flows:
  - authorizationCode
  - clientCredentials
  scope: User.ReadWrite.All
slug: active-directory-scopes
source_filename: active-directory-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/active-directory-applications-openapi.yaml, openapi/active-directory-groups-openapi.yaml,\n  openapi/active-directory-users-openapi.yaml\nschemes:\n- name: oauth2\n  source: openapi/active-directory-applications-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/active-directory-groups-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: OAuth2\
  \ with Microsoft identity platform (Azure AD)\n- name: oauth2\n  source: openapi/active-directory-users-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: OAuth2 with Microsoft identity platform (Azure AD)\nscopes:\n- scope: Application.Read.All\n  description: Read all applications\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/active-directory-applications-openapi.yaml\n- scope: Application.ReadWrite.All\n  description: Read and write all applications\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/active-directory-applications-openapi.yaml\n- scope: Directory.Read.All\n  description: Read directory data\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/active-directory-applications-openapi.yaml\n  - openapi/active-directory-groups-openapi.yaml\n  - openapi/active-directory-users-openapi.yaml\n- scope: Directory.ReadWrite.All\n  description: Read and write directory data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/active-directory-groups-openapi.yaml\n  - openapi/active-directory-users-openapi.yaml\n- scope: Group.Read.All\n  description: Read all groups\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/active-directory-groups-openapi.yaml\n- scope: Group.ReadWrite.All\n  description: Read and write all groups\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/active-directory-groups-openapi.yaml\n- scope: User.Read\n  description: Read signed-in user's profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/active-directory-users-openapi.yaml\n- scope: User.Read.All\n  description:\
  \ Read all users' full profiles\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/active-directory-users-openapi.yaml\n- scope: User.ReadBasic.All\n  description: Read all users' basic profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/active-directory-users-openapi.yaml\n- scope: User.ReadWrite\n  description: Read and write signed-in user's profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/active-directory-users-openapi.yaml\n- scope: User.ReadWrite.All\n  description: Read and write all users' full profiles\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/active-directory-users-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/scopes/active-directory-scopes.yml
summary_line: 11 scopes · authorizationCode/clientCredentials
tags:
- Active Directory
- Authentication
- Authorization
- Directory Services
- Identity Management
- Microsoft Entra
- Zero Trust
token_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
