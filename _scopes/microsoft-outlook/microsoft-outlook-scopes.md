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
docs: https://learn.microsoft.com/en-us/graph/permissions-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Outlook Scopes
name_suffix: OAuth Scopes
note: Microsoft identity platform (Entra ID) OAuth 2.0 permissions. Scopes exist in delegated (user-consented) and application (app-only) forms; the strings below are the delegated names. The OpenAPI declares only the mail subset — the wider Outlook surface (calendar, contacts, tasks, mailbox settings) is enriched from the Microsoft Graph permissions reference.
overview: 'Microsoft Outlook publishes 20 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Outlook API on a user''s behalf.


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
scope_count: 20
scope_names:
- Mail.Read
- Mail.ReadBasic
- Mail.Read.Shared
- Mail.ReadWrite
- Mail.ReadWrite.Shared
- Mail.Send
- Mail.Send.Shared
- MailboxSettings.Read
- MailboxSettings.ReadWrite
- MailboxFolder.Read
- MailboxFolder.ReadWrite
- Calendars.Read
- Calendars.ReadWrite
- Contacts.Read
- Contacts.ReadWrite
- Tasks.Read
- Tasks.ReadWrite
- People.Read
- User.Read
- offline_access
scopes:
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Read user basic mail (no body/attachments)
  flows:
  - authorizationCode
  scope: Mail.ReadBasic
- description: Read mail in shared mailboxes
  flows:
  - authorizationCode
  scope: Mail.Read.Shared
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
- description: Send mail on behalf of others
  flows:
  - authorizationCode
  scope: Mail.Send.Shared
- description: Read user mailbox settings (automatic replies
  flows:
  - authorizationCode
  scope: MailboxSettings.Read
- description: Read and write user mailbox settings
  flows:
  - authorizationCode
  scope: MailboxSettings.ReadWrite
- description: Read user mail folders
  flows:
  - authorizationCode
  scope: MailboxFolder.Read
- description: Read and write user mail folders
  flows:
  - authorizationCode
  scope: MailboxFolder.ReadWrite
- description: Read user calendars
  flows:
  - authorizationCode
  scope: Calendars.Read
- description: Read and write user calendars
  flows:
  - authorizationCode
  scope: Calendars.ReadWrite
- description: Read user contacts
  flows:
  - authorizationCode
  scope: Contacts.Read
- description: Read and write user contacts
  flows:
  - authorizationCode
  scope: Contacts.ReadWrite
- description: Read user tasks and to-do lists
  flows:
  - authorizationCode
  scope: Tasks.Read
- description: Create
  flows:
  - authorizationCode
  scope: Tasks.ReadWrite
- description: Read the signed-in user's relevant people list
  flows:
  - authorizationCode
  scope: People.Read
- description: Sign in and read the user's profile
  flows:
  - authorizationCode
  scope: User.Read
- description: Maintain access via refresh tokens
  flows:
  - authorizationCode
  scope: offline_access
slug: microsoft-outlook-scopes
source_filename: microsoft-outlook-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/microsoft-graph-mail-api-openapi.yml\ndocs: https://learn.microsoft.com/en-us/graph/permissions-reference\nnote: >-\n  Microsoft identity platform (Entra ID) OAuth 2.0 permissions. Scopes exist in\n  delegated (user-consented) and application (app-only) forms; the strings below\n  are the delegated names. The OpenAPI declares only the mail subset — the wider\n  Outlook surface (calendar, contacts, tasks, mailbox settings) is enriched from\n  the Microsoft Graph permissions reference.\nschemes:\n  - name: oauth2\n    source: openapi/microsoft-graph-mail-api-openapi.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n        tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    description: Microsoft identity platform OAuth 2.0 authorization. Supports delegated (user) and application permissions.\nscopes:\n  - {scope:\
  \ Mail.Read, description: Read user mail, flows: [authorizationCode], sources: [openapi/microsoft-graph-mail-api-openapi.yml]}\n  - {scope: Mail.ReadBasic, description: Read user basic mail (no body/attachments), flows: [authorizationCode], sources: [openapi/microsoft-graph-mail-api-openapi.yml]}\n  - {scope: Mail.Read.Shared, description: Read mail in shared mailboxes, flows: [authorizationCode], sources: [openapi/microsoft-graph-mail-api-openapi.yml]}\n  - {scope: Mail.ReadWrite, description: Read and write access to user mail, flows: [authorizationCode], sources: [openapi/microsoft-graph-mail-api-openapi.yml]}\n  - {scope: Mail.ReadWrite.Shared, description: Read and write mail in shared mailboxes, flows: [authorizationCode], sources: [openapi/microsoft-graph-mail-api-openapi.yml]}\n  - {scope: Mail.Send, description: Send mail as a user, flows: [authorizationCode], sources: [openapi/microsoft-graph-mail-api-openapi.yml]}\n  - {scope: Mail.Send.Shared, description: Send mail on behalf\
  \ of others, flows: [authorizationCode], sources: [docs]}\n  - {scope: MailboxSettings.Read, description: Read user mailbox settings (automatic replies, time zone, language), flows: [authorizationCode], sources: [docs]}\n  - {scope: MailboxSettings.ReadWrite, description: Read and write user mailbox settings, flows: [authorizationCode], sources: [docs]}\n  - {scope: MailboxFolder.Read, description: Read user mail folders, flows: [authorizationCode], sources: [docs]}\n  - {scope: MailboxFolder.ReadWrite, description: Read and write user mail folders, flows: [authorizationCode], sources: [docs]}\n  - {scope: Calendars.Read, description: Read user calendars, flows: [authorizationCode], sources: [docs]}\n  - {scope: Calendars.ReadWrite, description: Read and write user calendars, flows: [authorizationCode], sources: [docs]}\n  - {scope: Contacts.Read, description: Read user contacts, flows: [authorizationCode], sources: [docs]}\n  - {scope: Contacts.ReadWrite, description: Read and write user\
  \ contacts, flows: [authorizationCode], sources: [docs]}\n  - {scope: Tasks.Read, description: Read user tasks and to-do lists, flows: [authorizationCode], sources: [docs]}\n  - {scope: Tasks.ReadWrite, description: Create, read, update, delete user tasks and to-do lists, flows: [authorizationCode], sources: [docs]}\n  - {scope: People.Read, description: Read the signed-in user's relevant people list, flows: [authorizationCode], sources: [docs]}\n  - {scope: User.Read, description: Sign in and read the user's profile, flows: [authorizationCode], sources: [docs]}\n  - {scope: offline_access, description: Maintain access via refresh tokens, flows: [authorizationCode], sources: [docs]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/scopes/microsoft-outlook-scopes.yml
summary_line: 20 scopes · authorizationCode
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
