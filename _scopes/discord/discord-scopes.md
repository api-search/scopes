---
api_specs:
- filename: discord-api-spec
  format: yaml
  label: Discord REST API
  slug: discord-rest-api
  spec_type: OpenAPI
  url: https://github.com/discord/discord-api-spec
- filename: discord-gateway-api-asyncapi.yml
  format: yaml
  label: Discord Gateway API
  slug: discord-gateway-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/asyncapi/discord-gateway-api-asyncapi.yml
- filename: discord-interactions-api-openapi.yml
  format: yaml
  label: Discord Interactions API
  slug: discord-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/openapi/discord-interactions-api-openapi.yml
- filename: discord-oauth2-api-openapi.yml
  format: yaml
  label: Discord OAuth2 API
  slug: discord-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/openapi/discord-oauth2-api-openapi.yml
- filename: discord-webhook-events-api-openapi.yml
  format: yaml
  label: Discord Webhook Events API
  slug: discord-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/openapi/discord-webhook-events-api-openapi.yml
- filename: discord-voice-api-asyncapi.yml
  format: yaml
  label: Discord Voice API
  slug: discord-voice-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/asyncapi/discord-voice-api-asyncapi.yml
- filename: discord-linked-roles-api-openapi.yml
  format: yaml
  label: Discord Linked Roles API
  slug: discord-linked-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/openapi/discord-linked-roles-api-openapi.yml
authorization_urls:
- discord.com/oauth2/authorize
- https://discord.com/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Discord Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Discord publishes 33 OAuth 2.0 scopes via the implicit, clientCredentials, and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Discord API on a user''s behalf.


  Tokens are issued from https://discord.com/api/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Discord
provider_slug: discord
schemes:
- flows:
  - authorizationUrl: discord.com/oauth2/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://discord.com/api/oauth2/token
  - authorizationUrl: discord.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://discord.com/api/oauth2/token
  name: OAuth2
  source: openapi/discord-openapi-original.yml
- flows:
  - authorizationUrl: https://discord.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://discord.com/api/v10/oauth2/token
  name: OAuth2
  source: openapi/discord-rest-api-openapi.yml
scope_count: 33
scope_names:
- activities.read
- activities.write
- applications.builds.read
- applications.builds.upload
- applications.commands
- applications.commands.permissions.update
- applications.commands.update
- applications.entitlements
- applications.store.update
- bot
- connections
- dm_channels.read
- email
- gdm.join
- guilds
- guilds.join
- guilds.members.read
- identify
- messages.read
- openid
- relationships.read
- role_connections.write
- rpc
- rpc.activities.write
- rpc.notifications.read
- rpc.screenshare.read
- rpc.screenshare.write
- rpc.video.read
- rpc.video.write
- rpc.voice.read
- rpc.voice.write
- voice
- webhook.incoming
scopes:
- description: allows your app to fetch data from a user's "Now Playing/Recently Played" list - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: activities.read
- description: allows your app to update a user's activity - requires Discord approval (NOT REQUIRED FOR GAMESDK ACTIVITY MANAGER)
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: activities.write
- description: allows your app to read build data for a user's applications
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: applications.builds.read
- description: allows your app to upload/update builds for a user's applications - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: applications.builds.upload
- description: allows your app to use commands in a guild
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: applications.commands
- description: allows your app to update permissions for its commands in a guild a user has permissions to
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: applications.commands.permissions.update
- description: allows your app to update its commands using a Bearer token - client credentials grant only
  flows:
  - clientCredentials
  scope: applications.commands.update
- description: allows your app to read entitlements for a user's applications
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: applications.entitlements
- description: allows your app to read and update store data (SKUs, store listings, achievements, etc.) for a user's applications
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: applications.store.update
- description: for oauth2 bots, this puts the bot in the user's selected guild by default
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: bot
- description: allows /users/@me/connections to return linked third-party accounts
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: connections
- description: allows your app to see information about the user's DMs and group DMs - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: dm_channels.read
- description: enables /users/@me to return an email
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: email
- description: allows your app to join users to a group dm
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: gdm.join
- description: allows /users/@me/guilds to return basic information about all of a user's guilds
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: guilds
- description: allows /guilds/{guild.id}/members/{user.id} to be used for joining users to a guild
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: guilds.join
- description: allows /users/@me/guilds/{guild.id}/member to return a user's member information in a guild
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: guilds.members.read
- description: allows /users/@me without email
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: identify
- description: for local rpc server api access, this allows you to read messages from all client channels (otherwise restricted to channels/guilds your app creates)
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: messages.read
- description: for OpenID Connect, this allows your app to receive user id and basic profile information
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: openid
- description: allows your app to know a user's friends and implicit relationships - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: relationships.read
- description: allows your app to update a user's connection and metadata for the app
  flows:
  - authorizationCode
  scope: role_connections.write
