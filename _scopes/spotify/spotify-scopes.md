---
api_specs:
- filename: spotify-openapi-original.yml
  format: yaml
  label: Spotify Web API
  slug: spotify-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-openapi-original.yml
authorization_urls:
- https://accounts.spotify.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Spotify Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Spotify publishes 19 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spotify API on a user''s behalf.


  Tokens are issued from https://accounts.spotify.com/api/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spotify
provider_slug: spotify
schemes:
- description: Spotify supports OAuth 2.0 for authenticating all API requests.
  flows:
  - authorizationUrl: https://accounts.spotify.com/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.spotify.com/api/token
  name: oauth_2_0
  source: openapi/spotify-openapi-original.yml
scope_count: 19
scope_names:
- app-remote-control
- playlist-modify-private
- playlist-modify-public
- playlist-read-collaborative
- playlist-read-private
- streaming
- ugc-image-upload
- user-follow-modify
- user-follow-read
- user-library-modify
- user-library-read
- user-modify-playback-state
- user-read-currently-playing
- user-read-email
- user-read-playback-position
- user-read-playback-state
- user-read-private
- user-read-recently-played
- user-top-read
scopes:
- description: Communicate with the Spotify app on your device.
  flows:
  - authorizationCode
  scope: app-remote-control
- description: Manage your private playlists.
  flows:
  - authorizationCode
  scope: playlist-modify-private
- description: Manage your public playlists.
  flows:
  - authorizationCode
  scope: playlist-modify-public
- description: Access your collaborative playlists.
  flows:
  - authorizationCode
  scope: playlist-read-collaborative
- description: Access your private playlists.
  flows:
  - authorizationCode
  scope: playlist-read-private
- description: Play content and control playback on your other devices.
  flows:
  - authorizationCode
  scope: streaming
- description: Upload images to Spotify on your behalf.
  flows:
  - authorizationCode
  scope: ugc-image-upload
- description: Manage your saved content.
  flows:
  - authorizationCode
  scope: user-follow-modify
- description: Access your followers and who you are following.
  flows:
  - authorizationCode
  scope: user-follow-read
- description: Manage your saved content.
  flows:
  - authorizationCode
  scope: user-library-modify
- description: Access your saved content.
  flows:
  - authorizationCode
  scope: user-library-read
- description: Control playback on your Spotify clients and Spotify Connect devices.
  flows:
  - authorizationCode
  scope: user-modify-playback-state
- description: Read your currently playing content.
  flows:
  - authorizationCode
  scope: user-read-currently-playing
- description: Get your real email address.
  flows:
  - authorizationCode
  scope: user-read-email
- description: Read your position in content you have played.
  flows:
  - authorizationCode
  scope: user-read-playback-position
- description: Read your currently playing content and Spotify Connect devices information.
  flows:
  - authorizationCode
  scope: user-read-playback-state
- description: Access your subscription details.
  flows:
  - authorizationCode
  scope: user-read-private
- description: Access your recently played items.
  flows:
  - authorizationCode
  scope: user-read-recently-played
- description: Read your top artists and content.
  flows:
  - authorizationCode
  scope: user-top-read
slug: spotify-scopes
source_filename: spotify-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spotify-openapi-original.yml\nschemes:\n- name: oauth_2_0\n  source: openapi/spotify-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.spotify.com/authorize\n    tokenUrl: https://accounts.spotify.com/api/token\n  description: Spotify supports OAuth 2.0 for authenticating all API requests.\nscopes:\n- scope: app-remote-control\n  description: Communicate with the Spotify app on your device.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: playlist-modify-private\n  description: Manage your private playlists.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: playlist-modify-public\n  description: Manage your public playlists.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: playlist-read-collaborative\n  description: Access your\
  \ collaborative playlists.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: playlist-read-private\n  description: Access your private playlists.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: streaming\n  description: Play content and control playback on your other devices.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: ugc-image-upload\n  description: Upload images to Spotify on your behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-follow-modify\n  description: Manage your saved content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-follow-read\n  description: Access your followers and who you are following.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-library-modify\n\
  \  description: Manage your saved content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-library-read\n  description: Access your saved content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-modify-playback-state\n  description: Control playback on your Spotify clients and Spotify Connect devices.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-read-currently-playing\n  description: Read your currently playing content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-read-email\n  description: Get your real email address.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-read-playback-position\n  description: Read your position in content you have played.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n\
  - scope: user-read-playback-state\n  description: Read your currently playing content and Spotify Connect devices information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-read-private\n  description: Access your subscription details.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-read-recently-played\n  description: Access your recently played items.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n- scope: user-top-read\n  description: Read your top artists and content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spotify-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/scopes/spotify-scopes.yml
summary_line: 19 scopes · authorizationCode
tags:
- Music
- Audio
- Streaming
- Podcasts
- Playlists
token_urls:
- https://accounts.spotify.com/api/token
---
