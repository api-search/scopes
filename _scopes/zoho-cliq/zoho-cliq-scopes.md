---
api_specs:
- filename: chats.yml
  format: yaml
  label: Zoho Cliq API
  slug: zoho-cliq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-cliq/refs/heads/main/openapi/chats.yml
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth
description: ''
docs: ''
flows:
- implicit
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zoho Cliq Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoho Cliq publishes 61 OAuth 2.0 scopes via the implicit and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoho Cliq API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoho Cliq
provider_slug: zoho-cliq
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/bots.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/buttons.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/chats.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/datastores.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/dndsettings.yml
- flows:
  - flow: implicit
  name: Cliq_Auth
  source: openapi/extensions.yml
- flows:
  - flow: implicit
  name: Cliq_Auth
  source: openapi/functions.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/keyboardshortcuts.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/mentions.yml
- flows:
  - flow: implicit
  name: Cliq_Auth
  source: openapi/messageactions.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/messagecards.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/messageformat.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/messages.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/mobilesettings.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/mypins.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/pinmessages.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/reminders.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/scheduledmessages.yml
- flows:
  - flow: implicit
  name: Cliq_Auth
  source: openapi/slashcommands.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: Cliq_Auth
  source: openapi/stars.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/threads.yml
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  name: Cliq_Auth
  source: openapi/userpreferences.yml
scope_count: 61
scope_names:
- Commands.CREATE
- Commands.DELETE
- Commands.READ
- Commands.UPDATE
- DatastoreRecords.CREATE
- DatastoreRecords.DELETE
- DatastoreRecords.READ
- DatastoreRecords.UPDATE
- Datastores.CREATE
- Datastores.DELETE
- Datastores.READ
- Datastores.UPDATE
- Extensions.READ
- Extensions.UPDATE
- ZohoCliq.BotMessages.CREATE
- ZohoCliq.Bots.CREATE
- ZohoCliq.Bots.DELETE
- ZohoCliq.Bots.READ
- ZohoCliq.Bots.UPDATE
- ZohoCliq.Channels.CREATE
- ZohoCliq.Channels.UPDATE
- ZohoCliq.Chats.CREATE
- ZohoCliq.Chats.DELETE
- ZohoCliq.Chats.READ
- ZohoCliq.Chats.UPDATE
- ZohoCliq.Commands.CREATE
- ZohoCliq.Commands.DELETE
- ZohoCliq.Commands.READ
- ZohoCliq.Commands.UPDATE
- ZohoCliq.DatastoreRecords.CREATE
- ZohoCliq.DatastoreRecords.DELETE
- ZohoCliq.DatastoreRecords.READ
- ZohoCliq.DatastoreRecords.UPDATE
- ZohoCliq.Datastores.ALL
- ZohoCliq.Datastores.CREATE
- ZohoCliq.Datastores.DELETE
- ZohoCliq.Datastores.READ
- ZohoCliq.Datastores.UPDATE
- ZohoCliq.Extensions.CREATE
- ZohoCliq.Extensions.READ
- ZohoCliq.Extensions.UPDATE
- ZohoCliq.Functions.CREATE
- ZohoCliq.Functions.DELETE
- ZohoCliq.Functions.READ
- ZohoCliq.Functions.UPDATE
- ZohoCliq.MessageActions.CREATE
- ZohoCliq.MessageActions.DELETE
- ZohoCliq.MessageActions.READ
- ZohoCliq.MessageActions.UPDATE
- ZohoCliq.Messages.CREATE
- ZohoCliq.Messages.DELETE
- ZohoCliq.Messages.READ
- ZohoCliq.Messages.UPDATE
- ZohoCliq.Profile.DELETE
- ZohoCliq.Profile.READ
- ZohoCliq.Profile.UPDATE
- ZohoCliq.Reminders.CREATE
- ZohoCliq.Reminders.DELETE
- ZohoCliq.Reminders.READ
- ZohoCliq.Reminders.UPDATE
- ZohoCliq.Webhooks.CREATE
scopes:
- description: Create new custom Slash Commands.
  flows:
  - implicit
  scope: Commands.CREATE