- description: for local rpc server access, this allows you to control a user's local Discord client - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: rpc
- description: for local rpc server access, this allows you to update a user's activity - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: rpc.activities.write
- description: for local rpc server access, this allows you to receive notifications pushed out to the user - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: rpc.notifications.read
- description: for local rpc server access, this allows you to read a user's screenshare status- requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: rpc.screenshare.read
- description: for local rpc server access, this allows you to update a user's screenshare settings- requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: rpc.screenshare.write
- description: for local rpc server access, this allows you to read a user's video status - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: rpc.video.read
- description: for local rpc server access, this allows you to update a user's video settings - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: rpc.video.write
- description: for local rpc server access, this allows you to read a user's voice settings and listen for voice events - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: rpc.voice.read
- description: for local rpc server access, this allows you to update a user's voice settings - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: rpc.voice.write
- description: allows your app to connect to voice on user's behalf and see all the voice members - requires Discord approval
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: voice
- description: this generates a webhook that is returned in the oauth token response for authorization code grants
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: webhook.incoming
slug: discord-scopes
source_filename: discord-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/discord-openapi-original.yml, openapi/discord-rest-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/discord-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: discord.com/oauth2/authorize\n  - flow: clientCredentials\n    tokenUrl: https://discord.com/api/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: discord.com/oauth2/authorize\n    tokenUrl: https://discord.com/api/oauth2/token\n- name: OAuth2\n  source: openapi/discord-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://discord.com/oauth2/authorize\n    tokenUrl: https://discord.com/api/v10/oauth2/token\nscopes:\n- scope: activities.read\n  description: allows your app to fetch data from a user's \"Now Playing/Recently Played\" list\n    - requires Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n\
  - scope: activities.write\n  description: allows your app to update a user's activity - requires Discord approval (NOT\n    REQUIRED FOR GAMESDK ACTIVITY MANAGER)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: applications.builds.read\n  description: allows your app to read build data for a user's applications\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: applications.builds.upload\n  description: allows your app to upload/update builds for a user's applications - requires\n    Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: applications.commands\n  description: allows your app to use commands in a guild\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n\
  \  - openapi/discord-rest-api-openapi.yml\n- scope: applications.commands.permissions.update\n  description: allows your app to update permissions for its commands in a guild a user has\n    permissions to\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: applications.commands.update\n  description: allows your app to update its commands using a Bearer token - client credentials\n    grant only\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: applications.entitlements\n  description: allows your app to read entitlements for a user's applications\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: applications.store.update\n  description: allows your app to read and update store data (SKUs, store listings, achievements,\n    etc.) for a user's applications\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: bot\n  description: for oauth2 bots, this puts the bot in the user's selected guild by default\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n  - openapi/discord-rest-api-openapi.yml\n- scope: connections\n  description: allows /users/@me/connections to return linked third-party accounts\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n  - openapi/discord-rest-api-openapi.yml\n- scope: dm_channels.read\n  description: allows your app to see information about the user's DMs and group DMs - requires\n    Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: email\n  description: enables /users/@me to return an email\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n  - openapi/discord-rest-api-openapi.yml\n- scope: gdm.join\n  description: allows your app to join users to a group dm\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: guilds\n  description: allows /users/@me/guilds to return basic information about all of a user's guilds\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n  - openapi/discord-rest-api-openapi.yml\n- scope: guilds.join\n  description: allows /guilds/{guild.id}/members/{user.id} to be used for joining users to a\n    guild\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n  - openapi/discord-rest-api-openapi.yml\n- scope: guilds.members.read\n  description: allows /users/@me/guilds/{guild.id}/member to\
  \ return a user's member information\n    in a guild\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: identify\n  description: allows /users/@me without email\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n  - openapi/discord-rest-api-openapi.yml\n- scope: messages.read\n  description: for local rpc server api access, this allows you to read messages from all client\n    channels (otherwise restricted to channels/guilds your app creates)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n  - openapi/discord-rest-api-openapi.yml\n- scope: openid\n  description: for OpenID Connect, this allows your app to receive user id and basic profile\n    information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n\
  - scope: relationships.read\n  description: allows your app to know a user's friends and implicit relationships - requires\n    Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: role_connections.write\n  description: allows your app to update a user's connection and metadata for the app\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: rpc\n  description: for local rpc server access, this allows you to control a user's local Discord\n    client - requires Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: rpc.activities.write\n  description: for local rpc server access, this allows you to update a user's activity - requires\n    Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n\
  - scope: rpc.notifications.read\n  description: for local rpc server access, this allows you to receive notifications pushed\n    out to the user - requires Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: rpc.screenshare.read\n  description: for local rpc server access, this allows you to read a user's screenshare status-\n    requires Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: rpc.screenshare.write\n  description: for local rpc server access, this allows you to update a user's screenshare settings-\n    requires Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: rpc.video.read\n  description: for local rpc server access, this allows you to read a user's video status -\n    requires\
  \ Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: rpc.video.write\n  description: for local rpc server access, this allows you to update a user's video settings\n    - requires Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: rpc.voice.read\n  description: for local rpc server access, this allows you to read a user's voice settings\n    and listen for voice events - requires Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: rpc.voice.write\n  description: for local rpc server access, this allows you to update a user's voice settings\n    - requires Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n\
  - scope: voice\n  description: allows your app to connect to voice on user's behalf and see all the voice members\n    - requires Discord approval\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n- scope: webhook.incoming\n  description: this generates a webhook that is returned in the oauth token response for authorization\n    code grants\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/discord-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discord/refs/heads/main/scopes/discord-scopes.yml
summary_line: 33 scopes · implicit/clientCredentials/authorizationCode
tags:
- Chat
- Communication
- Gaming
- Messaging
- Social
- Video
- Voice
token_urls:
- https://discord.com/api/oauth2/token
- https://discord.com/api/v10/oauth2/token
---
