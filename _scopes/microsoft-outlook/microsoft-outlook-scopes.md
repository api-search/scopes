---
api_specs:
- filename: microsoft-graph-mail-api-openapi.yml
  format: yaml
  label: Microsoft Graph Mail API
  slug: microsoft-graph-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/openapi/microsoft-graph-mail-api-openapi.yml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Calendar API
  slug: microsoft-graph-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Contacts API
  slug: microsoft-graph-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Tasks API
  slug: microsoft-graph-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph People API
  slug: microsoft-graph-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Change Notifications API
  slug: microsoft-graph-change-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Focused Inbox API
  slug: microsoft-graph-focused-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Mail Rules API
  slug: microsoft-graph-mail-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Categories API
  slug: microsoft-graph-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Outlook Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Outlook publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Outlook API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schemes:
- description: Microsoft identity platform OAuth 2.0 authorization. Supports delegated (user) and application permissions.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-graph-mail-api-openapi.yml
scope_count: 6
scope_names:
- Mail.Read
- Mail.Read.Shared
- Mail.ReadBasic
- Mail.ReadWrite
- Mail.ReadWrite.Shared
- Mail.Send
scopes:
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Read mail in shared mailboxes
  flows:
  - authorizationCode
  scope: Mail.Read.Shared
- description: Read user basic mail
  flows:
  - authorizationCode
  scope: Mail.ReadBasic
- description: Read and write access to user mail
  flows:
  - authorizationCode
  scope: Mail.ReadWrite
- description: Read and write mail in shared mailboxes
  flows:
  - authorizationCode
  scope: Mail.ReadWrite.Shared
- description: Send mail as a user
  flows:
  - authorizationCode
  scope: Mail.Send
slug: microsoft-outlook-scopes
source_filename: microsoft-outlook-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-graph-mail-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-graph-mail-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft identity platform OAuth 2.0 authorization. Supports delegated (user)\n    and application permissions.\nscopes:\n- scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-mail-api-openapi.yml\n- scope: Mail.Read.Shared\n  description: Read mail in shared mailboxes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-mail-api-openapi.yml\n- scope: Mail.ReadBasic\n  description: Read user basic mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-mail-api-openapi.yml\n-\
  \ scope: Mail.ReadWrite\n  description: Read and write access to user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-mail-api-openapi.yml\n- scope: Mail.ReadWrite.Shared\n  description: Read and write mail in shared mailboxes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-mail-api-openapi.yml\n- scope: Mail.Send\n  description: Send mail as a user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-graph-mail-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/scopes/microsoft-outlook-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