- description: Permanently delete slash commands and their handlers.
  flows:
  - implicit
  scope: Commands.DELETE
- description: Read slash command configurations, handlers, and execution logs.
  flows:
  - implicit
  scope: Commands.READ
- description: Update slash command configurations and manage command handlers.
  flows:
  - implicit
  scope: Commands.UPDATE
- description: ''
  flows: []
  scope: DatastoreRecords.CREATE
- description: ''
  flows: []
  scope: DatastoreRecords.DELETE
- description: ''
  flows: []
  scope: DatastoreRecords.READ
- description: ''
  flows: []
  scope: DatastoreRecords.UPDATE
- description: ''
  flows: []
  scope: Datastores.CREATE
- description: ''
  flows: []
  scope: Datastores.DELETE
- description: ''
  flows: []
  scope: Datastores.READ
- description: ''
  flows: []
  scope: Datastores.UPDATE
- description: ''
  flows: []
  scope: Extensions.READ
- description: ''
  flows: []
  scope: Extensions.UPDATE
- description: Send messages via bot incoming webhooks
  flows:
  - implicit
  scope: ZohoCliq.BotMessages.CREATE
- description: Create Bots
  flows:
  - implicit
  scope: ZohoCliq.Bots.CREATE
- description: Delete Bots
  flows:
  - implicit
  scope: ZohoCliq.Bots.DELETE
- description: Read Bot Information
  flows:
  - implicit
  scope: ZohoCliq.Bots.READ
- description: Update Bots
  flows:
  - implicit
  scope: ZohoCliq.Bots.UPDATE
- description: Post messages to channels
  flows:
  - implicit
  scope: ZohoCliq.Channels.CREATE
- description: Update Channel Settings
  flows:
  - implicit
  scope: ZohoCliq.Channels.UPDATE
- description: Create Chats
  flows:
  - implicit
  scope: ZohoCliq.Chats.CREATE
- description: Delete Chats
  flows:
  - implicit
  scope: ZohoCliq.Chats.DELETE
- description: Read Chats
  flows:
  - implicit
  scope: ZohoCliq.Chats.READ
- description: Modify Chats
  flows:
  - implicit
  scope: ZohoCliq.Chats.UPDATE
- description: ''
  flows: []
  scope: ZohoCliq.Commands.CREATE
- description: ''
  flows: []
  scope: ZohoCliq.Commands.DELETE
- description: ''
  flows: []
  scope: ZohoCliq.Commands.READ
- description: ''
  flows: []
  scope: ZohoCliq.Commands.UPDATE
- description: Insert new records into Datastores.
  flows:
  - implicit
  scope: ZohoCliq.DatastoreRecords.CREATE
- description: Delete records from Datastores.
  flows:
  - implicit
  scope: ZohoCliq.DatastoreRecords.DELETE
- description: Read and query records from Datastores.
  flows:
  - implicit
  scope: ZohoCliq.DatastoreRecords.READ
- description: Update existing records in Datastores.
  flows:
  - implicit
  scope: ZohoCliq.DatastoreRecords.UPDATE
- description: Create, Read, Update and Delete Datastores
  flows:
  - implicit
  scope: ZohoCliq.Datastores.ALL
- description: Create new Datastores with schema definitions.
  flows:
  - implicit
  scope: ZohoCliq.Datastores.CREATE
- description: Permanently delete Datastores and all their records.
  flows:
  - implicit
  scope: ZohoCliq.Datastores.DELETE
- description: Read Datastore metadata, field schemas, and execution logs.
  flows:
  - implicit
  scope: ZohoCliq.Datastores.READ
- description: Update Datastore metadata and field schema definitions.
  flows:
  - implicit
  scope: ZohoCliq.Datastores.UPDATE
- description: Install Extensions (Applications) into an organisation or network scope.
  flows:
  - implicit
  scope: ZohoCliq.Extensions.CREATE
