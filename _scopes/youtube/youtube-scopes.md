---
api_specs:
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Activities API
  slug: youtube-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Channels API
  slug: youtube-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Comments API
  slug: youtube-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Comment Threads API
  slug: youtube-comment-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Playlists API
  slug: youtube-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Playlist Items API
  slug: youtube-playlist-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Search API
  slug: youtube-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Subscriptions API
  slug: youtube-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Videos API
  slug: youtube-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Captions API
  slug: youtube-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Video Categories API
  slug: youtube-video-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube I18n Languages API
  slug: youtube-i18n-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube I18n Regions API
  slug: youtube-i18n-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-analytics-openapi.yml
  format: yaml
  label: YouTube Analytics API
  slug: youtube-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-analytics-openapi.yml
- filename: youtube-reporting-openapi.yml
  format: yaml
  label: YouTube Reporting API
  slug: youtube-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-reporting-openapi.yml
- filename: youtube-live-streaming-openapi.yml
  format: yaml
  label: YouTube Live Streaming API
  slug: youtube-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-live-streaming-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Youtube Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Youtube publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Youtube API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Youtube
provider_slug: youtube
schemes:
- description: OAuth 2.0 authentication for YouTube Analytics API
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/youtube-analytics-openapi-original.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/youtube-analytics-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/youtube-data-api-openapi.yml
- description: OAuth 2.0 authentication for YouTube Data API
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/youtube-data-openapi-original.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/youtube-live-streaming-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/youtube-reporting-openapi.yml
scope_count: 7
scope_names:
- https://www.googleapis.com/auth/youtube
- https://www.googleapis.com/auth/youtube.force-ssl
- https://www.googleapis.com/auth/youtube.readonly
- https://www.googleapis.com/auth/youtube.upload
- https://www.googleapis.com/auth/youtubepartner
- https://www.googleapis.com/auth/yt-analytics-monetary.readonly
- https://www.googleapis.com/auth/yt-analytics.readonly
scopes:
- description: Manage your YouTube account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/youtube
- description: See, edit, and permanently delete your YouTube videos, ratings, comments and captions
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/youtube.force-ssl
- description: View your YouTube account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/youtube.readonly
- description: Manage your YouTube videos
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/youtube.upload
- description: View and manage your assets and associated content on YouTube
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/youtubepartner
- description: View YouTube Analytics monetary reports
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/yt-analytics-monetary.readonly
- description: View YouTube Analytics reports
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/yt-analytics.readonly
slug: youtube-scopes
source_filename: youtube-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/youtube-analytics-openapi-original.yml, openapi/youtube-analytics-openapi.yml,\n  openapi/youtube-data-api-openapi.yml, openapi/youtube-data-openapi-original.yml, openapi/youtube-live-streaming-openapi.yml,\n  openapi/youtube-reporting-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/youtube-analytics-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for YouTube Analytics API\n- name: oauth2\n  source: openapi/youtube-analytics-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/youtube-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n\
  \    tokenUrl: https://oauth2.googleapis.com/token\n- name: OAuth2\n  source: openapi/youtube-data-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for YouTube Data API\n- name: oauth2\n  source: openapi/youtube-live-streaming-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/youtube-reporting-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/youtube\n  description: Manage your YouTube account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/youtube-analytics-openapi-original.yml\n  - openapi/youtube-analytics-openapi.yml\n\
  \  - openapi/youtube-data-api-openapi.yml\n  - openapi/youtube-data-openapi-original.yml\n  - openapi/youtube-live-streaming-openapi.yml\n- scope: https://www.googleapis.com/auth/youtube.force-ssl\n  description: See, edit, and permanently delete your YouTube videos, ratings, comments and\n    captions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/youtube-data-api-openapi.yml\n  - openapi/youtube-data-openapi-original.yml\n  - openapi/youtube-live-streaming-openapi.yml\n- scope: https://www.googleapis.com/auth/youtube.readonly\n  description: View your YouTube account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/youtube-analytics-openapi-original.yml\n  - openapi/youtube-analytics-openapi.yml\n  - openapi/youtube-data-api-openapi.yml\n  - openapi/youtube-data-openapi-original.yml\n  - openapi/youtube-live-streaming-openapi.yml\n- scope: https://www.googleapis.com/auth/youtube.upload\n  description: Manage your YouTube videos\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/youtube-data-api-openapi.yml\n  - openapi/youtube-data-openapi-original.yml\n- scope: https://www.googleapis.com/auth/youtubepartner\n  description: View and manage your assets and associated content on YouTube\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/youtube-data-api-openapi.yml\n- scope: https://www.googleapis.com/auth/yt-analytics-monetary.readonly\n  description: View YouTube Analytics monetary reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/youtube-analytics-openapi-original.yml\n  - openapi/youtube-analytics-openapi.yml\n  - openapi/youtube-reporting-openapi.yml\n- scope: https://www.googleapis.com/auth/yt-analytics.readonly\n  description: View YouTube Analytics reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/youtube-analytics-openapi-original.yml\n  - openapi/youtube-analytics-openapi.yml\n  - openapi/youtube-reporting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/scopes/youtube-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
token_urls:
- https://oauth2.googleapis.com/token
---
