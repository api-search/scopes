---
api_specs:
- filename: lichess-openapi.yml
  format: yaml
  label: Lichess API
  slug: lichess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lichess/refs/heads/main/openapi/lichess-openapi.yml
authorization_urls:
- https://lichess.org/oauth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Lichess Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lichess publishes 23 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lichess API on a user''s behalf.


  Tokens are issued from https://lichess.org/api/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lichess
provider_slug: lichess
schemes:
- description: Read [the introduction for how to make authenticated requests](#description/authentication).
  flows:
  - authorizationUrl: https://lichess.org/oauth
    flow: authorizationCode
    tokenUrl: https://lichess.org/api/token
  name: OAuth2
  source: openapi/lichess-openapi.yml
scope_count: 23
scope_names:
- board:play
- bot:play
- challenge:bulk
- challenge:read
- challenge:write
- email:read
- engine:read
- engine:write
- follow:read
- follow:write
- msg:write
- preference:read
- preference:write
- puzzle:read
- puzzle:write
- racer:write
- study:read
- study:write
- team:lead
- team:read
- team:write
- tournament:write
- web:mod
scopes:
- description: Play with the Board API
  flows:
  - authorizationCode
  scope: board:play
- description: Play with the Bot API. Only for [Bot accounts](#tag/bot/POST/api/bot/account/upgrade)
  flows:
  - authorizationCode
  scope: bot:play
- description: Create, delete, query bulk pairings
  flows:
  - authorizationCode
  scope: challenge:bulk
- description: Read incoming challenges
  flows:
  - authorizationCode
  scope: challenge:read
- description: Create, accept, decline challenges
  flows:
  - authorizationCode
  scope: challenge:write
- description: Read your email address
  flows:
  - authorizationCode
  scope: email:read
- description: Read your external engines
  flows:
  - authorizationCode
  scope: engine:read
- description: Create, update, delete your external engines
  flows:
  - authorizationCode
  scope: engine:write
- description: Read followed players
  flows:
  - authorizationCode
  scope: follow:read
- description: Follow and unfollow other players
  flows:
  - authorizationCode
  scope: follow:write
- description: Send private messages to other players
  flows:
  - authorizationCode
  scope: msg:write
- description: Read your preferences
  flows:
  - authorizationCode
  scope: preference:read
- description: Write your preferences
  flows:
  - authorizationCode
  scope: preference:write
- description: Read puzzle activity
  flows:
  - authorizationCode
  scope: puzzle:read
- description: Write puzzle activity
  flows:
  - authorizationCode
  scope: puzzle:write
- description: Create and join puzzle races
  flows:
  - authorizationCode
  scope: racer:write
- description: Read private studies and broadcasts
  flows:
  - authorizationCode
  scope: study:read
- description: Create, update, delete studies and broadcasts
  flows:
  - authorizationCode
  scope: study:write
- description: Manage teams (kick members, send PMs)
  flows:
  - authorizationCode
  scope: team:lead
- description: Read private team information
  flows:
  - authorizationCode
  scope: team:read
- description: Join, leave teams
  flows:
  - authorizationCode
  scope: team:write
- description: Create tournaments
  flows:
  - authorizationCode
  scope: tournament:write
- description: Use moderator tools (within the bounds of your permissions)
  flows:
  - authorizationCode
  scope: web:mod
slug: lichess-scopes
source_filename: lichess-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lichess-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/lichess-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lichess.org/oauth\n    tokenUrl: https://lichess.org/api/token\n  description: Read [the introduction for how to make authenticated requests](#description/authentication).\nscopes:\n- scope: board:play\n  description: Play with the Board API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: bot:play\n  description: Play with the Bot API. Only for [Bot accounts](#tag/bot/POST/api/bot/account/upgrade)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: challenge:bulk\n  description: Create, delete, query bulk pairings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: challenge:read\n  description: Read incoming challenges\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/lichess-openapi.yml\n- scope: challenge:write\n  description: Create, accept, decline challenges\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: email:read\n  description: Read your email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: engine:read\n  description: Read your external engines\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: engine:write\n  description: Create, update, delete your external engines\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: follow:read\n  description: Read followed players\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: follow:write\n  description: Follow and unfollow other players\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: msg:write\n  description: Send private messages to other\
  \ players\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: preference:read\n  description: Read your preferences\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: preference:write\n  description: Write your preferences\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: puzzle:read\n  description: Read puzzle activity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: puzzle:write\n  description: Write puzzle activity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: racer:write\n  description: Create and join puzzle races\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: study:read\n  description: Read private studies and broadcasts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: study:write\n  description: Create, update,\
  \ delete studies and broadcasts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: team:lead\n  description: Manage teams (kick members, send PMs)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: team:read\n  description: Read private team information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: team:write\n  description: Join, leave teams\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: tournament:write\n  description: Create tournaments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n- scope: web:mod\n  description: Use moderator tools (within the bounds of your permissions)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lichess-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lichess/refs/heads/main/scopes/lichess-scopes.yml
summary_line: 23 scopes · authorizationCode
tags:
- Chess
- Games
- Open Source
- Nonprofit
- Tournaments
- Puzzles
- Bots
- Streaming
- ND-JSON
- OAuth
token_urls:
- https://lichess.org/api/token
---
