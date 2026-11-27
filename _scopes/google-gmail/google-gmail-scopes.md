---
api_specs:
- filename: google-gmail-domains-api-openapi.yml
  format: yaml
  label: Google Gmail Domains API
  slug: google-gmail-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gmail/openapi/google-gmail-domains-api-openapi.yml
- filename: google-gmail-domainstats-api-openapi.yml
  format: yaml
  label: Google Gmail Domain Stats API
  slug: google-gmail-domainstats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gmail/openapi/google-gmail-domainstats-api-openapi.yml
- filename: google-gmail-users-api-openapi.yml
  format: yaml
  label: Google Gmail Users API
  slug: google-gmail-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gmail/openapi/google-gmail-users-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Gmail Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Gmail publishes 30 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Gmail API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Gmail
provider_slug: google-gmail
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gmail-gmail-users-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml
scope_count: 30
scope_names:
- https://mail.google.com/
- https://www.googleapis.com/auth/gmail.addons.current.action.compose
- https://www.googleapis.com/auth/gmail.addons.current.message.action
- https://www.googleapis.com/auth/gmail.addons.current.message.metadata
- https://www.googleapis.com/auth/gmail.addons.current.message.readonly
- https://www.googleapis.com/auth/gmail.compose
- https://www.googleapis.com/auth/gmail.drafts
- https://www.googleapis.com/auth/gmail.drafts.create
- https://www.googleapis.com/auth/gmail.drafts.readonly
- https://www.googleapis.com/auth/gmail.insert
- https://www.googleapis.com/auth/gmail.labels
- https://www.googleapis.com/auth/gmail.labels.create
- https://www.googleapis.com/auth/gmail.labels.readonly
- https://www.googleapis.com/auth/gmail.messages
- https://www.googleapis.com/auth/gmail.messages.delete
- https://www.googleapis.com/auth/gmail.messages.modify
- https://www.googleapis.com/auth/gmail.messages.readonly
- https://www.googleapis.com/auth/gmail.metadata
- https://www.googleapis.com/auth/gmail.modify
- https://www.googleapis.com/auth/gmail.readonly
- https://www.googleapis.com/auth/gmail.send
- https://www.googleapis.com/auth/gmail.send.self
- https://www.googleapis.com/auth/gmail.settings.basic
- https://www.googleapis.com/auth/gmail.settings.filters
- https://www.googleapis.com/auth/gmail.settings.filters.readonly
- https://www.googleapis.com/auth/gmail.settings.sharing
- https://www.googleapis.com/auth/postmaster
- https://www.googleapis.com/auth/postmaster.domain
- https://www.googleapis.com/auth/postmaster.traffic.readonly
- https://www.googleapis.com/auth/postmaster.user
scopes:
- description: Read, compose, send, and permanently delete all your email from Gmail
  flows:
  - authorizationCode
  scope: https://mail.google.com/
- description: Manage drafts and send emails when you interact with the add-on
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.addons.current.action.compose
- description: View your email messages when you interact with the add-on
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.addons.current.message.action
- description: View your email message metadata when the add-on is running
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.addons.current.message.metadata
- description: View your email messages when the add-on is running
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.addons.current.message.readonly
- description: Manage drafts and send emails
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.compose
- description: Read, compose, send, update, and permanently delete your draft emails
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.drafts
- description: Compose new draft emails
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.drafts.create
- description: Read your draft emails
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.drafts.readonly
- description: Add emails into your Gmail mailbox
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.insert
- description: See and edit your email labels
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.labels
- description: Create new email labels
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.labels.create
- description: Read your email labels
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.labels.readonly
- description: Read, update, and permanently delete all your emails
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.messages
- description: Permanently delete all your emails
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.messages.delete
- description: Update but not delete your emails
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.messages.modify
- description: Read your emails
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.messages.readonly
- description: View your email message metadata such as labels and headers, but not the email body
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.metadata
- description: Read, compose, and send emails from your Gmail account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.modify
- description: View your email messages and settings
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.readonly
- description: Send email on your behalf
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.send
- description: Send email to yourself
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.send.self
- description: See, edit, create, or change your email settings and filters in Gmail
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.settings.basic
- description: Read, create, and delete your filters
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.settings.filters
- description: Read your filters
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.settings.filters.readonly
- description: Manage your sensitive mail settings, including who can manage your mail
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/gmail.settings.sharing
- description: Get email traffic metrics, manage domains, and manage domain users for the domains you have registered with Postmaster Tools
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/postmaster
- description: View and manage the domains you have registered with Postmaster Tools
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/postmaster.domain
- description: Get email traffic metrics for the domains you have registered with Postmaster Tools
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/postmaster.traffic.readonly
- description: View and manage users for the domains you have registered with Postmaster Tools
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/postmaster.user
slug: google-gmail-scopes
source_filename: google-gmail-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-gmail-gmail-users-api-openapi.yml, openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml,\n  openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-gmail-gmail-users-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n\
  - scope: https://mail.google.com/\n  description: Read, compose, send, and permanently delete all your email from Gmail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.addons.current.action.compose\n  description: Manage drafts and send emails when you interact with the add-on\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.addons.current.message.action\n  description: View your email messages when you interact with the add-on\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.addons.current.message.metadata\n  description: View your email message metadata when the add-on is running\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.addons.current.message.readonly\n\
  \  description: View your email messages when the add-on is running\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.compose\n  description: Manage drafts and send emails\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.drafts\n  description: Read, compose, send, update, and permanently delete your draft emails\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.drafts.create\n  description: Compose new draft emails\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.drafts.readonly\n  description: Read your draft emails\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/gmail.insert\n  description: Add emails into your Gmail mailbox\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.labels\n  description: See and edit your email labels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.labels.create\n  description: Create new email labels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.labels.readonly\n  description: Read your email labels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.messages\n  description: Read, update, and permanently delete all your emails\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/gmail.messages.delete\n  description: Permanently delete all your emails\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.messages.modify\n  description: Update but not delete your emails\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.messages.readonly\n  description: Read your emails\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.metadata\n  description: View your email message metadata such as labels and headers, but not the email\n    body\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.modify\n  description: Read, compose, and send emails from your Gmail\
  \ account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.readonly\n  description: View your email messages and settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.send\n  description: Send email on your behalf\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.send.self\n  description: Send email to yourself\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.settings.basic\n  description: See, edit, create, or change your email settings and filters in Gmail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.settings.filters\n\
  \  description: Read, create, and delete your filters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.settings.filters.readonly\n  description: Read your filters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/gmail.settings.sharing\n  description: Manage your sensitive mail settings, including who can manage your mail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/postmaster\n  description: Get email traffic metrics, manage domains, and manage domain users for the domains\n    you have registered with Postmaster Tools\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml\n  - openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/postmaster.domain\n  description: View and manage the domains you have registered with Postmaster Tools\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml\n  - openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml\n- scope: https://www.googleapis.com/auth/postmaster.traffic.readonly\n  description: Get email traffic metrics for the domains you have registered with Postmaster\n    Tools\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml\n  - openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml\n- scope: https://www.googleapis.com/auth/postmaster.user\n  description: View and manage users for the domains you have registered with Postmaster Tools\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml\n  - openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-gmail/scopes/google-gmail-scopes.yml
summary_line: 30 scopes · authorizationCode
tags:
- Drafts
- Email
- Gmail
- Google
- Google Workspace
- Labels
- Messaging
- Threads
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