- description: Read extension configurations, handlers, properties, and execution logs.
  flows:
  - implicit
  scope: ZohoCliq.Extensions.READ
- description: Update extension configurations, handlers, and properties; manage extension lifecycle.
  flows:
  - implicit
  scope: ZohoCliq.Extensions.UPDATE
- description: Create new Functions in the platform.
  flows:
  - implicit
  scope: ZohoCliq.Functions.CREATE
- description: Permanently delete Functions and their handlers.
  flows:
  - implicit
  scope: ZohoCliq.Functions.DELETE
- description: Read function configurations, handlers, and execution logs.
  flows:
  - implicit
  scope: ZohoCliq.Functions.READ
- description: Update function configurations and manage function handlers.
  flows:
  - implicit
  scope: ZohoCliq.Functions.UPDATE
- description: Create new custom Message Actions.
  flows:
  - implicit
  scope: ZohoCliq.MessageActions.CREATE
- description: Permanently delete Message Actions and their handlers.
  flows:
  - implicit
  scope: ZohoCliq.MessageActions.DELETE
- description: Read message action configurations, handlers, and execution logs.
  flows:
  - implicit
  scope: ZohoCliq.MessageActions.READ
- description: Update message action configurations and manage message action handlers.
  flows:
  - implicit
  scope: ZohoCliq.MessageActions.UPDATE
- description: Send messages to users and chats
  flows:
  - authorizationCode
  - implicit
  scope: ZohoCliq.Messages.CREATE
- description: Delete Messages
  flows:
  - authorizationCode
  - implicit
  scope: ZohoCliq.Messages.DELETE
- description: Read Messages
  flows:
  - authorizationCode
  - implicit
  scope: ZohoCliq.Messages.READ
- description: Modify Messages
  flows:
  - authorizationCode
  - implicit
  scope: ZohoCliq.Messages.UPDATE
- description: Delete user profile settings
  flows:
  - implicit
  scope: ZohoCliq.Profile.DELETE
- description: Read user profile settings
  flows:
  - implicit
  scope: ZohoCliq.Profile.READ
- description: Update user profile settings
  flows:
  - implicit
  scope: ZohoCliq.Profile.UPDATE
- description: Create reminder notifications
  flows:
  - implicit
  scope: ZohoCliq.Reminders.CREATE
- description: Delete reminders
  flows:
  - implicit
  scope: ZohoCliq.Reminders.DELETE
- description: Read reminders
  flows:
  - implicit
  scope: ZohoCliq.Reminders.READ
- description: Update reminders
  flows:
  - implicit
  scope: ZohoCliq.Reminders.UPDATE
- description: Post messages to conversations via webhooks
  flows:
  - implicit
  scope: ZohoCliq.Webhooks.CREATE
