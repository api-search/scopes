---
api_specs:
- filename: sharepoint-rest-openapi.json
  format: json
  label: SharePoint REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://example.com/sharepoint-rest-openapi.json
- filename: graph-sharepoint-openapi.json
  format: json
  label: Microsoft Graph API (SharePoint)
  slug: graph-api-sharepoint
  spec_type: OpenAPI
  url: https://example.com/graph-sharepoint-openapi.json
authorization_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Sharepoint Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft SharePoint publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft SharePoint API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schemes:
- description: OAuth 2.0 via Azure AD / Microsoft Identity Platform.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/sharepoint-rest-api.yaml
scope_count: 4
scope_names:
- Sites.FullControl.All
- Sites.Manage.All
- Sites.Read.All
- Sites.ReadWrite.All
scopes:
- description: Full control of all site collections.
  flows:
  - authorizationCode
  scope: Sites.FullControl.All
- description: Create, edit, and delete items and lists.
  flows:
  - authorizationCode
  scope: Sites.Manage.All
- description: Read all site collections.
  flows:
  - authorizationCode
  scope: Sites.Read.All
- description: Read and write all site collections.
  flows:
  - authorizationCode
  scope: Sites.ReadWrite.All
slug: sharepoint-scopes
source_filename: sharepoint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sharepoint-rest-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/sharepoint-rest-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: OAuth 2.0 via Azure AD / Microsoft Identity Platform.\nscopes:\n- scope: Sites.FullControl.All\n  description: Full control of all site collections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n- scope: Sites.Manage.All\n  description: Create, edit, and delete items and lists.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n- scope: Sites.Read.All\n  description: Read all site collections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n- scope: Sites.ReadWrite.All\n  description: Read and write all\
  \ site collections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/scopes/sharepoint-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
token_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
