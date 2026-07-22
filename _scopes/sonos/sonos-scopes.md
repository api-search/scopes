---
authorization_urls:
- https://api.sonos.com/login/v3/oauth
description: The Sonos Control API defines a single OAuth 2.0 scope. It is requested in the authorize step and grants control over all players and groups in the authenticated user's household(s).
docs: https://docs.sonos.com/docs/authorize
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sonos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sonos publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sonos API on a user''s behalf.


  Tokens are issued from https://api.sonos.com/login/v3/oauth/access.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sonos
provider_slug: sonos
schemes:
- flows:
  - authorizationUrl: https://api.sonos.com/login/v3/oauth
    flow: authorizationCode
    tokenUrl: https://api.sonos.com/login/v3/oauth/access
  name: SonosOAuth
  source: https://docs.sonos.com/docs/authorize
scope_count: 1
scope_names:
- playback-control-all
scopes:
- description: 'Full control access to the household''s Sonos system: read household/group state and drive playback, volume, grouping, favorites, playlists, home theater, audio clips, and cloud-queue sessions.'
  flows:
  - authorizationCode
  scope: playback-control-all
slug: sonos-scopes
source_filename: sonos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sonos.com/docs/authorize\ndocs: https://docs.sonos.com/docs/authorize\ndescription: >-\n  The Sonos Control API defines a single OAuth 2.0 scope. It is requested in the\n  authorize step and grants control over all players and groups in the\n  authenticated user's household(s).\nschemes:\n- name: SonosOAuth\n  source: https://docs.sonos.com/docs/authorize\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.sonos.com/login/v3/oauth\n    tokenUrl: https://api.sonos.com/login/v3/oauth/access\nscopes:\n- scope: playback-control-all\n  description: >-\n    Full control access to the household's Sonos system: read household/group\n    state and drive playback, volume, grouping, favorites, playlists, home\n    theater, audio clips, and cloud-queue sessions.\n  flows: [authorizationCode]\n  sources: [https://docs.sonos.com/docs/authorize]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonos/refs/heads/main/scopes/sonos-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Consumer
- Audio
- Music
- Smart Home
- IoT
- Streaming
- Speakers
- Home Automation
- Voice
token_urls:
- https://api.sonos.com/login/v3/oauth/access
---
