---
api_specs:
- filename: sendmux-ai-billing-api-openapi.yml
  format: yaml
  label: sendmux-ai Billing API
  slug: sendmux-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-billing-api-openapi.yml
- filename: sendmux-ai-connection-api-openapi.yml
  format: yaml
  label: sendmux-ai Connection API
  slug: sendmux-ai-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-connection-api-openapi.yml
- filename: sendmux-ai-domain-filters-api-openapi.yml
  format: yaml
  label: sendmux-ai Domain Filters API
  slug: sendmux-ai-domain-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-domain-filters-api-openapi.yml
- filename: sendmux-ai-domains-api-openapi.yml
  format: yaml
  label: sendmux-ai Domains API
  slug: sendmux-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-domains-api-openapi.yml
- filename: sendmux-ai-emails-api-openapi.yml
  format: yaml
  label: sendmux-ai Emails API
  slug: sendmux-ai-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-emails-api-openapi.yml
- filename: sendmux-ai-inboxes-api-openapi.yml
  format: yaml
  label: sendmux-ai Inboxes API
  slug: sendmux-ai-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-inboxes-api-openapi.yml
- filename: sendmux-ai-mailbox-api-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailbox API
  slug: sendmux-ai-mailbox-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailbox-api-api-openapi.yml
- filename: sendmux-ai-mailbox-filters-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailbox Filters API
  slug: sendmux-ai-mailbox-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailbox-filters-api-openapi.yml
- filename: sendmux-ai-mailboxes-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailboxes API
  slug: sendmux-ai-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailboxes-api-openapi.yml
- filename: sendmux-ai-sending-accounts-api-openapi.yml
  format: yaml
  label: sendmux-ai Sending accounts API
  slug: sendmux-ai-sending-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-sending-accounts-api-openapi.yml
- filename: sendmux-ai-webhooks-api-openapi.yml
  format: yaml
  label: sendmux-ai Webhooks API
  slug: sendmux-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-webhooks-api-openapi.yml
authorization_urls:
- https://app.sendmux.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Sendmux Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'sendmux-ai publishes 52 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the sendmux-ai API on a user''s behalf.


  Tokens are issued from https://app.sendmux.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: sendmux-ai
provider_slug: sendmux-ai
schemes:
- description: Use the authorisation-code flow with S256 PKCE and resource=https://sendmux.ai/api. The user selects the team, API access and mailboxes during consent. OAuth access tokens authenticate HTTP API requests; use separate credentials for SMTP and IMAP.
  flows:
  - authorizationUrl: https://app.sendmux.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.sendmux.ai/oauth/token
  name: oauth2
  source: openapi/openapi-app.json
scope_count: 52
scope_names:
- analytics.*
- analytics.read
- billing.*
- billing.auto_topup
- billing.read
- billing.topup
- calendar.read
- calendar.write
- domain.*
- domain.create
- domain.delete
- domain.read
- domain.verify
- email.receive
- email.send
- key.*
- key.create
- key.read
- key.revoke
- key.rotate
- logs.*
- logs.read
- mailbox.admin.*
- mailbox.admin.create
- mailbox.admin.delete
- mailbox.admin.manage
- mailbox.admin.read
- mailbox.drafts.write
- mailbox.read
- mailbox.settings.update
- provider.*
- provider.create
- provider.delete
- provider.read
- provider.update
- routing.*
- routing.create
- routing.delete
- routing.read
- routing.update
- team.*
- team.members.invite
- team.members.remove
- team.members.roles
- team.read
- team.update
- webhook.*
- webhook.create
- webhook.delete
- webhook.manage
- webhook.read
- webhook.update
scopes:
- description: All analytics operations
  flows:
  - authorizationCode
  scope: analytics.*
- description: View key usage analytics and verification logs
  flows:
  - authorizationCode
  scope: analytics.read
- description: All billing operations
  flows:
  - authorizationCode
  scope: billing.*
- description: Configure auto top-up settings
  flows:
  - authorizationCode
  scope: billing.auto_topup
- description: View balance, transactions, invoices
  flows:
  - authorizationCode
  scope: billing.read
- description: Purchase balance top-ups
  flows:
  - authorizationCode
  scope: billing.topup
