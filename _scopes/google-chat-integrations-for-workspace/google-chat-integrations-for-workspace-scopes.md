---
api_specs:
- filename: google-chat-integrations-for-workspace-spaces-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Spaces API
  slug: google-chat-integrations-for-workspace-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat-integrations-for-workspace/openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml
- filename: google-chat-integrations-for-workspace-media-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Chat Integrations For Workspace Media API
  slug: google-chat-integrations-for-workspace-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat-integrations-for-workspace/openapi/google-chat-integrations-for-workspace-media-api-openapi.yml
- filename: google-chat-integrations-for-workspace-users-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Chat Integrations For Workspace Users API
  slug: google-chat-integrations-for-workspace-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat-integrations-for-workspace/openapi/google-chat-integrations-for-workspace-users-api-openapi.yml
- filename: google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Custom Emojis API
  slug: google-chat-integrations-for-workspace-custom-emojis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat-integrations-for-workspace/openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Chat Integrations for Workspace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Chat Integrations for Workspace publishes 41 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Chat Integrations for Workspace API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Chat Integrations for Workspace
provider_slug: google-chat-integrations-for-workspace
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-chat-integrations-for-workspace-media-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-chat-integrations-for-workspace-users-api-openapi.yml
scope_count: 41
scope_names:
- https://www.googleapis.com/auth/chat.admin.delete
- https://www.googleapis.com/auth/chat.admin.memberships
- https://www.googleapis.com/auth/chat.admin.memberships.readonly
- https://www.googleapis.com/auth/chat.admin.spaces
- https://www.googleapis.com/auth/chat.admin.spaces.readonly
- https://www.googleapis.com/auth/chat.app.all.memberships.readonly
- https://www.googleapis.com/auth/chat.app.all.messages.readonly
- https://www.googleapis.com/auth/chat.app.all.spaces.readonly
- https://www.googleapis.com/auth/chat.app.delete
- https://www.googleapis.com/auth/chat.app.memberships
- https://www.googleapis.com/auth/chat.app.memberships.readonly
- https://www.googleapis.com/auth/chat.app.messages.readonly
- https://www.googleapis.com/auth/chat.app.spaces
- https://www.googleapis.com/auth/chat.app.spaces.create
- https://www.googleapis.com/auth/chat.app.spaces.readonly
- https://www.googleapis.com/auth/chat.bot
- https://www.googleapis.com/auth/chat.customemojis
- https://www.googleapis.com/auth/chat.customemojis.readonly
- https://www.googleapis.com/auth/chat.delete
- https://www.googleapis.com/auth/chat.import
- https://www.googleapis.com/auth/chat.memberships
- https://www.googleapis.com/auth/chat.memberships.app
- https://www.googleapis.com/auth/chat.memberships.readonly
- https://www.googleapis.com/auth/chat.messages
- https://www.googleapis.com/auth/chat.messages.create
- https://www.googleapis.com/auth/chat.messages.reactions
- https://www.googleapis.com/auth/chat.messages.reactions.create
- https://www.googleapis.com/auth/chat.messages.reactions.readonly
- https://www.googleapis.com/auth/chat.messages.readonly
- https://www.googleapis.com/auth/chat.spaces
- https://www.googleapis.com/auth/chat.spaces.create
- https://www.googleapis.com/auth/chat.spaces.pins
- https://www.googleapis.com/auth/chat.spaces.pins.readonly
- https://www.googleapis.com/auth/chat.spaces.readonly
- https://www.googleapis.com/auth/chat.users.availability
- https://www.googleapis.com/auth/chat.users.availability.readonly
- https://www.googleapis.com/auth/chat.users.readstate
- https://www.googleapis.com/auth/chat.users.readstate.readonly
- https://www.googleapis.com/auth/chat.users.sections
- https://www.googleapis.com/auth/chat.users.sections.readonly
- https://www.googleapis.com/auth/chat.users.spacesettings
scopes:
- description: Delete conversations and spaces owned by your organization and remove access to associated files in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.admin.delete
- description: View, add, update and remove members and managers in conversations owned by your organization
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.admin.memberships
- description: View members and managers in conversations owned by your organization
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.admin.memberships.readonly
- description: View or edit display name, description, and other metadata for all Google Chat conversations owned by your organization
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.admin.spaces
- description: View display name, description, and other metadata for all Google Chat conversations owned by your organization
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.admin.spaces.readonly
- description: On their own behalf, apps in Google Chat can see all members in Google Chat spaces and conversations throughout your Workspace organization, even when the Chat app isn't a member
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.all.memberships.readonly
- description: On their own behalf, apps in Google Chat can see all messages and reactions throughout your Workspace organization, even when the Chat app isn't a member of a space or conversation
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.all.messages.readonly
- description: On their own behalf, apps in Google Chat can see metadata about all spaces and conversations in Google Chat throughout your Workspace organization, even when the Chat app isn't a member
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.all.spaces.readonly
- description: On their own behalf, apps in Google Chat can delete conversations and spaces and remove access to associated files
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.delete
- description: On their own behalf, apps in Google Chat can see, add, update, and remove members from conversations and spaces
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.memberships
- description: On their own behalf, apps in Google Chat can see members of conversations and spaces
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.memberships.readonly
- description: On their own behalf, apps in Google Chat can see all messages and their associated reactions and message content
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.messages.readonly
- description: On their own behalf, apps in Google Chat can create conversations and spaces and see or update their metadata (including history settings and access settings)
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.spaces
- description: On their own behalf, apps in Google Chat can create conversations and spaces
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.spaces.create
- description: On their own behalf, apps in Google Chat can see conversations and spaces and their metadata (including history settings and access settings)
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.app.spaces.readonly
- description: 'Private Service: https://www.googleapis.com/auth/chat.bot'
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.bot
- description: View, create, and delete custom emoji in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.customemojis
- description: View custom emoji in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.customemojis.readonly
- description: Delete conversations and spaces and remove access to associated files in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.delete
- description: Import spaces, messages, and memberships into Google Chat.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.import
- description: See, add, update, and remove members from conversations and spaces in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.memberships
- description: Add and remove itself from conversations and spaces in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.memberships.app
- description: View members in Google Chat conversations.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.memberships.readonly
- description: See, compose, send, update, and delete messages, their content, and attached cards; add, see, and delete reactions to messages.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.messages
- description: Compose and send messages and attach cards
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.messages.create
- description: See, add, and delete reactions as well as their reaction content to messages in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.messages.reactions
- description: Add reactions to messages in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.messages.reactions.create
- description: View reactions as well as their reaction content to messages in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.messages.reactions.readonly
- description: See messages as well as their reactions and message content in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.messages.readonly
- description: Create conversations and spaces and see or update metadata (including history settings and access settings) in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.spaces
- description: Create new conversations and spaces in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.spaces.create
- description: See, add, and remove pins in your Google Chat spaces
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.spaces.pins
- description: See pins in your Google Chat spaces
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.spaces.pins.readonly
- description: View chat and spaces in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.spaces.readonly
- description: See and change your availability status in Google Chat.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.users.availability
- description: See your availability status in Google Chat.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.users.availability.readonly
- description: View and modify last read time for Google Chat conversations
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.users.readstate
- description: View last read time for Google Chat conversations
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.users.readstate.readonly
- description: View, create, update, and delete your sections in Google Chat; move and list your section items in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.users.sections
- description: View your sections and their section items in Google Chat
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.users.sections.readonly
- description: Read and update your space settings
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chat.users.spacesettings
slug: google-chat-integrations-for-workspace-scopes
source_filename: google-chat-integrations-for-workspace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml, openapi/google-chat-integrations-for-workspace-media-api-openapi.yml,\n  openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml, openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/chat.admin.delete\n  description: Delete conversations and spaces owned by your organization and remove access\n    to associated files in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.admin.memberships\n  description:\
  \ View, add, update and remove members and managers in conversations owned by your\n    organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.admin.memberships.readonly\n  description: View members and managers in conversations owned by your organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.admin.spaces\n\
  \  description: View or edit display name, description, and other metadata for all Google Chat\n    conversations owned by your organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.admin.spaces.readonly\n  description: View display name, description, and other metadata for all Google Chat conversations\n    owned by your organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/chat.app.all.memberships.readonly\n  description: On their own behalf, apps in Google Chat can see all members in Google Chat spaces\n    and conversations throughout your Workspace organization, even when the Chat app isn't a\n    member\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.app.all.messages.readonly\n  description: On their own behalf, apps in Google Chat can see all messages and reactions throughout\n    your Workspace organization, even when the Chat app isn't a member of a space or conversation\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n\
  \  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.app.all.spaces.readonly\n  description: On their own behalf, apps in Google Chat can see metadata about all spaces and\n    conversations in Google Chat throughout your Workspace organization, even when the Chat\n    app isn't a member\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.app.delete\n  description: On their own behalf, apps in Google Chat can delete conversations and\
  \ spaces\n    and remove access to associated files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.app.memberships\n  description: On their own behalf, apps in Google Chat can see, add, update, and remove members\n    from conversations and spaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.app.memberships.readonly\n\
  \  description: On their own behalf, apps in Google Chat can see members of conversations and\n    spaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.app.messages.readonly\n  description: On their own behalf, apps in Google Chat can see all messages and their associated\n    reactions and message content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/chat.app.spaces\n  description: On their own behalf, apps in Google Chat can create conversations and spaces\n    and see or update their metadata (including history settings and access settings)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.app.spaces.create\n  description: On their own behalf, apps in Google Chat can create conversations and spaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n\
  \  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.app.spaces.readonly\n  description: On their own behalf, apps in Google Chat can see conversations and spaces and\n    their metadata (including history settings and access settings)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.bot\n  description: 'Private Service: https://www.googleapis.com/auth/chat.bot'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n\
  \  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.customemojis\n  description: View, create, and delete custom emoji in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.customemojis.readonly\n  description: View custom emoji in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/chat.delete\n  description: Delete conversations and spaces and remove access to associated files in Google\n    Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.import\n  description: Import spaces, messages, and memberships into Google Chat.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.memberships\n\
  \  description: See, add, update, and remove members from conversations and spaces in Google\n    Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.memberships.app\n  description: Add and remove itself from conversations and spaces in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.memberships.readonly\n\
  \  description: View members in Google Chat conversations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.messages\n  description: See, compose, send, update, and delete messages, their content, and attached\n    cards; add, see, and delete reactions to messages.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.messages.create\n\
  \  description: Compose and send messages and attach cards\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.messages.reactions\n  description: See, add, and delete reactions as well as their reaction content to messages\n    in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.messages.reactions.create\n\
  \  description: Add reactions to messages in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.messages.reactions.readonly\n  description: View reactions as well as their reaction content to messages in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.messages.readonly\n  description:\
  \ See messages as well as their reactions and message content in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.spaces\n  description: Create conversations and spaces and see or update metadata (including history\n    settings and access settings) in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.spaces.create\n\
  \  description: Create new conversations and spaces in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.spaces.pins\n  description: See, add, and remove pins in your Google Chat spaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.spaces.pins.readonly\n  description: See pins in your Google\
  \ Chat spaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.spaces.readonly\n  description: View chat and spaces in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.users.availability\n  description: See and change your availability status in Google Chat.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.users.availability.readonly\n  description: See your availability status in Google Chat.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.users.readstate\n  description: View and modify last read time for Google Chat conversations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n\
  \  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.users.readstate.readonly\n  description: View last read time for Google Chat conversations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.users.sections\n  description: View, create, update, and delete your sections in Google Chat; move and list\n    your section items in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n\
  \  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.users.sections.readonly\n  description: View your sections and their section items in Google Chat\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/chat.users.spacesettings\n  description: Read and update your space settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-custom-emojis-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-media-api-openapi.yml\n\
  \  - openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml\n  - openapi/google-chat-integrations-for-workspace-users-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-chat-integrations-for-workspace/scopes/google-chat-integrations-for-workspace-scopes.yml
summary_line: 41 scopes · authorizationCode
tags:
- Google Workspace
- Team Chat
- Messaging
- Collaboration
- Chat Apps
- Spaces
- Slash Commands
- Bots
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
