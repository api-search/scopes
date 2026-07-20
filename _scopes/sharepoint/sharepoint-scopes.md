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
docs: https://learn.microsoft.com/en-us/graph/permissions-reference#sites-permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sharepoint Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft SharePoint publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft SharePoint API on a user''s behalf.


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
scope_count: 5
scope_names:
- Sites.FullControl.All
- Sites.Manage.All
- Sites.Read.All
- Sites.ReadWrite.All
- Sites.Selected
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
- description: Access only to specific SharePoint site collections granted explicitly by an admin (per-site authorization).
  flows:
  - authorizationCode
  scope: Sites.Selected
slug: sharepoint-scopes
source_filename: sharepoint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/sharepoint-rest-api.yaml\ndocs: https://learn.microsoft.com/en-us/graph/permissions-reference#sites-permissions\nnotes: >-\n  SharePoint permissions are Microsoft Graph / Microsoft Entra scopes. The Sites.* set below\n  is documented in the Microsoft Graph permissions reference. Both delegated and application\n  permission variants exist; Sites.Selected additionally supports per-site granular grants.\nschemes:\n- name: oauth2\n  source: openapi/sharepoint-rest-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: OAuth 2.0 via Azure AD / Microsoft Identity Platform.\nscopes:\n- scope: Sites.FullControl.All\n  description: Full control of all site collections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n- scope:\
  \ Sites.Manage.All\n  description: Create, edit, and delete items and lists.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n- scope: Sites.Read.All\n  description: Read all site collections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n- scope: Sites.ReadWrite.All\n  description: Read and write all site collections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n- scope: Sites.Selected\n  description: Access only to specific SharePoint site collections granted explicitly by an admin (per-site authorization).\n  flows:\n  - authorizationCode\n  sources:\n  - https://learn.microsoft.com/en-us/graph/permissions-reference#sites-permissions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/scopes/sharepoint-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
token_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
