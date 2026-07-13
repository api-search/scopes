---
api_specs:
- filename: youtube.yml
  format: yaml
  label: YouTube Data API v3
  slug: youtube-data-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/openapi/youtube.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Youtube Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'YouTube Data publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the YouTube Data API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: YouTube Data
provider_slug: google-youtube
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/youtube.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/youtube
- https://www.googleapis.com/auth/youtube.readonly
- https://www.googleapis.com/auth/youtube.upload
scopes:
- description: Manage your YouTube account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/youtube
- description: View your YouTube account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/youtube.readonly
- description: Upload YouTube videos
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/youtube.upload
slug: google-youtube-scopes
source_filename: google-youtube-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/youtube.yml\nschemes:\n- name: oauth2\n  source: openapi/youtube.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/youtube\n  description: Manage your YouTube account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/youtube.yml\n- scope: https://www.googleapis.com/auth/youtube.readonly\n  description: View your YouTube account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/youtube.yml\n- scope: https://www.googleapis.com/auth/youtube.upload\n  description: Upload YouTube videos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/youtube.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/scopes/google-youtube-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Channels
- Google
- Media
- Playlists
- Search
- Streaming
- Video
- YouTube
token_urls:
- https://oauth2.googleapis.com/token
---
