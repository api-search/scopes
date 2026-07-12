---
authorization_urls:
- https://oauth.battle.net/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Activision Blizzard Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'activision-blizzard publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the activision-blizzard API on a user''s behalf.


  Tokens are issued from https://oauth.battle.net/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: activision-blizzard
provider_slug: activision-blizzard
schemes:
- description: OAuth2 authentication. Create a client at develop.battle.net for client ID and secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.battle.net/token
  - authorizationUrl: https://oauth.battle.net/authorize
    flow: authorizationCode
    tokenUrl: https://oauth.battle.net/token
  name: OAuth2ClientCredentials
  source: openapi/activision-blizzard-battle-net.json
scope_count: 3
scope_names:
- openid
- sc2.profile
- wow.profile
scopes:
- description: Access basic account information
  flows:
  - authorizationCode
  - clientCredentials
  scope: openid
- description: Access StarCraft II profile data
  flows:
  - authorizationCode
  - clientCredentials
  scope: sc2.profile
- description: Access WoW character profile data
  flows:
  - authorizationCode
  - clientCredentials
  scope: wow.profile
slug: activision-blizzard-scopes
source_filename: activision-blizzard-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/activision-blizzard-battle-net.json\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/activision-blizzard-battle-net.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.battle.net/token\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.battle.net/authorize\n    tokenUrl: https://oauth.battle.net/token\n  description: OAuth2 authentication. Create a client at develop.battle.net for client ID and\n    secret.\nscopes:\n- scope: openid\n  description: Access basic account information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/activision-blizzard-battle-net.json\n- scope: sc2.profile\n  description: Access StarCraft II profile data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/activision-blizzard-battle-net.json\n- scope: wow.profile\n  description: Access WoW character profile data\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/activision-blizzard-battle-net.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/scopes/activision-blizzard-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Fortune 1000
token_urls:
- https://oauth.battle.net/token
---
