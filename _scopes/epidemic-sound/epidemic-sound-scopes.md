---
authorization_urls:
- https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/auth
description: ''
docs: https://developers.epidemicsound.com/docs/auth/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Epidemic Sound Scopes
name_suffix: OAuth Scopes
note: Epidemic Sound Connect uses OpenID Connect (authorization code + PKCE) but publishes no OAuth scopes reference — the auth docs (https://developers.epidemicsound.com/docs/auth/) show no scope parameter, and access is governed by the partnership agreement and the user's subscription tier rather than scopes (a token-response example shows only standard OIDC "email profile").
overview: 'Epidemic Sound uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Epidemic Sound
provider_slug: epidemic-sound
schemes:
- description: 'For users signing in with an Epidemic Sound account, user authentication is

    handled with OpenID Connect, which is a layer on top of OAuth 2.0.


    > **Example Header:** `Authorization: Bearer es-connect-token`'
  flows:
  - authorizationUrl: https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/token
  name: EpidemicSoundConnectAuth
  source: openapi/epidemic-sound-partner-content-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: epidemic-sound-scopes
source_filename: epidemic-sound-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/epidemic-sound-partner-content-api-openapi.yml\ndocs: https://developers.epidemicsound.com/docs/auth/\nnote: Epidemic Sound Connect uses OpenID Connect (authorization code + PKCE) but publishes no OAuth scopes reference — the auth docs (https://developers.epidemicsound.com/docs/auth/) show no scope parameter, and access is governed by the partnership agreement and the user's subscription tier rather than scopes (a token-response example shows only standard OIDC \"email profile\").\nschemes:\n- name: EpidemicSoundConnectAuth\n  source: openapi/epidemic-sound-partner-content-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/auth\n    tokenUrl: https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/token\n  description: |-\n    For users signing in with an Epidemic Sound account, user authentication\
  \ is\n    handled with OpenID Connect, which is a layer on top of OAuth 2.0.\n\n    > **Example Header:** `Authorization: Bearer es-connect-token`\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epidemic-sound/refs/heads/main/scopes/epidemic-sound-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Music
- Sound Effects
- Royalty-Free Music
- Audio
- Audio Licensing
- Soundtracking
- Sync Licensing
- Creators
- Video
- AI Voiceover
- Semantic Search
- MCP
token_urls:
- https://login.epidemicsound.com/auth/realms/accounts/protocol/openid-connect/token
---
