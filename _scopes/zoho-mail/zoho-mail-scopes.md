---
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zoho Mail Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoho Mail publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoho Mail API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoho Mail
provider_slug: zoho-mail
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: OAuth2
  source: openapi/openapi.json
scope_count: 11
scope_names:
- ZohoMail.accounts
- ZohoMail.accounts.READ
- ZohoMail.bookmarks
- ZohoMail.folders
- ZohoMail.labels
- ZohoMail.messages
- ZohoMail.notes
- ZohoMail.organization
- ZohoMail.organization.accounts
- ZohoMail.signatures
- ZohoMail.tasks
scopes:
- description: Access account settings
  flows:
  - authorizationCode
  scope: ZohoMail.accounts
- description: Read account details
  flows:
  - authorizationCode
  scope: ZohoMail.accounts.READ
- description: Access bookmarks
  flows:
  - authorizationCode
  scope: ZohoMail.bookmarks
- description: Access folders
  flows:
  - authorizationCode
  scope: ZohoMail.folders
- description: Access labels
  flows:
  - authorizationCode
  scope: ZohoMail.labels
- description: Access email messages
  flows:
  - authorizationCode
  scope: ZohoMail.messages
- description: Access notes
  flows:
  - authorizationCode
  scope: ZohoMail.notes
- description: Access organization settings
  flows:
  - authorizationCode
  scope: ZohoMail.organization
- description: Admin access to user accounts
  flows:
  - authorizationCode
  scope: ZohoMail.organization.accounts
- description: Access signatures
  flows:
  - authorizationCode
  scope: ZohoMail.signatures
- description: Access tasks
  flows:
  - authorizationCode
  scope: ZohoMail.tasks
slug: zoho-mail-scopes
source_filename: zoho-mail-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\nscopes:\n- scope: ZohoMail.accounts\n  description: Access account settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.accounts.READ\n  description: Read account details\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.bookmarks\n  description: Access bookmarks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.folders\n  description: Access folders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.labels\n  description: Access labels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.messages\n\
  \  description: Access email messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.notes\n  description: Access notes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.organization\n  description: Access organization settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.organization.accounts\n  description: Admin access to user accounts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.signatures\n  description: Access signatures\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoMail.tasks\n  description: Access tasks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-mail/refs/heads/main/scopes/zoho-mail-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Email
- Mail
- Collaboration
- Messaging
- Calendar
- Contacts
- Organization Management
- SaaS
token_urls:
- https://accounts.zoho.com/oauth/v2/token
---
