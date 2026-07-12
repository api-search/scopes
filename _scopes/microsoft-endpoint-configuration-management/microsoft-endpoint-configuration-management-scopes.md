---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Endpoint Configuration Management Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Endpoint Configuration Management publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Endpoint Configuration Management API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Endpoint Configuration Management
provider_slug: microsoft-endpoint-configuration-management
schemes:
- description: OAuth 2.0 via Azure AD for cloud management gateway access.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml
- description: OAuth 2.0 via Microsoft Entra ID. Requires Intune service administrator role or role-based access to the Intune data warehouse resource.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml
scope_count: 7
scope_names:
- DeviceManagementApps.Read.All
- DeviceManagementApps.ReadWrite.All
- DeviceManagementConfiguration.Read.All
- DeviceManagementConfiguration.ReadWrite.All
- DeviceManagementManagedDevices.Read.All
- DeviceManagementManagedDevices.ReadWrite.All
- https://api.manage.microsoft.com/.default
scopes:
- description: Read app management data
  flows:
  - authorizationCode
  scope: DeviceManagementApps.Read.All
- description: Read and write app management data
  flows:
  - authorizationCode
  scope: DeviceManagementApps.ReadWrite.All
- description: Read device configurations
  flows:
  - authorizationCode
  scope: DeviceManagementConfiguration.Read.All
- description: Read and write device configurations
  flows:
  - authorizationCode
  scope: DeviceManagementConfiguration.ReadWrite.All
- description: Read managed devices
  flows:
  - authorizationCode
  scope: DeviceManagementManagedDevices.Read.All
- description: Read and write managed devices
  flows:
  - authorizationCode
  scope: DeviceManagementManagedDevices.ReadWrite.All
- description: Access Intune Data Warehouse
  flows:
  - authorizationCode
  scope: https://api.manage.microsoft.com/.default
slug: microsoft-endpoint-configuration-management-scopes
source_filename: microsoft-endpoint-configuration-management-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml,\n  openapi/microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml,\n  openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml, openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 via Azure AD for cloud management gateway access.\n- name: oauth2\n  source: openapi/microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n\
  \    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 via Microsoft Entra ID. Requires Intune service administrator role\n    or role-based access to the Intune data warehouse resource.\n- name: oauth2\n  source: openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\nscopes:\n- scope: DeviceManagementApps.Read.All\n  description: Read app management data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml\n\
  \  - openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\n- scope: DeviceManagementApps.ReadWrite.All\n  description: Read and write app management data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml\n  - openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\n- scope: DeviceManagementConfiguration.Read.All\n  description: Read device configurations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml\n  - openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\n- scope: DeviceManagementConfiguration.ReadWrite.All\n  description: Read and write device configurations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml\n  - openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\n\
  - scope: DeviceManagementManagedDevices.Read.All\n  description: Read managed devices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml\n  - openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\n- scope: DeviceManagementManagedDevices.ReadWrite.All\n  description: Read and write managed devices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml\n  - openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\n- scope: https://api.manage.microsoft.com/.default\n  description: Access Intune Data Warehouse\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/scopes/microsoft-endpoint-configuration-management-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Compliance
- Configuration Management
- Device Management
- Endpoint Management
- Mobile Device Management
- Patch Management
- Software Deployment
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
