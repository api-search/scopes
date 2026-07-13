---
api_specs:
- filename: powerpoint-openapi.yml
  format: yaml
  label: PowerPoint via Microsoft Graph
  slug: powerpoint-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerpoint/refs/heads/main/openapi/powerpoint-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Powerpoint Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PowerPoint publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PowerPoint API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PowerPoint
provider_slug: powerpoint
schemes:
- description: 'Microsoft Graph uses Microsoft Entra ID (Azure AD) OAuth 2.0.

    Apps require delegated or application permissions such as Files.Read,

    Files.ReadWrite, Sites.Read.All, or Sites.ReadWrite.All.'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: OAuth2
  source: openapi/powerpoint-openapi.yml
scope_count: 4
scope_names:
- Files.Read
- Files.ReadWrite
- Sites.Read.All
- Sites.ReadWrite.All
scopes:
- description: Read user files
  flows:
  - authorizationCode
  scope: Files.Read
- description: Read and write user files
  flows:
  - authorizationCode
  scope: Files.ReadWrite
- description: Read items in all site collections
  flows:
  - authorizationCode
  scope: Sites.Read.All
- description: Read and write items in all site collections
  flows:
  - authorizationCode
  scope: Sites.ReadWrite.All
slug: powerpoint-scopes
source_filename: powerpoint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/powerpoint-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/powerpoint-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: |-\n    Microsoft Graph uses Microsoft Entra ID (Azure AD) OAuth 2.0.\n    Apps require delegated or application permissions such as Files.Read,\n    Files.ReadWrite, Sites.Read.All, or Sites.ReadWrite.All.\nscopes:\n- scope: Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/powerpoint-openapi.yml\n- scope: Files.ReadWrite\n  description: Read and write user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/powerpoint-openapi.yml\n- scope: Sites.Read.All\n  description: Read items in all site collections\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/powerpoint-openapi.yml\n- scope: Sites.ReadWrite.All\n  description: Read and write items in all site collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/powerpoint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerpoint/refs/heads/main/scopes/powerpoint-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Microsoft Office
- Microsoft 365
- Presentations
- Productivity
- Documents
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