- description: Read calendars and events in this mailbox
  flows:
  - authorizationCode
  scope: calendar.read
- description: Create calendars and create, edit and delete events in this mailbox
  flows:
  - authorizationCode
  scope: calendar.write
- description: All domain operations
  flows:
  - authorizationCode
  scope: domain.*
- description: Add sending domains
  flows:
  - authorizationCode
  scope: domain.create
- description: Remove domains
  flows:
  - authorizationCode
  scope: domain.delete
- description: List/view domains and DNS status
  flows:
  - authorizationCode
  scope: domain.read
- description: Trigger domain verification
  flows:
  - authorizationCode
  scope: domain.verify
- description: Authorise email reception
  flows:
  - authorizationCode
  scope: email.receive
- description: Send email through the HTTP API
  flows:
  - authorizationCode
  scope: email.send
- description: All key management operations
  flows:
  - authorizationCode
  scope: key.*
- description: Create new API keys (both root and mailbox)
  flows:
  - authorizationCode
  scope: key.create
- description: List/view API keys and their metadata
  flows:
  - authorizationCode
  scope: key.read
- description: Revoke API keys
  flows:
  - authorizationCode
  scope: key.revoke
- description: Rotate API keys
  flows:
  - authorizationCode
  scope: key.rotate
- description: All log operations
  flows:
  - authorizationCode
  scope: logs.*
- description: View delivery logs
  flows:
  - authorizationCode
  scope: logs.read
- description: All mailbox admin operations
  flows:
  - authorizationCode
  scope: mailbox.admin.*
- description: Create mailboxes (admin-level)
  flows:
  - authorizationCode
  scope: mailbox.admin.create
- description: Delete mailboxes (admin-level)
  flows:
  - authorizationCode
  scope: mailbox.admin.delete
- description: Manage all mailbox settings
  flows:
  - authorizationCode
  scope: mailbox.admin.manage
- description: List/view mailboxes (admin-level)
  flows:
  - authorizationCode
  scope: mailbox.admin.read
- description: Create and edit saved mailbox drafts
  flows:
  - authorizationCode
  scope: mailbox.drafts.write
- description: Read mailbox contents (folders, messages)
  flows:
  - authorizationCode
  scope: mailbox.read
- description: Update own mailbox settings (signature, auto-reply)
  flows:
  - authorizationCode
  scope: mailbox.settings.update
- description: All provider operations
  flows:
  - authorizationCode
  scope: provider.*
- description: Add email provider accounts (Google, Microsoft, SMTP)
  flows:
  - authorizationCode
  scope: provider.create
- description: Remove provider accounts
  flows:
  - authorizationCode
  scope: provider.delete
- description: List/view provider accounts and connection status
  flows:
  - authorizationCode
  scope: provider.read
- description: Update provider settings, refresh tokens
  flows:
  - authorizationCode
  scope: provider.update
- description: All routing operations
  flows:
  - authorizationCode
  scope: routing.*
- description: Create delivery groups
  flows:
  - authorizationCode
  scope: routing.create
- description: Remove delivery groups
  flows:
  - authorizationCode
  scope: routing.delete
- description: List/view delivery groups and routing rules
  flows:
  - authorizationCode
  scope: routing.read
- description: Update delivery group configuration
  flows:
  - authorizationCode
  scope: routing.update
- description: All team operations
  flows:
  - authorizationCode
  scope: team.*
- description: Invite team members
  flows:
  - authorizationCode
  scope: team.members.invite
- description: Remove team members
  flows:
  - authorizationCode
  scope: team.members.remove
- description: Change member roles
  flows:
  - authorizationCode
  scope: team.members.roles
- description: View team settings and members
  flows:
  - authorizationCode
  scope: team.read
- description: Update team settings
  flows:
  - authorizationCode
  scope: team.update
- description: All webhook operations
  flows:
  - authorizationCode
  scope: webhook.*
- description: Create webhook subscriptions
  flows:
  - authorizationCode
  scope: webhook.create
- description: Delete webhook subscriptions
  flows:
  - authorizationCode
  scope: webhook.delete
