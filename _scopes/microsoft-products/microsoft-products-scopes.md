---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: azure-rest-api-specs
  format: yaml
  label: Azure REST API
  slug: azure-rest-api
  spec_type: OpenAPI
  url: https://github.com/Azure/azure-rest-api-specs
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Products Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Products publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Products API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Products
provider_slug: microsoft-products
schemes:
- description: Microsoft Entra ID (Azure AD) OAuth 2.0. Use the authorization code, client credentials, or device code flow depending on the scenario.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-products-openapi.yml
scope_count: 7
scope_names:
- ChannelMessage.Send
- Files.Read
- Files.ReadWrite
- Mail.Read
- Mail.Send
- Team.ReadBasic.All
- User.Read
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
slug: microsoft-products-scopes
source_filename: microsoft-products-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-products-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-products-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0. Use the authorization code, client credentials,\n    or device code flow depending on the scenario.\nscopes:\n- scope: ChannelMessage.Send\n  description: Send channel messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-products-openapi.yml\n- scope: Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-products-openapi.yml\n- scope: Files.ReadWrite\n  description: Read and write user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-products-openapi.yml\n\
  - scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-products-openapi.yml\n- scope: Mail.Send\n  description: Send mail as user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-products-openapi.yml\n- scope: Team.ReadBasic.All\n  description: Read basic team info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-products-openapi.yml\n- scope: User.Read\n  description: Sign in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-products-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-products/refs/heads/main/scopes/microsoft-products-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Cloud
- Enterprise
- Microsoft
- Productivity
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
