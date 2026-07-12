---
authorization_urls:
- https://app.vssps.visualstudio.com/oauth2/authorize
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft publishes 42 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft API on a user''s behalf.


  Tokens are issued from https://app.vssps.visualstudio.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft
provider_slug: microsoft
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token
  name: oauth2
  source: openapi/microsoft-azure-devops-openapi.yml
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-azure-openai-openapi.yml
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-azure-rest-openapi.yml
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-dynamics-365-openapi.yml
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-entra-id-openapi.yml
- description: Microsoft identity platform OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-graph-openapi.yml
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-intune-openapi.yml
- description: OAuth 2.0 via Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-onedrive-openapi.yml
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-outlook-openapi.yml
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-power-bi-openapi.yml
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-power-platform-openapi.yml
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-sharepoint-openapi.yml
- description: OAuth 2.0 via Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-teams-openapi.yml
scope_count: 42
scope_names:
- Application.Read.All
- Application.ReadWrite.All
- Calendars.Read
- Calendars.ReadWrite
- Channel.ReadBasic.All
- ChannelMessage.Read.All
- ChannelMessage.Send
- Contacts.Read
- Contacts.ReadWrite
- DeviceManagementApps.Read.All
- DeviceManagementConfiguration.Read.All
- DeviceManagementManagedDevices.Read.All
- DeviceManagementManagedDevices.ReadWrite.All
- Directory.ReadWrite.All
- Files.Read
- Files.Read.All
- Files.ReadWrite
- Files.ReadWrite.All
- Group.Read.All
- Group.ReadWrite.All
- Mail.Read
- Mail.ReadWrite
- Mail.Send
- Sites.Read.All
- Sites.ReadWrite.All
- Team.Create
- Team.ReadBasic.All
- TeamMember.Read.All
- User.Read
- User.Read.All
- User.ReadWrite
- User.ReadWrite.All
- https://analysis.windows.net/powerbi/api/.default
- https://cognitiveservices.azure.com/.default
- https://graph.microsoft.com/.default
- https://management.azure.com/.default
- https://org.api.crm.dynamics.com/.default
- https://org.crm.dynamics.com/.default
- vso.build_execute
- vso.code
- vso.project
- vso.work_write
scopes:
- description: Read all applications
  flows:
  - authorizationCode
  scope: Application.Read.All
- description: Read and write all applications
  flows:
  - authorizationCode
  - clientCredentials
  scope: Application.ReadWrite.All
- description: Read user calendars
  flows:
  - authorizationCode
  scope: Calendars.Read
- description: Read and write user calendars
  flows:
  - authorizationCode
  scope: Calendars.ReadWrite
- description: Read channel names and descriptions
  flows:
  - authorizationCode
  scope: Channel.ReadBasic.All
- description: Read all channel messages
  flows:
  - authorizationCode
  scope: ChannelMessage.Read.All
- description: Send channel messages
  flows:
  - authorizationCode
  scope: ChannelMessage.Send
- description: Read user contacts
  flows:
  - authorizationCode
  scope: Contacts.Read
- description: Read and write user contacts
  flows:
  - authorizationCode
  scope: Contacts.ReadWrite
- description: Read mobile apps
  flows:
  - clientCredentials
  scope: DeviceManagementApps.Read.All
- description: Read device configurations
  flows:
  - clientCredentials
  scope: DeviceManagementConfiguration.Read.All
- description: Read managed devices
  flows:
  - clientCredentials
  scope: DeviceManagementManagedDevices.Read.All
- description: Read and write managed devices
  flows:
  - clientCredentials
  scope: DeviceManagementManagedDevices.ReadWrite.All
- description: Read and write directory data
  flows:
  - clientCredentials
  scope: Directory.ReadWrite.All
- description: Read user files
  flows:
  - authorizationCode
  scope: Files.Read
- description: Read all files that user can access
  flows:
  - authorizationCode
  scope: Files.Read.All
- description: Read and write user files
  flows:
  - authorizationCode
  scope: Files.ReadWrite
