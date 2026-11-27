---
api_specs:
- filename: sharepoint-admin-edge-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Admin.edge API
  slug: sharepoint-admin-edge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-admin-edge-api-openapi.yml
- filename: sharepoint-groups-group-functions-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Groups.group.Functions API
  slug: sharepoint-groups-group-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-groups-group-functions-api-openapi.yml
- filename: sharepoint-groups-site-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Groups.site API
  slug: sharepoint-groups-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-groups-site-api-openapi.yml
- filename: sharepoint-sites-baseitem-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.base Item API
  slug: sharepoint-sites-baseitem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-baseitem-api-openapi.yml
- filename: sharepoint-sites-basesitepage-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.base Site Page API
  slug: sharepoint-sites-basesitepage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-basesitepage-api-openapi.yml
- filename: sharepoint-sites-columndefinition-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.column Definition API
  slug: sharepoint-sites-columndefinition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-columndefinition-api-openapi.yml
- filename: sharepoint-sites-contenttype-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.content Type API
  slug: sharepoint-sites-contenttype-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-contenttype-api-openapi.yml
- filename: sharepoint-sites-drive-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.drive API
  slug: sharepoint-sites-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-drive-api-openapi.yml
- filename: sharepoint-sites-itemanalytics-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.item Analytics API
  slug: sharepoint-sites-itemanalytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-itemanalytics-api-openapi.yml
- filename: sharepoint-sites-list-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.list API
  slug: sharepoint-sites-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-list-api-openapi.yml
- filename: sharepoint-sites-onenote-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.onenote API
  slug: sharepoint-sites-onenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-onenote-api-openapi.yml
- filename: sharepoint-sites-permission-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.permission API
  slug: sharepoint-sites-permission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-permission-api-openapi.yml
- filename: sharepoint-sites-richlongrunningoperation-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.rich Long Running Operation API
  slug: sharepoint-sites-richlongrunningoperation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-richlongrunningoperation-api-openapi.yml
- filename: sharepoint-sites-site-actions-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.site.Actions API
  slug: sharepoint-sites-site-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-site-actions-api-openapi.yml
- filename: sharepoint-sites-site-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.site API
  slug: sharepoint-sites-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-site-api-openapi.yml
- filename: sharepoint-sites-site-functions-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.site.Functions API
  slug: sharepoint-sites-site-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-site-functions-api-openapi.yml
- filename: sharepoint-sites-store-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.store API
  slug: sharepoint-sites-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-store-api-openapi.yml
- filename: sharepoint-sites-user-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.user API
  slug: sharepoint-sites-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-user-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
description: ''
docs: https://learn.microsoft.com/en-us/graph/permissions-reference#sites-permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft SharePoint Scopes
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
source_yaml_url: https://artifacts.apis.io/sharepoint/scopes/sharepoint-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
token_bound: false
token_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
