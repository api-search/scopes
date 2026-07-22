---
api_specs:
- filename: streamelements-openapi-original.yml
  format: yaml
  label: StreamElements API
  slug: streamelements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamelements/refs/heads/main/openapi/streamelements-openapi-original.yml
authorization_urls:
- https://api.streamelements.com/oauth2/authorize
description: ''
docs: https://dev.streamelements.com/docs/api-docs/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Streamelements Scopes
name_suffix: OAuth Scopes
note: Baseline scopes derived from the OpenAPI OAuth2 flow, upgraded from the SE developer docs (OAuth2 + WebSocket topic references). Some scopes (overlays:broadcast, stream-live:read, tips:moderation, session:read) are documented on the Astro WebSocket topic pages but not enumerated in the OpenAPI flow.
overview: 'StreamElements publishes 20 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the StreamElements API on a user''s behalf.


  Tokens are issued from https://api.streamelements.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: StreamElements
provider_slug: streamelements
schemes:
- flows:
  - authorizationUrl: https://api.streamelements.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.streamelements.com/oauth2/token
  name: OAuth2
  source: openapi/streamelements-openapi-original.yml
scope_count: 20
scope_names:
- activities:read
- activities:write
- bot:read
- bot:write
- contest:read
- contest:write
- giveaway:read
- giveaway:write
- loyalty:read
- loyalty:write
- overlays:broadcast
- overlays:read
- overlays:write
- session:read
- store:read
- store:write
- stream-live:read
- tips:moderation
- tips:read
- tips:write
scopes:
- description: Grants read of activities
  flows:
  - authorizationCode
  scope: activities:read
- description: Grants create activities
  flows:
  - authorizationCode
  scope: activities:write
- description: Grants read timers, commands, spam filters and modules
  flows:
  - authorizationCode
  scope: bot:read
- description: Grants create and update timers, commands, spam filters and modules
  flows:
  - authorizationCode
  scope: bot:write
- description: Grants read of contests
  flows:
  - authorizationCode
  scope: contest:read
- description: Grants create and update contests
  flows:
  - authorizationCode
  scope: contest:write
- description: Grants read of giveaways
  flows:
  - authorizationCode
  scope: giveaway:read
- description: Grants create and update giveaways
  flows:
  - authorizationCode
  scope: giveaway:write
- description: Grants read of loyalty settings and the leaderboard
  flows:
  - authorizationCode
  scope: loyalty:read
- description: Grants update of loyalty settings and update the leaderboard
  flows:
  - authorizationCode
  scope: loyalty:write
- description: Send/receive overlay broadcast messages (Astro channel.overlay.broadcast topic).
  flows:
  - authorizationCode
  scope: overlays:broadcast
- description: Grants read overlays
  flows:
  - authorizationCode
  scope: overlays:read
- description: Grants creation, update, deletion of overlays
  flows:
  - authorizationCode
  scope: overlays:write
- description: Grants read of session data
  flows:
  - authorizationCode
  scope: session:read
- description: Grants read redemptions and items
  flows:
  - authorizationCode
  scope: store:read
- description: Grants create new store items and complete redemptions
  flows:
  - authorizationCode
  scope: store:write
- description: Read stream live/offline status (Astro channel.stream.status topic).
  flows:
  - authorizationCode
  scope: stream-live:read
- description: Read tip moderation state (Astro channel.tips.moderation topic).
  flows:
  - authorizationCode
  scope: tips:moderation
- description: Ability read of tips
  flows:
  - authorizationCode
  scope: tips:read
- description: Grants create/modify/delete tips
  flows:
  - authorizationCode
  scope: tips:write
slug: streamelements-scopes
source_filename: streamelements-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/streamelements-openapi-original.yml\nschemes:\n- name: OAuth2\n  source: openapi/streamelements-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.streamelements.com/oauth2/authorize\n    tokenUrl: https://api.streamelements.com/oauth2/token\nscopes:\n- scope: activities:read\n  description: Grants read of activities\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: activities:write\n  description: Grants create activities\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: bot:read\n  description: Grants read timers, commands, spam filters and modules\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: bot:write\n  description: Grants create and update timers, commands, spam filters and modules\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: contest:read\n  description: Grants read of contests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: contest:write\n  description: Grants create and update contests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: giveaway:read\n  description: Grants read of giveaways\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: giveaway:write\n  description: Grants create and update giveaways\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: loyalty:read\n  description: Grants read of loyalty settings and the leaderboard\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: loyalty:write\n  description: Grants update of loyalty settings and update the leaderboard\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: overlays:broadcast\n  description: Send/receive overlay broadcast messages (Astro channel.overlay.broadcast topic).\n  flows:\n  - authorizationCode\n  sources:\n  - https://dev.streamelements.com/docs/websockets\n- scope: overlays:read\n  description: Grants read overlays\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: overlays:write\n  description: Grants creation, update, deletion of overlays\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: session:read\n  description: Grants read of session data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: store:read\n  description: Grants read redemptions and items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: store:write\n\
  \  description: Grants create new store items and complete redemptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: stream-live:read\n  description: Read stream live/offline status (Astro channel.stream.status topic).\n  flows:\n  - authorizationCode\n  sources:\n  - https://dev.streamelements.com/docs/websockets\n- scope: tips:moderation\n  description: Read tip moderation state (Astro channel.tips.moderation topic).\n  flows:\n  - authorizationCode\n  sources:\n  - https://dev.streamelements.com/docs/websockets\n- scope: tips:read\n  description: Ability read of tips\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\n- scope: tips:write\n  description: Grants create/modify/delete tips\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamelements-openapi-original.yml\ndocs: https://dev.streamelements.com/docs/api-docs/authentication\nnote: Baseline scopes derived from the\
  \ OpenAPI OAuth2 flow, upgraded from the SE developer docs (OAuth2\n  + WebSocket topic references). Some scopes (overlays:broadcast, stream-live:read, tips:moderation, session:read)\n  are documented on the Astro WebSocket topic pages but not enumerated in the OpenAPI flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamelements/refs/heads/main/scopes/streamelements-scopes.yml
summary_line: 20 scopes · authorizationCode
tags:
- Company
- Consumer
- Live Streaming
- Creator Economy
- Overlays
- Chatbot
- Monetization
- Donations
- Loyalty Points
- Giveaways
- Video
- Twitch
- YouTube
- Real-Time
- WebSockets
- Webhooks
- REST
token_urls:
- https://api.streamelements.com/oauth2/token
---
