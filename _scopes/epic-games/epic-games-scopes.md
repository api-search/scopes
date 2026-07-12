---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Epic Games Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Epic Games publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Epic Games API on a user''s behalf.


  Tokens are issued from https://api.epicgames.dev/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Epic Games
provider_slug: epic-games
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.epicgames.dev/auth/v1/oauth/token
  name: oauthClientCredentials
  source: openapi/epic-games-openapi.yml
scope_count: 1
scope_names:
- basic_profile
scopes:
- description: Basic profile access
  flows:
  - clientCredentials
  scope: basic_profile
slug: epic-games-scopes
source_filename: epic-games-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/epic-games-openapi.yml\nschemes:\n- name: oauthClientCredentials\n  source: openapi/epic-games-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.epicgames.dev/auth/v1/oauth/token\nscopes:\n- scope: basic_profile\n  description: Basic profile access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/epic-games-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epic-games/refs/heads/main/scopes/epic-games-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Achievements
- Anti-Cheat
- Cross-Platform
- EOS
- Epic Online Services
- Game Backend
- Game Development
- Games
- Identity
- Lobby
- Matchmaking
- Multiplayer
- Sessions
- Unreal Engine
- Voice
token_urls:
- https://api.epicgames.dev/auth/v1/oauth/token
---
