---
authorization_urls:
- https://id.twitch.tv/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Twitch Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Twitch publishes 42 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Twitch API on a user''s behalf.


  Tokens are issued from https://id.twitch.tv/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Twitch
provider_slug: twitch
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://id.twitch.tv/oauth2/token
  name: oauth2
  source: openapi/twitch-drops-openapi.yml
- flows:
  - authorizationUrl: https://id.twitch.tv/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://id.twitch.tv/oauth2/token
  name: oauth2
  source: openapi/twitch-extensions-openapi.yml
- description: OAuth 2.0 Authorization Code Flow
  flows:
  - authorizationUrl: https://id.twitch.tv/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://id.twitch.tv/oauth2/token
  name: oauth2
  source: openapi/twitch-helix-openapi.yml
- description: Twitch OAuth2 Client Credentials for IGDB access
  flows:
  - flow: clientCredentials
    tokenUrl: https://id.twitch.tv/oauth2/token
  name: oauth2
  source: openapi/twitch-igdb-openapi.yml
- flows:
  - authorizationUrl: https://id.twitch.tv/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://id.twitch.tv/oauth2/token
  name: oauth2
  source: openapi/twitch-insights-analytics-openapi.yml
scope_count: 42
scope_names:
- analytics:read:extensions
- analytics:read:games
- bits:read
- channel:edit:commercial
- channel:manage:broadcast
- channel:manage:moderators
- channel:manage:polls
- channel:manage:predictions
- channel:manage:raids
- channel:manage:redemptions
- channel:manage:schedule
- channel:manage:videos
- channel:read:editors
- channel:read:goals
- channel:read:hype_train
- channel:read:polls
- channel:read:predictions
- channel:read:redemptions
- channel:read:stream_key
- channel:read:subscriptions
- chat:edit
- chat:read
- clips:edit
- moderation:read
- moderator:manage:announcements
- moderator:manage:automod
- moderator:manage:banned_users
- moderator:manage:blocked_terms
- moderator:manage:chat_messages
- moderator:manage:chat_settings
- moderator:read:chatters
- moderator:read:followers
- user:edit
- user:edit:broadcast
- user:manage:blocked_users
- user:manage:whispers
- user:read:blocked_users
- user:read:broadcast
- user:read:email
- user:read:follows
- user:read:subscriptions
- whispers:read
scopes:
- description: View analytics data for extensions
  flows:
  - authorizationCode
  scope: analytics:read:extensions
- description: View analytics data for games
  flows:
  - authorizationCode
  scope: analytics:read:games
- description: View Bits information
  flows:
  - authorizationCode
  scope: bits:read
- description: Run commercials on a channel
  flows:
  - authorizationCode
  scope: channel:edit:commercial
- description: Manage a channel's broadcast configuration
  flows:
  - authorizationCode
  scope: channel:manage:broadcast
- description: Add and remove channel moderators
  flows:
  - authorizationCode
  scope: channel:manage:moderators
- description: Manage a channel's polls
  flows:
  - authorizationCode
  scope: channel:manage:polls
- description: Manage a channel's predictions
  flows:
  - authorizationCode
  scope: channel:manage:predictions
- description: Manage a channel's raids
  flows:
  - authorizationCode
  scope: channel:manage:raids
- description: Manage channel points custom rewards and their redemptions
  flows:
  - authorizationCode
  scope: channel:manage:redemptions
- description: Manage a channel's stream schedule
  flows:
  - authorizationCode
  scope: channel:manage:schedule
- description: Manage a channel's videos
  flows:
  - authorizationCode
  scope: channel:manage:videos
- description: View a channel's editors
  flows:
  - authorizationCode
  scope: channel:read:editors
- description: View a channel's goals
  flows:
  - authorizationCode
  scope: channel:read:goals
- description: View Hype Train information
  flows:
  - authorizationCode
  scope: channel:read:hype_train
- description: View a channel's polls
  flows:
  - authorizationCode
  scope: channel:read:polls
- description: View a channel's predictions
  flows:
  - authorizationCode
  scope: channel:read:predictions
- description: View channel points custom rewards and their redemptions
  flows:
  - authorizationCode
  scope: channel:read:redemptions
- description: Read an authorized user's stream key
  flows:
  - authorizationCode
  scope: channel:read:stream_key
- description: View a channel's subscribers
  flows:
  - authorizationCode
  scope: channel:read:subscriptions
- description: Send live stream chat messages
  flows:
  - authorizationCode
  scope: chat:edit
- description: View live stream chat messages
  flows:
  - authorizationCode
  scope: chat:read
- description: Create clips
  flows:
  - authorizationCode
  scope: clips:edit
- description: View a channel's moderation data
  flows:
  - authorizationCode
  scope: moderation:read
- description: Send announcements in channels
  flows:
  - authorizationCode
  scope: moderator:manage:announcements
- description: Manage messages held by AutoMod
  flows:
  - authorizationCode
  scope: moderator:manage:automod
- description: Ban and unban users
  flows:
  - authorizationCode
  scope: moderator:manage:banned_users
- description: Manage blocked terms
  flows:
  - authorizationCode
  scope: moderator:manage:blocked_terms
- description: Delete chat messages
  flows:
  - authorizationCode
  scope: moderator:manage:chat_messages
- description: Manage chat settings
  flows:
  - authorizationCode
  scope: moderator:manage:chat_settings
