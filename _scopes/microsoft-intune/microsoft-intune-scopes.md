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
name: Microsoft Intune Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Intune publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Intune API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Intune
provider_slug: microsoft-intune
schemes:
- description: OAuth 2.0 authorization using Azure Active Directory. Requires an active Intune license for the tenant.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-intune-openapi.yml
scope_count: 4
scope_names:
- DeviceManagementConfiguration.Read.All
- DeviceManagementConfiguration.ReadWrite.All
- DeviceManagementManagedDevices.Read.All
- DeviceManagementManagedDevices.ReadWrite.All
scopes:
- description: Read Microsoft Intune device configuration and policies
  flows:
  - authorizationCode
  scope: DeviceManagementConfiguration.Read.All
- description: Read and write Microsoft Intune device configuration and policies
  flows:
  - authorizationCode
  scope: DeviceManagementConfiguration.ReadWrite.All
- description: Read Microsoft Intune managed devices
  flows:
  - authorizationCode
  scope: DeviceManagementManagedDevices.Read.All
- description: Read and write Microsoft Intune managed devices
  flows:
  - authorizationCode
  scope: DeviceManagementManagedDevices.ReadWrite.All
slug: microsoft-intune-scopes
source_filename: microsoft-intune-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-intune-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-intune-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization using Azure Active Directory. Requires an active Intune\n    license for the tenant.\nscopes:\n- scope: DeviceManagementConfiguration.Read.All\n  description: Read Microsoft Intune device configuration and policies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-intune-openapi.yml\n- scope: DeviceManagementConfiguration.ReadWrite.All\n  description: Read and write Microsoft Intune device configuration and policies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-intune-openapi.yml\n- scope: DeviceManagementManagedDevices.Read.All\n  description:\
  \ Read Microsoft Intune managed devices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-intune-openapi.yml\n- scope: DeviceManagementManagedDevices.ReadWrite.All\n  description: Read and write Microsoft Intune managed devices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-intune-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-intune/refs/heads/main/scopes/microsoft-intune-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- App Protection
- Azure
- Compliance
- Device Configuration
- Endpoint Management
- Enrollment
- MAM
- MDM
- Microsoft Graph
- Mobile Application Management
- Mobile Device Management
- Security
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
