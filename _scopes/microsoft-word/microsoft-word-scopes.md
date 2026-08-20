---
api_specs:
- filename: microsoft-word-body-api-openapi.yml
  format: yaml
  label: Microsoft Word Body API
  slug: microsoft-word-body-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-body-api-openapi.yml
- filename: microsoft-word-checkout-api-openapi.yml
  format: yaml
  label: Microsoft Word Checkout API
  slug: microsoft-word-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-checkout-api-openapi.yml
- filename: microsoft-word-comments-api-openapi.yml
  format: yaml
  label: Microsoft Word Comments API
  slug: microsoft-word-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-comments-api-openapi.yml
- filename: microsoft-word-content-api-openapi.yml
  format: yaml
  label: Microsoft Word Content API
  slug: microsoft-word-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-content-api-openapi.yml
- filename: microsoft-word-content-controls-api-openapi.yml
  format: yaml
  label: Microsoft Word Content Controls API
  slug: microsoft-word-content-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-content-controls-api-openapi.yml
- filename: microsoft-word-documents-api-openapi.yml
  format: yaml
  label: Microsoft Word Documents API
  slug: microsoft-word-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-documents-api-openapi.yml
- filename: microsoft-word-drive-items-api-openapi.yml
  format: yaml
  label: Microsoft Word Drive Items API
  slug: microsoft-word-drive-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-drive-items-api-openapi.yml
- filename: microsoft-word-headers-and-footers-api-openapi.yml
  format: yaml
  label: Microsoft Word Headers And Footers API
  slug: microsoft-word-headers-and-footers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-headers-and-footers-api-openapi.yml
- filename: microsoft-word-images-api-openapi.yml
  format: yaml
  label: Microsoft Word Images API
  slug: microsoft-word-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-images-api-openapi.yml
- filename: microsoft-word-paragraphs-api-openapi.yml
  format: yaml
  label: Microsoft Word Paragraphs API
  slug: microsoft-word-paragraphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-paragraphs-api-openapi.yml
- filename: microsoft-word-permissions-api-openapi.yml
  format: yaml
  label: Microsoft Word Permissions API
  slug: microsoft-word-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-permissions-api-openapi.yml
- filename: microsoft-word-properties-api-openapi.yml
  format: yaml
  label: Microsoft Word Properties API
  slug: microsoft-word-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-properties-api-openapi.yml
- filename: microsoft-word-search-api-openapi.yml
  format: yaml
  label: Microsoft Word Search API
  slug: microsoft-word-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-search-api-openapi.yml
- filename: microsoft-word-sections-api-openapi.yml
  format: yaml
  label: Microsoft Word Sections API
  slug: microsoft-word-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-sections-api-openapi.yml
- filename: microsoft-word-styles-api-openapi.yml
  format: yaml
  label: Microsoft Word Styles API
  slug: microsoft-word-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-styles-api-openapi.yml
- filename: microsoft-word-tables-api-openapi.yml
  format: yaml
  label: Microsoft Word Tables API
  slug: microsoft-word-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-tables-api-openapi.yml
- filename: microsoft-word-thumbnails-api-openapi.yml
  format: yaml
  label: Microsoft Word Thumbnails API
  slug: microsoft-word-thumbnails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-thumbnails-api-openapi.yml
- filename: microsoft-word-versions-api-openapi.yml
  format: yaml
  label: Microsoft Word Versions API
  slug: microsoft-word-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-versions-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: https://learn.microsoft.com/en-us/graph/permissions-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Word Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Word publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Word API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Word
provider_slug: microsoft-word
schemes:
- description: OAuth 2.0 authorization code flow with Microsoft Identity Platform.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-word-graph-api.yaml
- description: OAuth 2.0 via Microsoft Identity Platform for Office Add-ins.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-word-javascript-api.yaml
scope_count: 8
scope_names:
- Files.Read
- Files.Read.All
- Files.ReadWrite
- Files.ReadWrite.All
- Files.ReadWrite.AppFolder
- Sites.Read.All
- Sites.ReadWrite.All
- User.Read
scopes:
- description: Read the signed-in user's files.
  flows:
  - authorizationCode
  scope: Files.Read
- description: Read all files the signed-in user can access.
  flows:
  - authorizationCode
  scope: Files.Read.All
- description: Read and write the signed-in user's files.
  flows:
  - authorizationCode
  scope: Files.ReadWrite
- description: Read and write all files the signed-in user can access.
  flows:
  - authorizationCode
  scope: Files.ReadWrite.All
- description: Read and write files in the application's dedicated folder.
  flows:
  - authorizationCode
  scope: Files.ReadWrite.AppFolder
- description: Read items in all SharePoint site collections the user can access (SharePoint document libraries).
  flows:
  - authorizationCode
  scope: Sites.Read.All
- description: Read and write items in all SharePoint site collections (admin consent typically required).
  flows:
  - authorizationCode
  scope: Sites.ReadWrite.All
- description: Sign in and read the signed-in user's profile (baseline scope requested at login).
  flows:
  - authorizationCode
  scope: User.Read
slug: microsoft-word-scopes
source_filename: microsoft-word-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/microsoft-word-graph-api.yaml, openapi/microsoft-word-javascript-api.yaml\ndocs: https://learn.microsoft.com/en-us/graph/permissions-reference\nnotes: >-\n  Microsoft Graph permissions (scopes) for the Word document surface are the Files.*\n  and Sites.* permission families. Each exists as a delegated and an application\n  permission; .All variants and Sites.* permissions typically require admin consent.\n  Scopes below extend the four declared in the OpenAPI with the additional documented\n  file/site permissions that Word-in-OneDrive/SharePoint operations use.\nschemes:\n- name: oauth2\n  source: openapi/microsoft-word-graph-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization code flow with Microsoft Identity Platform.\n\
  - name: oauth2\n  source: openapi/microsoft-word-javascript-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 via Microsoft Identity Platform for Office Add-ins.\nscopes:\n- scope: Files.Read\n  description: Read the signed-in user's files.\n  flows: [authorizationCode]\n  sources: [openapi/microsoft-word-graph-api.yaml]\n- scope: Files.Read.All\n  description: Read all files the signed-in user can access.\n  flows: [authorizationCode]\n  sources: [openapi/microsoft-word-graph-api.yaml]\n- scope: Files.ReadWrite\n  description: Read and write the signed-in user's files.\n  flows: [authorizationCode]\n  sources: [openapi/microsoft-word-graph-api.yaml, openapi/microsoft-word-javascript-api.yaml]\n- scope: Files.ReadWrite.All\n  description: Read and write all files the signed-in user can access.\n  flows: [authorizationCode]\n\
  \  sources: [openapi/microsoft-word-graph-api.yaml]\n- scope: Files.ReadWrite.AppFolder\n  description: Read and write files in the application's dedicated folder.\n  flows: [authorizationCode]\n  sources: [docs]\n- scope: Sites.Read.All\n  description: Read items in all SharePoint site collections the user can access (SharePoint document libraries).\n  flows: [authorizationCode]\n  sources: [docs]\n- scope: Sites.ReadWrite.All\n  description: Read and write items in all SharePoint site collections (admin consent typically required).\n  flows: [authorizationCode]\n  sources: [docs]\n- scope: User.Read\n  description: Sign in and read the signed-in user's profile (baseline scope requested at login).\n  flows: [authorizationCode]\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/scopes/microsoft-word-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Documents
- Microsoft-365
- Office
- Productivity
- Word Processing
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