- description: Full access to all files
  flows:
  - authorizationCode
  scope: Files.ReadWrite.All
- description: Read all groups
  flows:
  - authorizationCode
  scope: Group.Read.All
- description: Read and write all groups
  flows:
  - authorizationCode
  scope: Group.ReadWrite.All
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Read and write user mail
  flows:
  - authorizationCode
  scope: Mail.ReadWrite
- description: Send mail as a user
  flows:
  - authorizationCode
  scope: Mail.Send
- description: Read items in all site collections
  flows:
  - authorizationCode
  scope: Sites.Read.All
- description: Read and write items in all site collections
  flows:
  - authorizationCode
  scope: Sites.ReadWrite.All
- description: Create teams
  flows:
  - authorizationCode
  scope: Team.Create
- description: Read the names and descriptions of teams
  flows:
  - authorizationCode
  scope: Team.ReadBasic.All
- description: Read team members
  flows:
  - authorizationCode
  scope: TeamMember.Read.All
- description: Read the signed-in user's profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Read all users' full profiles
  flows:
  - authorizationCode
  scope: User.Read.All
- description: Read and update the signed-in user's profile
  flows:
  - authorizationCode
  scope: User.ReadWrite
- description: Read and write all users' full profiles
  flows:
  - authorizationCode
  scope: User.ReadWrite.All
- description: Access Power BI
  flows:
  - authorizationCode
  scope: https://analysis.windows.net/powerbi/api/.default
- description: Access Azure OpenAI
  flows:
  - clientCredentials
  scope: https://cognitiveservices.azure.com/.default
- description: Access Microsoft Graph
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
- description: Access Azure Resource Manager
  flows:
  - clientCredentials
  scope: https://management.azure.com/.default
- description: Access Dynamics 365
  flows:
  - authorizationCode
  scope: https://org.api.crm.dynamics.com/.default
- description: Access Dataverse
  flows:
  - authorizationCode
  scope: https://org.crm.dynamics.com/.default
- description: Execute builds
  flows:
  - authorizationCode
  scope: vso.build_execute
- description: Read source code
  flows:
  - authorizationCode
  scope: vso.code
- description: Read projects
  flows:
  - authorizationCode
  scope: vso.project
- description: Read and write work items
  flows:
  - authorizationCode
  scope: vso.work_write