- description: View the chatters in a channel
  flows:
  - authorizationCode
  scope: moderator:read:chatters
- description: Read the followers of a channel
  flows:
  - authorizationCode
  scope: moderator:read:followers
- description: Manage a user's account
  flows:
  - authorizationCode
  scope: user:edit
- description: Edit a user's broadcasting configuration
  flows:
  - authorizationCode
  scope: user:edit:broadcast
- description: Manage user's block list
  flows:
  - authorizationCode
  scope: user:manage:blocked_users
- description: Send whisper messages
  flows:
  - authorizationCode
  scope: user:manage:whispers
- description: View a user's block list
  flows:
  - authorizationCode
  scope: user:read:blocked_users
- description: View a user's broadcasting configuration
  flows:
  - authorizationCode
  scope: user:read:broadcast
- description: View a user's email address
  flows:
  - authorizationCode
  scope: user:read:email
- description: View the list of channels a user follows
  flows:
  - authorizationCode
  scope: user:read:follows
- description: View a user's subscriptions
  flows:
  - authorizationCode
  scope: user:read:subscriptions
- description: View whisper messages
  flows:
  - authorizationCode
  scope: whispers:read
slug: twitch-scopes
source_filename: twitch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/twitch-drops-openapi.yml, openapi/twitch-extensions-openapi.yml, openapi/twitch-helix-openapi.yml,\n  openapi/twitch-igdb-openapi.yml, openapi/twitch-insights-analytics-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/twitch-drops-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.twitch.tv/oauth2/token\n- name: oauth2\n  source: openapi/twitch-extensions-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.twitch.tv/oauth2/authorize\n    tokenUrl: https://id.twitch.tv/oauth2/token\n- name: oauth2\n  source: openapi/twitch-helix-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.twitch.tv/oauth2/authorize\n    tokenUrl: https://id.twitch.tv/oauth2/token\n  description: OAuth 2.0 Authorization Code Flow\n- name: oauth2\n  source: openapi/twitch-igdb-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.twitch.tv/oauth2/token\n\
  \  description: Twitch OAuth2 Client Credentials for IGDB access\n- name: oauth2\n  source: openapi/twitch-insights-analytics-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.twitch.tv/oauth2/authorize\n    tokenUrl: https://id.twitch.tv/oauth2/token\nscopes:\n- scope: analytics:read:extensions\n  description: View analytics data for extensions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n  - openapi/twitch-insights-analytics-openapi.yml\n- scope: analytics:read:games\n  description: View analytics data for games\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n  - openapi/twitch-insights-analytics-openapi.yml\n- scope: bits:read\n  description: View Bits information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:edit:commercial\n  description: Run commercials on a channel\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n\
  - scope: channel:manage:broadcast\n  description: Manage a channel's broadcast configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:manage:moderators\n  description: Add and remove channel moderators\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:manage:polls\n  description: Manage a channel's polls\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:manage:predictions\n  description: Manage a channel's predictions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:manage:raids\n  description: Manage a channel's raids\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:manage:redemptions\n  description: Manage channel points custom rewards and their redemptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n\
  - scope: channel:manage:schedule\n  description: Manage a channel's stream schedule\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:manage:videos\n  description: Manage a channel's videos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:read:editors\n  description: View a channel's editors\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:read:goals\n  description: View a channel's goals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:read:hype_train\n  description: View Hype Train information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:read:polls\n  description: View a channel's polls\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:read:predictions\n  description: View a\
  \ channel's predictions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:read:redemptions\n  description: View channel points custom rewards and their redemptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:read:stream_key\n  description: Read an authorized user's stream key\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: channel:read:subscriptions\n  description: View a channel's subscribers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: chat:edit\n  description: Send live stream chat messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: chat:read\n  description: View live stream chat messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: clips:edit\n  description: Create clips\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: moderation:read\n  description: View a channel's moderation data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: moderator:manage:announcements\n  description: Send announcements in channels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: moderator:manage:automod\n  description: Manage messages held by AutoMod\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: moderator:manage:banned_users\n  description: Ban and unban users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: moderator:manage:blocked_terms\n  description: Manage blocked terms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: moderator:manage:chat_messages\n  description: Delete chat messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n\
  - scope: moderator:manage:chat_settings\n  description: Manage chat settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: moderator:read:chatters\n  description: View the chatters in a channel\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: moderator:read:followers\n  description: Read the followers of a channel\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: user:edit\n  description: Manage a user's account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: user:edit:broadcast\n  description: Edit a user's broadcasting configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-extensions-openapi.yml\n- scope: user:manage:blocked_users\n  description: Manage user's block list\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: user:manage:whispers\n\
  \  description: Send whisper messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: user:read:blocked_users\n  description: View a user's block list\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: user:read:broadcast\n  description: View a user's broadcasting configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-extensions-openapi.yml\n  - openapi/twitch-helix-openapi.yml\n- scope: user:read:email\n  description: View a user's email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: user:read:follows\n  description: View the list of channels a user follows\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: user:read:subscriptions\n  description: View a user's subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n- scope: whispers:read\n\
  \  description: View whisper messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitch-helix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/scopes/twitch-scopes.yml
summary_line: 42 scopes · clientCredentials/authorizationCode
tags:
- Entertainment
- Gaming
- Live Video
- Streaming
- Video
token_urls:
- https://id.twitch.tv/oauth2/token
---
