---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Exchange Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Exchange publishes 18 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Exchange API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Exchange
provider_slug: microsoft-exchange
schemes:
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-exchange-admin-api-openapi.yml
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-exchange-graph-calendar-openapi.yml
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-exchange-graph-contacts-openapi.yml
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-exchange-graph-import-export-openapi.yml
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-exchange-graph-mail-openapi.yml
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-exchange-graph-people-openapi.yml
scope_count: 18
scope_names:
- Calendars.Read
- Calendars.Read.Shared
- Calendars.ReadWrite
- Calendars.ReadWrite.Shared
- Contacts.Read
- Contacts.Read.Shared
- Contacts.ReadWrite
- Contacts.ReadWrite.Shared
- Mail.Read
- Mail.ReadBasic
- Mail.ReadWrite
- Mail.Send
- Mailbox.Export
- Mailbox.Import
- MailboxFolder.Read
- People.Read
- People.Read.All
- https://outlook.office365.com/.default
scopes:
- description: Read user calendars
  flows:
  - authorizationCode
  scope: Calendars.Read
- description: Read shared calendars
  flows:
  - authorizationCode
  scope: Calendars.Read.Shared
- description: Read and write access to user calendars
  flows:
  - authorizationCode
  scope: Calendars.ReadWrite
- description: Read and write shared calendars
  flows:
  - authorizationCode
  scope: Calendars.ReadWrite.Shared
- description: Read user contacts
  flows:
  - authorizationCode
  scope: Contacts.Read
- description: Read shared contacts
  flows:
  - authorizationCode
  scope: Contacts.Read.Shared
- description: Read and write user contacts
  flows:
  - authorizationCode
  scope: Contacts.ReadWrite
- description: Read and write shared contacts
  flows:
  - authorizationCode
  scope: Contacts.ReadWrite.Shared
- description: Read user mail
  flows:
  - authorizationCode
  scope: Mail.Read
- description: Read user basic mail
  flows:
  - authorizationCode
  scope: Mail.ReadBasic
- description: Read and write access to user mail
  flows:
  - authorizationCode
  scope: Mail.ReadWrite
- description: Send mail as a user
  flows:
  - authorizationCode
  scope: Mail.Send
- description: Export content from mailboxes
  flows:
  - clientCredentials
  scope: Mailbox.Export
- description: Import content into mailboxes
  flows:
  - clientCredentials
  scope: Mailbox.Import
- description: Read mailbox folder information
  flows:
  - clientCredentials
  scope: MailboxFolder.Read
- description: Read user's relevant people list
  flows:
  - authorizationCode
  scope: People.Read
- description: Read all users' relevant people lists
  flows:
  - authorizationCode
  scope: People.Read.All
- description: Default scope for Exchange Online Admin API
  flows:
  - clientCredentials
  scope: https://outlook.office365.com/.default
slug: microsoft-exchange-scopes
source_filename: microsoft-exchange-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-exchange-admin-api-openapi.yml, openapi/microsoft-exchange-graph-calendar-openapi.yml,\n  openapi/microsoft-exchange-graph-contacts-openapi.yml, openapi/microsoft-exchange-graph-import-export-openapi.yml,\n  openapi/microsoft-exchange-graph-mail-openapi.yml, openapi/microsoft-exchange-graph-people-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-exchange-admin-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: OAuth 2.0 authorization with Microsoft identity platform\n- name: oauth2\n  source: openapi/microsoft-exchange-graph-calendar-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization with Microsoft\
  \ identity platform\n- name: oauth2\n  source: openapi/microsoft-exchange-graph-contacts-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization with Microsoft identity platform\n- name: oauth2\n  source: openapi/microsoft-exchange-graph-import-export-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: OAuth 2.0 authorization with Microsoft identity platform\n- name: oauth2\n  source: openapi/microsoft-exchange-graph-mail-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization with Microsoft identity platform\n- name:\
  \ oauth2\n  source: openapi/microsoft-exchange-graph-people-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization with Microsoft identity platform\nscopes:\n- scope: Calendars.Read\n  description: Read user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-calendar-openapi.yml\n- scope: Calendars.Read.Shared\n  description: Read shared calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-calendar-openapi.yml\n- scope: Calendars.ReadWrite\n  description: Read and write access to user calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-calendar-openapi.yml\n- scope: Calendars.ReadWrite.Shared\n  description: Read and write shared calendars\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/microsoft-exchange-graph-calendar-openapi.yml\n- scope: Contacts.Read\n  description: Read user contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-contacts-openapi.yml\n- scope: Contacts.Read.Shared\n  description: Read shared contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-contacts-openapi.yml\n- scope: Contacts.ReadWrite\n  description: Read and write user contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-contacts-openapi.yml\n- scope: Contacts.ReadWrite.Shared\n  description: Read and write shared contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-contacts-openapi.yml\n- scope: Mail.Read\n  description: Read user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-mail-openapi.yml\n- scope: Mail.ReadBasic\n  description: Read user basic mail\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/microsoft-exchange-graph-mail-openapi.yml\n- scope: Mail.ReadWrite\n  description: Read and write access to user mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-mail-openapi.yml\n- scope: Mail.Send\n  description: Send mail as a user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-mail-openapi.yml\n- scope: Mailbox.Export\n  description: Export content from mailboxes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-exchange-graph-import-export-openapi.yml\n- scope: Mailbox.Import\n  description: Import content into mailboxes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-exchange-graph-import-export-openapi.yml\n- scope: MailboxFolder.Read\n  description: Read mailbox folder information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-exchange-graph-import-export-openapi.yml\n- scope: People.Read\n  description: Read user's relevant\
  \ people list\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-people-openapi.yml\n- scope: People.Read.All\n  description: Read all users' relevant people lists\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-exchange-graph-people-openapi.yml\n- scope: https://outlook.office365.com/.default\n  description: Default scope for Exchange Online Admin API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-exchange-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/scopes/microsoft-exchange-scopes.yml
summary_line: 18 scopes · clientCredentials/authorizationCode
tags:
- Calendar
- Collaboration
- Contacts
- Email
- Enterprise
token_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