- description: Rotate signing secret + send test events
  flows:
  - authorizationCode
  scope: webhook.manage
- description: List/view webhook subscriptions
  flows:
  - authorizationCode
  scope: webhook.read
- description: Update webhook URL, event types, enabled flag
  flows:
  - authorizationCode
  scope: webhook.update
slug: sendmux-ai-scopes
source_filename: sendmux-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/openapi-app.json\nschemes:\n- name: oauth2\n  source: openapi/openapi-app.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.sendmux.ai/oauth/authorize\n    tokenUrl: https://app.sendmux.ai/oauth/token\n  description: Use the authorisation-code flow with S256 PKCE and resource=https://sendmux.ai/api.\n    The user selects the team, API access and mailboxes during consent. OAuth access tokens\n    authenticate HTTP API requests; use separate credentials for SMTP and IMAP.\nscopes:\n- scope: analytics.*\n  description: All analytics operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: analytics.read\n  description: View key usage analytics and verification logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: billing.*\n  description: All billing operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n\
  - scope: billing.auto_topup\n  description: Configure auto top-up settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: billing.read\n  description: View balance, transactions, invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: billing.topup\n  description: Purchase balance top-ups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: calendar.read\n  description: Read calendars and events in this mailbox\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: calendar.write\n  description: Create calendars and create, edit and delete events in this mailbox\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: domain.*\n  description: All domain operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: domain.create\n  description: Add sending domains\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/openapi-app.json\n- scope: domain.delete\n  description: Remove domains\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: domain.read\n  description: List/view domains and DNS status\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: domain.verify\n  description: Trigger domain verification\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: email.receive\n  description: Authorise email reception\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: email.send\n  description: Send email through the HTTP API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: key.*\n  description: All key management operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: key.create\n  description: Create new API keys (both root and mailbox)\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/openapi-app.json\n- scope: key.read\n  description: List/view API keys and their metadata\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: key.revoke\n  description: Revoke API keys\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: key.rotate\n  description: Rotate API keys\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: logs.*\n  description: All log operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: logs.read\n  description: View delivery logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: mailbox.admin.*\n  description: All mailbox admin operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: mailbox.admin.create\n  description: Create mailboxes (admin-level)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n\
  - scope: mailbox.admin.delete\n  description: Delete mailboxes (admin-level)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: mailbox.admin.manage\n  description: Manage all mailbox settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: mailbox.admin.read\n  description: List/view mailboxes (admin-level)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: mailbox.drafts.write\n  description: Create and edit saved mailbox drafts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: mailbox.read\n  description: Read mailbox contents (folders, messages)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: mailbox.settings.update\n  description: Update own mailbox settings (signature, auto-reply)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: provider.*\n  description: All provider operations\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: provider.create\n  description: Add email provider accounts (Google, Microsoft, SMTP)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: provider.delete\n  description: Remove provider accounts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: provider.read\n  description: List/view provider accounts and connection status\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: provider.update\n  description: Update provider settings, refresh tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: routing.*\n  description: All routing operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: routing.create\n  description: Create delivery groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: routing.delete\n\
  \  description: Remove delivery groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: routing.read\n  description: List/view delivery groups and routing rules\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: routing.update\n  description: Update delivery group configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: team.*\n  description: All team operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: team.members.invite\n  description: Invite team members\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: team.members.remove\n  description: Remove team members\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: team.members.roles\n  description: Change member roles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: team.read\n  description:\
  \ View team settings and members\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: team.update\n  description: Update team settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: webhook.*\n  description: All webhook operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: webhook.create\n  description: Create webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: webhook.delete\n  description: Delete webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: webhook.manage\n  description: Rotate signing secret + send test events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: webhook.read\n  description: List/view webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n- scope: webhook.update\n  description:\
  \ Update webhook URL, event types, enabled flag\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi-app.json\n"
source_yaml_url: https://artifacts.apis.io/sendmux-ai/scopes/sendmux-ai-scopes.yml
summary_line: 52 scopes · authorizationCode
tags:
- Company
- Email
- Artificial Intelligence
- Agents
- Integration
token_bound: false
token_urls:
- https://app.sendmux.ai/oauth/token
---
