---
authorization_urls:
- https://connect.deezer.com/oauth/auth.php
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Deezer Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Deezer publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deezer API on a user''s behalf.


  Tokens are issued from https://connect.deezer.com/oauth/access_token.php.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deezer
provider_slug: deezer
schemes:
- flows:
  - authorizationUrl: https://connect.deezer.com/oauth/auth.php
    flow: authorizationCode
    tokenUrl: https://connect.deezer.com/oauth/access_token.php
  name: oauth2
  source: openapi/deezer-openapi.yml
scope_count: 7
scope_names:
- basic_access
- delete_library
- email
- listening_history
- manage_community
- manage_library
- offline_access
scopes:
- description: Basic profile info
  flows:
  - authorizationCode
  scope: basic_access
- description: Delete from user's library
  flows:
  - authorizationCode
  scope: delete_library
- description: Get user's email address
  flows:
  - authorizationCode
  scope: email
- description: Read listening history
  flows:
  - authorizationCode
  scope: listening_history
- description: Manage user's community
  flows:
  - authorizationCode
  scope: manage_community
- description: Manage user's library
  flows:
  - authorizationCode
  scope: manage_library
- description: Long-lived access
  flows:
  - authorizationCode
  scope: offline_access
slug: deezer-scopes
source_filename: deezer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deezer-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/deezer-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://connect.deezer.com/oauth/auth.php\n    tokenUrl: https://connect.deezer.com/oauth/access_token.php\nscopes:\n- scope: basic_access\n  description: Basic profile info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/deezer-openapi.yml\n- scope: delete_library\n  description: Delete from user's library\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/deezer-openapi.yml\n- scope: email\n  description: Get user's email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/deezer-openapi.yml\n- scope: listening_history\n  description: Read listening history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/deezer-openapi.yml\n- scope: manage_community\n  description: Manage user's community\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/deezer-openapi.yml\n- scope: manage_library\n  description: Manage user's library\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/deezer-openapi.yml\n- scope: offline_access\n  description: Long-lived access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/deezer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/scopes/deezer-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Music
- Streaming
- Audio
- OAuth
- Catalog
- Playlists
token_urls:
- https://connect.deezer.com/oauth/access_token.php
---
