---
authorization_urls:
- https://api.firework.com/oauth/authorize
description: ''
docs: https://docs.firework.com/firework-for-developers/api/authentication
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Firework Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Firework publishes 12 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Firework API on a user''s behalf.


  Tokens are issued from https://api.firework.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Firework
provider_slug: firework
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.firework.com/oauth/token
  - authorizationUrl: https://api.firework.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.firework.com/oauth/token
  name: OAuth2
  source: well-known/firework-oauth-authorization-server.json
scope_count: 12
scope_names:
- businesses:read
- channels:read
- channels:write
- insights:read
- livestreams:read
- livestreams:write
- playlists:read
- playlists:write
- products:read
- products:write
- videos:read
- videos:write
scopes:
- description: List businesses the token can act on.
  flows:
  - clientCredentials
  - authorizationCode
  scope: businesses:read
- description: List channels.
  flows:
  - clientCredentials
  - authorizationCode
  scope: channels:read
- description: Update a channel's metadata.
  flows:
  - clientCredentials
  - authorizationCode
  scope: channels:write
- description: Read analytics / insights data.
  flows:
  - clientCredentials
  - authorizationCode
  scope: insights:read
- description: Read livestream resources.
  flows:
  - clientCredentials
  - authorizationCode
  scope: livestreams:read
- description: Create and manage livestream resources.
  flows:
  - clientCredentials
  - authorizationCode
  scope: livestreams:write
- description: Read playlists.
  flows:
  - clientCredentials
  - authorizationCode
  scope: playlists:read
- description: Create and manage playlists.
  flows:
  - clientCredentials
  - authorizationCode
  scope: playlists:write
- description: List or search products and business stores.
  flows:
  - clientCredentials
  - authorizationCode
  scope: products:read
- description: Create and manage products.
  flows:
  - clientCredentials
  - authorizationCode
  scope: products:write
- description: List videos, read video details, and check async import status.
  flows:
  - clientCredentials
  - authorizationCode
  scope: videos:read
- description: Upload, create, update, delete, publish, archive videos and manage subtitles/posters.
  flows:
  - clientCredentials
  - authorizationCode
  scope: videos:write
slug: firework-scopes
source_filename: firework-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: well-known/firework-oauth-authorization-server.json\ndocs: https://docs.firework.com/firework-for-developers/api/authentication\nschemes:\n  - name: OAuth2\n    source: well-known/firework-oauth-authorization-server.json\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.firework.com/oauth/token\n      - flow: authorizationCode\n        authorizationUrl: https://api.firework.com/oauth/authorize\n        tokenUrl: https://api.firework.com/oauth/token\nscopes:\n  - scope: businesses:read\n    description: List businesses the token can act on.\n    flows: [clientCredentials, authorizationCode]\n  - scope: channels:read\n    description: List channels.\n    flows: [clientCredentials, authorizationCode]\n  - scope: channels:write\n    description: Update a channel's metadata.\n    flows: [clientCredentials, authorizationCode]\n  - scope: insights:read\n    description: Read analytics / insights data.\n \
  \   flows: [clientCredentials, authorizationCode]\n  - scope: livestreams:read\n    description: Read livestream resources.\n    flows: [clientCredentials, authorizationCode]\n  - scope: livestreams:write\n    description: Create and manage livestream resources.\n    flows: [clientCredentials, authorizationCode]\n  - scope: playlists:read\n    description: Read playlists.\n    flows: [clientCredentials, authorizationCode]\n  - scope: playlists:write\n    description: Create and manage playlists.\n    flows: [clientCredentials, authorizationCode]\n  - scope: products:read\n    description: List or search products and business stores.\n    flows: [clientCredentials, authorizationCode]\n  - scope: products:write\n    description: Create and manage products.\n    flows: [clientCredentials, authorizationCode]\n  - scope: videos:read\n    description: List videos, read video details, and check async import status.\n    flows: [clientCredentials, authorizationCode]\n  - scope: videos:write\n\
  \    description: Upload, create, update, delete, publish, archive videos and manage subtitles/posters.\n    flows: [clientCredentials, authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firework/refs/heads/main/scopes/firework-scopes.yml
summary_line: 12 scopes · clientCredentials/authorizationCode
tags:
- Company
- Consumer
- Video Commerce
- Shoppable Video
- Livestream Shopping
- Ecommerce
- Retail
- Video
- SDK
- Webhooks
token_urls:
- https://api.firework.com/oauth/token
---
