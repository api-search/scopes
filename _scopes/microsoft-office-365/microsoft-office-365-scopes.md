---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/openapi.yaml
- filename: mail.yaml
  format: yaml
  label: Outlook Mail API
  slug: outlook-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/mail.yaml
- filename: calendar.yaml
  format: yaml
  label: Outlook Calendar API
  slug: outlook-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/calendar.yaml
- filename: files.yaml
  format: yaml
  label: OneDrive API
  slug: onedrive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/files.yaml
- filename: sites.yaml
  format: yaml
  label: SharePoint API
  slug: sharepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/sites.yaml
- filename: teams.yaml
  format: yaml
  label: Microsoft Teams API
  slug: microsoft-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/teams.yaml
- filename: users.yaml
  format: yaml
  label: Office 365 Users API
  slug: office-365-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/users.yaml
- filename: planner.yaml
  format: yaml
  label: Planner API
  slug: planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/planner.yaml
- filename: microsoft-graph-api-openapi.yml
  format: yaml
  label: Office 365 Groups API
  slug: office-365-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/openapi/microsoft-graph-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Office 365 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Office 365 publishes 18 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Office 365 API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schemes:
- description: Microsoft identity platform OAuth 2.0 authorization. Supports delegated (user) and application-only permissions. Microsoft Graph uses scopes to control access to resources.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-graph-api-openapi.yml
scope_count: 18
scope_names:
- Calendars.Read
- Calendars.ReadWrite
- Directory.Read.All
- Directory.ReadWrite.All
- Group.Read.All
- Group.ReadWrite.All
- GroupMember.Read.All
- GroupMember.ReadWrite.All
- Mail.Read
- Mail.ReadBasic
- Mail.ReadWrite
- Mail.Send
- User.Read
- User.Read.All
- User.ReadBasic.All
- User.ReadWrite
- User.ReadWrite.All
- https://graph.microsoft.com/.default
scopes:
- description: Read user calendars
  flows:
  - authorizationCode
  scope: Calendars.Read
- description: Read and write user calendars
  flows:
  - authorizationCode
  scope: Calendars.ReadWrite
- description: Read directory data
  flows:
  - authorizationCode
  scope: Directory.Read.All
- description: Read and write directory data
  flows:
  - authorizationCode
  scope: Directory.ReadWrite.All
- description: Read all groups
  flows:
  - authorizationCode
  scope: Group.Read.All
- description: Read and write all groups
  flows:
  - authorizationCode
  scope: Group.ReadWrite.All
- description: Read all group memberships
  flows:
  - authorizationCode
  scope: GroupMember.Read.All
- description: Read and write all group memberships
  flows:
  - authorizationCode
  scope: GroupMember.ReadWrite.All
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Read user basic mail
  flows:
  - authorizationCode
  scope: Mail.ReadBasic
- description: Read and write user mail
  flows:
  - authorizationCode
  scope: Mail.ReadWrite
- description: Send mail as a user
  flows:
  - authorizationCode
  scope: Mail.Send
- description: Sign in and read user profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Read all users' full profiles
  flows:
  - authorizationCode
  scope: User.Read.All
- description: Read all users' basic profiles
  flows:
  - authorizationCode
  scope: User.ReadBasic.All
- description: Read and update your profile
  flows:
  - authorizationCode
  scope: User.ReadWrite
- description: Read and write all users' full profiles
  flows:
  - authorizationCode
  scope: User.ReadWrite.All
- description: Default scope for application permissions
  flows:
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: microsoft-office-365-scopes
source_filename: microsoft-office-365-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-graph-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-graph-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: Microsoft identity platform OAuth 2.0 authorization. Supports delegated (user)\n    and application-only permissions. Microsoft Graph uses scopes to control access to resources.\nscopes:\n- scope: Calendars.Read\n  description: Read user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: Calendars.ReadWrite\n  description: Read and write user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n\
  - scope: Directory.Read.All\n  description: Read directory data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: Directory.ReadWrite.All\n  description: Read and write directory data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: Group.Read.All\n  description: Read all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: Group.ReadWrite.All\n  description: Read and write all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: GroupMember.Read.All\n  description: Read all group memberships\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: GroupMember.ReadWrite.All\n  description: Read and write all group memberships\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: Mail.Read\n  description:\
  \ Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: Mail.ReadBasic\n  description: Read user basic mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: Mail.ReadWrite\n  description: Read and write user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: Mail.Send\n  description: Send mail as a user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: User.Read\n  description: Sign in and read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: User.Read.All\n  description: Read all users' full profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: User.ReadBasic.All\n  description: Read all users' basic profiles\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/microsoft-graph-api-openapi.yml\n- scope: User.ReadWrite\n  description: Read and update your profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: User.ReadWrite.All\n  description: Read and write all users' full profiles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- scope: https://graph.microsoft.com/.default\n  description: Default scope for application permissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/scopes/microsoft-office-365-scopes.yml
summary_line: 18 scopes · authorizationCode/clientCredentials
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