slug: microsoft-scopes
source_filename: microsoft-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-devops-openapi.yml, openapi/microsoft-azure-openai-openapi.yml,\n  openapi/microsoft-azure-rest-openapi.yml, openapi/microsoft-dynamics-365-openapi.yml, openapi/microsoft-entra-id-openapi.yml,\n  openapi/microsoft-graph-openapi.yml, openapi/microsoft-intune-openapi.yml, openapi/microsoft-onedrive-openapi.yml,\n  openapi/microsoft-outlook-openapi.yml, openapi/microsoft-power-bi-openapi.yml, openapi/microsoft-power-platform-openapi.yml,\n  openapi/microsoft-sharepoint-openapi.yml, openapi/microsoft-teams-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-azure-devops-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize\n    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-azure-openai-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-azure-rest-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-dynamics-365-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-entra-id-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-graph-openapi.yml\n  flows:\n  - flow: authorizationCode\n \
  \   authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: Microsoft identity platform OAuth 2.0 authorization\n- name: oauth2\n  source: openapi/microsoft-intune-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-onedrive-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 via Microsoft identity platform\n- name: oauth2\n  source: openapi/microsoft-outlook-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-power-bi-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-power-platform-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-sharepoint-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n\
  \    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\n- name: oauth2\n  source: openapi/microsoft-teams-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 via Microsoft identity platform\nscopes:\n- scope: Application.Read.All\n  description: Read all applications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n- scope: Application.ReadWrite.All\n  description: Read and write all applications\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n  - openapi/microsoft-graph-openapi.yml\n- scope: Calendars.Read\n  description: Read user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-outlook-openapi.yml\n\
  - scope: Calendars.ReadWrite\n  description: Read and write user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-outlook-openapi.yml\n- scope: Channel.ReadBasic.All\n  description: Read channel names and descriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-teams-openapi.yml\n- scope: ChannelMessage.Read.All\n  description: Read all channel messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-teams-openapi.yml\n- scope: ChannelMessage.Send\n  description: Send channel messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-teams-openapi.yml\n- scope: Contacts.Read\n  description: Read user contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-outlook-openapi.yml\n- scope: Contacts.ReadWrite\n  description:\
  \ Read and write user contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-outlook-openapi.yml\n- scope: DeviceManagementApps.Read.All\n  description: Read mobile apps\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-intune-openapi.yml\n- scope: DeviceManagementConfiguration.Read.All\n  description: Read device configurations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-intune-openapi.yml\n- scope: DeviceManagementManagedDevices.Read.All\n  description: Read managed devices\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-intune-openapi.yml\n- scope: DeviceManagementManagedDevices.ReadWrite.All\n  description: Read and write managed devices\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-intune-openapi.yml\n- scope: Directory.ReadWrite.All\n  description: Read and write directory data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n- scope:\
  \ Files.Read\n  description: Read user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-onedrive-openapi.yml\n- scope: Files.Read.All\n  description: Read all files that user can access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-onedrive-openapi.yml\n- scope: Files.ReadWrite\n  description: Read and write user files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-onedrive-openapi.yml\n- scope: Files.ReadWrite.All\n  description: Full access to all files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-onedrive-openapi.yml\n- scope: Group.Read.All\n  description: Read all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n- scope: Group.ReadWrite.All\n  description: Read and write all groups\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/microsoft-graph-openapi.yml\n- scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-outlook-openapi.yml\n- scope: Mail.ReadWrite\n  description: Read and write user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-outlook-openapi.yml\n- scope: Mail.Send\n  description: Send mail as a user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-outlook-openapi.yml\n- scope: Sites.Read.All\n  description: Read items in all site collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-sharepoint-openapi.yml\n- scope: Sites.ReadWrite.All\n  description: Read and write items in all site collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-sharepoint-openapi.yml\n- scope: Team.Create\n  description: Create teams\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-openapi.yml\n- scope: Team.ReadBasic.All\n  description: Read the names and descriptions of teams\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n  - openapi/microsoft-teams-openapi.yml\n- scope: TeamMember.Read.All\n  description: Read team members\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-openapi.yml\n- scope: User.Read\n  description: Read the signed-in user's profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n- scope: User.Read.All\n  description: Read all users' full profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n- scope: User.ReadWrite\n  description: Read and update the signed-in user's profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n- scope: User.ReadWrite.All\n  description: Read and write all users'\
  \ full profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n- scope: https://analysis.windows.net/powerbi/api/.default\n  description: Access Power BI\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-power-bi-openapi.yml\n- scope: https://cognitiveservices.azure.com/.default\n  description: Access Azure OpenAI\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-azure-openai-openapi.yml\n- scope: https://graph.microsoft.com/.default\n  description: Access Microsoft Graph\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n  - openapi/microsoft-graph-openapi.yml\n- scope: https://management.azure.com/.default\n  description: Access Azure Resource Manager\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-azure-rest-openapi.yml\n- scope: https://org.api.crm.dynamics.com/.default\n  description: Access Dynamics 365\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/microsoft-dynamics-365-openapi.yml\n- scope: https://org.crm.dynamics.com/.default\n  description: Access Dataverse\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-power-platform-openapi.yml\n- scope: vso.build_execute\n  description: Execute builds\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-azure-devops-openapi.yml\n- scope: vso.code\n  description: Read source code\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-azure-devops-openapi.yml\n- scope: vso.project\n  description: Read projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-azure-devops-openapi.yml\n- scope: vso.work_write\n  description: Read and write work items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-azure-devops-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/scopes/microsoft-scopes.yml
summary_line: 42 scopes · authorizationCode/clientCredentials
tags:
- Fortune 100
token_urls:
- https://app.vssps.visualstudio.com/oauth2/token
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
- https://login.microsoftonline.com/common/oauth2/v2.0/token
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