slug: zoho-cliq-scopes
source_filename: zoho-cliq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bots.yml, openapi/buttons.yml, openapi/chats.yml, openapi/datastores.yml, openapi/dndsettings.yml,\n  openapi/extensions.yml, openapi/functions.yml, openapi/keyboardshortcuts.yml, openapi/mentions.yml,\n  openapi/messageactions.yml, openapi/messagecards.yml, openapi/messageformat.yml, openapi/messages.yml,\n  openapi/mobilesettings.yml, openapi/mypins.yml, openapi/pinmessages.yml, openapi/reminders.yml,\n  openapi/scheduledmessages.yml, openapi/slashcommands.yml, openapi/stars.yml, openapi/threads.yml,\n  openapi/userpreferences.yml\nschemes:\n- name: Cliq_Auth\n  source: openapi/bots.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/buttons.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/chats.yml\n  flows:\n  - flow: implicit\n    authorizationUrl:\
  \ https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/datastores.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/dndsettings.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/extensions.yml\n  flows:\n  - flow: implicit\n- name: Cliq_Auth\n  source: openapi/functions.yml\n  flows:\n  - flow: implicit\n- name: Cliq_Auth\n  source: openapi/keyboardshortcuts.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/mentions.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/messageactions.yml\n  flows:\n  - flow: implicit\n- name: Cliq_Auth\n  source: openapi/messagecards.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n\
  - name: Cliq_Auth\n  source: openapi/messageformat.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/messages.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/mobilesettings.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/mypins.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/pinmessages.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/reminders.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/scheduledmessages.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n\
  - name: Cliq_Auth\n  source: openapi/slashcommands.yml\n  flows:\n  - flow: implicit\n- name: Cliq_Auth\n  source: openapi/stars.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n- name: Cliq_Auth\n  source: openapi/threads.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n- name: Cliq_Auth\n  source: openapi/userpreferences.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\nscopes:\n- scope: Commands.CREATE\n  description: Create new custom Slash Commands.\n  flows:\n  - implicit\n  sources:\n  - openapi/slashcommands.yml\n- scope: Commands.DELETE\n  description: Permanently delete slash commands and their handlers.\n  flows:\n  - implicit\n  sources:\n  - openapi/slashcommands.yml\n- scope: Commands.READ\n  description: Read slash command configurations, handlers, and execution logs.\n\
  \  flows:\n  - implicit\n  sources:\n  - openapi/slashcommands.yml\n- scope: Commands.UPDATE\n  description: Update slash command configurations and manage command handlers.\n  flows:\n  - implicit\n  sources:\n  - openapi/slashcommands.yml\n- scope: DatastoreRecords.CREATE\n  sources:\n  - openapi/datastores.yml\n- scope: DatastoreRecords.DELETE\n  sources:\n  - openapi/datastores.yml\n- scope: DatastoreRecords.READ\n  sources:\n  - openapi/datastores.yml\n- scope: DatastoreRecords.UPDATE\n  sources:\n  - openapi/datastores.yml\n- scope: Datastores.CREATE\n  sources:\n  - openapi/datastores.yml\n- scope: Datastores.DELETE\n  sources:\n  - openapi/datastores.yml\n- scope: Datastores.READ\n  sources:\n  - openapi/datastores.yml\n- scope: Datastores.UPDATE\n  sources:\n  - openapi/datastores.yml\n- scope: Extensions.READ\n  sources:\n  - openapi/extensions.yml\n- scope: Extensions.UPDATE\n  sources:\n  - openapi/extensions.yml\n- scope: ZohoCliq.BotMessages.CREATE\n  description: Send messages\
  \ via bot incoming webhooks\n  flows:\n  - implicit\n  sources:\n  - openapi/bots.yml\n- scope: ZohoCliq.Bots.CREATE\n  description: Create Bots\n  flows:\n  - implicit\n  sources:\n  - openapi/bots.yml\n- scope: ZohoCliq.Bots.DELETE\n  description: Delete Bots\n  flows:\n  - implicit\n  sources:\n  - openapi/bots.yml\n- scope: ZohoCliq.Bots.READ\n  description: Read Bot Information\n  flows:\n  - implicit\n  sources:\n  - openapi/bots.yml\n- scope: ZohoCliq.Bots.UPDATE\n  description: Update Bots\n  flows:\n  - implicit\n  sources:\n  - openapi/bots.yml\n- scope: ZohoCliq.Channels.CREATE\n  description: Post messages to channels\n  flows:\n  - implicit\n  sources:\n  - openapi/messagecards.yml\n- scope: ZohoCliq.Channels.UPDATE\n  description: Update Channel Settings\n  flows:\n  - implicit\n  sources:\n  - openapi/bots.yml\n  - openapi/threads.yml\n- scope: ZohoCliq.Chats.CREATE\n  description: Create Chats\n  flows:\n  - implicit\n  sources:\n  - openapi/chats.yml\n  - openapi/mypins.yml\n\
  \  - openapi/pinmessages.yml\n- scope: ZohoCliq.Chats.DELETE\n  description: Delete Chats\n  flows:\n  - implicit\n  sources:\n  - openapi/chats.yml\n  - openapi/mypins.yml\n  - openapi/pinmessages.yml\n  - openapi/threads.yml\n- scope: ZohoCliq.Chats.READ\n  description: Read Chats\n  flows:\n  - implicit\n  sources:\n  - openapi/chats.yml\n  - openapi/mentions.yml\n  - openapi/messages.yml\n  - openapi/mypins.yml\n  - openapi/pinmessages.yml\n  - openapi/threads.yml\n- scope: ZohoCliq.Chats.UPDATE\n  description: Modify Chats\n  flows:\n  - implicit\n  sources:\n  - openapi/chats.yml\n  - openapi/mypins.yml\n  - openapi/pinmessages.yml\n  - openapi/threads.yml\n- scope: ZohoCliq.Commands.CREATE\n  sources:\n  - openapi/slashcommands.yml\n- scope: ZohoCliq.Commands.DELETE\n  sources:\n  - openapi/slashcommands.yml\n- scope: ZohoCliq.Commands.READ\n  sources:\n  - openapi/slashcommands.yml\n- scope: ZohoCliq.Commands.UPDATE\n  sources:\n  - openapi/slashcommands.yml\n- scope: ZohoCliq.DatastoreRecords.CREATE\n\
  \  description: Insert new records into Datastores.\n  flows:\n  - implicit\n  sources:\n  - openapi/datastores.yml\n- scope: ZohoCliq.DatastoreRecords.DELETE\n  description: Delete records from Datastores.\n  flows:\n  - implicit\n  sources:\n  - openapi/datastores.yml\n- scope: ZohoCliq.DatastoreRecords.READ\n  description: Read and query records from Datastores.\n  flows:\n  - implicit\n  sources:\n  - openapi/datastores.yml\n- scope: ZohoCliq.DatastoreRecords.UPDATE\n  description: Update existing records in Datastores.\n  flows:\n  - implicit\n  sources:\n  - openapi/datastores.yml\n- scope: ZohoCliq.Datastores.ALL\n  description: Create, Read, Update and Delete Datastores\n  flows:\n  - implicit\n  sources:\n  - openapi/datastores.yml\n- scope: ZohoCliq.Datastores.CREATE\n  description: Create new Datastores with schema definitions.\n  flows:\n  - implicit\n  sources:\n  - openapi/datastores.yml\n- scope: ZohoCliq.Datastores.DELETE\n  description: Permanently delete Datastores and\
  \ all their records.\n  flows:\n  - implicit\n  sources:\n  - openapi/datastores.yml\n- scope: ZohoCliq.Datastores.READ\n  description: Read Datastore metadata, field schemas, and execution logs.\n  flows:\n  - implicit\n  sources:\n  - openapi/datastores.yml\n- scope: ZohoCliq.Datastores.UPDATE\n  description: Update Datastore metadata and field schema definitions.\n  flows:\n  - implicit\n  sources:\n  - openapi/datastores.yml\n- scope: ZohoCliq.Extensions.CREATE\n  description: Install Extensions (Applications) into an organisation or network scope.\n  flows:\n  - implicit\n  sources:\n  - openapi/extensions.yml\n- scope: ZohoCliq.Extensions.READ\n  description: Read extension configurations, handlers, properties, and execution logs.\n  flows:\n  - implicit\n  sources:\n  - openapi/extensions.yml\n- scope: ZohoCliq.Extensions.UPDATE\n  description: Update extension configurations, handlers, and properties; manage extension lifecycle.\n  flows:\n  - implicit\n  sources:\n  - openapi/extensions.yml\n\
  - scope: ZohoCliq.Functions.CREATE\n  description: Create new Functions in the platform.\n  flows:\n  - implicit\n  sources:\n  - openapi/functions.yml\n- scope: ZohoCliq.Functions.DELETE\n  description: Permanently delete Functions and their handlers.\n  flows:\n  - implicit\n  sources:\n  - openapi/functions.yml\n- scope: ZohoCliq.Functions.READ\n  description: Read function configurations, handlers, and execution logs.\n  flows:\n  - implicit\n  sources:\n  - openapi/functions.yml\n- scope: ZohoCliq.Functions.UPDATE\n  description: Update function configurations and manage function handlers.\n  flows:\n  - implicit\n  sources:\n  - openapi/functions.yml\n- scope: ZohoCliq.MessageActions.CREATE\n  description: Create new custom Message Actions.\n  flows:\n  - implicit\n  sources:\n  - openapi/messageactions.yml\n  - openapi/messages.yml\n- scope: ZohoCliq.MessageActions.DELETE\n  description: Permanently delete Message Actions and their handlers.\n  flows:\n  - implicit\n  sources:\n\
  \  - openapi/messageactions.yml\n  - openapi/messages.yml\n- scope: ZohoCliq.MessageActions.READ\n  description: Read message action configurations, handlers, and execution logs.\n  flows:\n  - implicit\n  sources:\n  - openapi/messageactions.yml\n  - openapi/messages.yml\n- scope: ZohoCliq.MessageActions.UPDATE\n  description: Update message action configurations and manage message action handlers.\n  flows:\n  - implicit\n  sources:\n  - openapi/messageactions.yml\n- scope: ZohoCliq.Messages.CREATE\n  description: Send messages to users and chats\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/messagecards.yml\n  - openapi/messages.yml\n  - openapi/scheduledmessages.yml\n  - openapi/stars.yml\n- scope: ZohoCliq.Messages.DELETE\n  description: Delete Messages\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/chats.yml\n  - openapi/messages.yml\n  - openapi/scheduledmessages.yml\n  - openapi/stars.yml\n- scope: ZohoCliq.Messages.READ\n  description:\
  \ Read Messages\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/messages.yml\n  - openapi/scheduledmessages.yml\n  - openapi/stars.yml\n  - openapi/threads.yml\n- scope: ZohoCliq.Messages.UPDATE\n  description: Modify Messages\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/chats.yml\n  - openapi/messages.yml\n  - openapi/scheduledmessages.yml\n  - openapi/stars.yml\n- scope: ZohoCliq.Profile.DELETE\n  description: Delete user profile settings\n  flows:\n  - implicit\n  sources:\n  - openapi/keyboardshortcuts.yml\n- scope: ZohoCliq.Profile.READ\n  description: Read user profile settings\n  flows:\n  - implicit\n  sources:\n  - openapi/dndsettings.yml\n  - openapi/keyboardshortcuts.yml\n  - openapi/mobilesettings.yml\n  - openapi/userpreferences.yml\n- scope: ZohoCliq.Profile.UPDATE\n  description: Update user profile settings\n  flows:\n  - implicit\n  sources:\n  - openapi/dndsettings.yml\n  - openapi/keyboardshortcuts.yml\n  - openapi/mobilesettings.yml\n\
  \  - openapi/userpreferences.yml\n- scope: ZohoCliq.Reminders.CREATE\n  description: Create reminder notifications\n  flows:\n  - implicit\n  sources:\n  - openapi/reminders.yml\n- scope: ZohoCliq.Reminders.DELETE\n  description: Delete reminders\n  flows:\n  - implicit\n  sources:\n  - openapi/reminders.yml\n- scope: ZohoCliq.Reminders.READ\n  description: Read reminders\n  flows:\n  - implicit\n  sources:\n  - openapi/reminders.yml\n- scope: ZohoCliq.Reminders.UPDATE\n  description: Update reminders\n  flows:\n  - implicit\n  sources:\n  - openapi/reminders.yml\n- scope: ZohoCliq.Webhooks.CREATE\n  description: Post messages to conversations via webhooks\n  flows:\n  - implicit\n  sources:\n  - openapi/bots.yml\n  - openapi/buttons.yml\n  - openapi/mentions.yml\n  - openapi/messagecards.yml\n  - openapi/messageformat.yml\n  - openapi/messages.yml\n  - openapi/threads.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-cliq/refs/heads/main/scopes/zoho-cliq-scopes.yml
summary_line: 61 scopes · implicit/authorizationCode
tags:
- Messaging
- Team Collaboration
- Chat
- Bots
- Webhooks
- Slash Commands
- Communication
token_urls:
- https://accounts.zoho.com/oauth/v2/token
---
