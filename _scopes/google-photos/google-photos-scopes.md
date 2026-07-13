---
api_specs:
- filename: photos.yml
  format: yaml
  label: Google Photos Library API v1
  slug: google-photos-library-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-photos/refs/heads/main/openapi/photos.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Photos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Photos Library publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Photos Library API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Photos Library
provider_slug: google-photos
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/photos.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/photoslibrary
- https://www.googleapis.com/auth/photoslibrary.readonly
- https://www.googleapis.com/auth/photoslibrary.sharing
scopes:
- description: View and manage your Google Photos library
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/photoslibrary
- description: View your Google Photos library
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/photoslibrary.readonly
- description: Manage and add to shared albums
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/photoslibrary.sharing
slug: google-photos-scopes
source_filename: google-photos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/photos.yml\nschemes:\n- name: oauth2\n  source: openapi/photos.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/photoslibrary\n  description: View and manage your Google Photos library\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/photos.yml\n- scope: https://www.googleapis.com/auth/photoslibrary.readonly\n  description: View your Google Photos library\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/photos.yml\n- scope: https://www.googleapis.com/auth/photoslibrary.sharing\n  description: Manage and add to shared albums\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/photos.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-photos/refs/heads/main/scopes/google-photos-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Albums
- Google
- Images
- Media
- Photos
- Sharing
- Storage
token_urls:
- https://oauth2.googleapis.com/token
---
