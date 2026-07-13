---
api_specs:
- filename: battle-net-hearthstone-game-data.yaml
  format: yaml
  label: Hearthstone Game Data API
  slug: hearthstone-game-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/openapi/battle-net-hearthstone-game-data.yaml
authorization_urls: []
description: ''
docs: https://community.developer.battle.net/documentation/guides/using-oauth
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Battle Net Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Battle.net publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Battle.net API on a user''s behalf.


  Tokens are issued from https://oauth.battle.net/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Battle.net
provider_slug: battle-net
schemes:
- description: Battle.net OAuth 2.0 authentication. Use client credentials flow for game data APIs.
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.battle.net/token
  name: oauth2
  source: openapi/battle-net-hearthstone-game-data.yaml
scope_count: 4
scope_names:
- wow.profile
- sc2.profile
- d3.profile
- openid
scopes:
- description: Access to a user's World of Warcraft characters.
  flows: []
  scope: wow.profile
- description: Access to a user's StarCraft II profile.
  flows: []
  scope: sc2.profile
- description: Access to a user's Diablo III profile.
  flows: []
  scope: d3.profile
- description: Access details about a currently logged in user using OpenID Connect (OIDC).
  flows: []
  scope: openid
slug: battle-net-scopes
source_filename: battle-net-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/battle-net-hearthstone-game-data.yaml\ndocs: https://community.developer.battle.net/documentation/guides/using-oauth\nschemes:\n- name: oauth2\n  source: openapi/battle-net-hearthstone-game-data.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.battle.net/token\n  description: Battle.net OAuth 2.0 authentication. Use client credentials flow for game data\n    APIs.\nscopes:\n- scope: wow.profile\n  description: Access to a user's World of Warcraft characters.\n  sources:\n  - https://community.developer.battle.net/documentation/guides/using-oauth\n- scope: sc2.profile\n  description: Access to a user's StarCraft II profile.\n  sources:\n  - https://community.developer.battle.net/documentation/guides/using-oauth\n- scope: d3.profile\n  description: Access to a user's Diablo III profile.\n  sources:\n  - https://community.developer.battle.net/documentation/guides/using-oauth\n- scope: openid\n \
  \ description: Access details about a currently logged in user using OpenID Connect (OIDC).\n  sources:\n  - https://community.developer.battle.net/documentation/guides/using-oauth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/scopes/battle-net-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
token_urls:
- https://oauth.battle.net/token
---
