---
api_specs:
- filename: medialab-ai-imgur-api.postman_collection.json
  format: json
  label: Imgur API
  slug: imgur-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/medialab-ai/refs/heads/main/postman/medialab-ai-imgur-api.postman_collection.json
authorization_urls:
- https://api.genius.com/oauth/authorize
description: ''
docs: https://docs.genius.com/#available-scopes
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Medialab Ai Scopes
name_suffix: OAuth Scopes
note: Captured verbatim from the Genius API "Available Scopes" table. Only the Genius API has an OAuth scope surface across the MediaLab.AI portfolio - Imgur's OAuth 2.0 implementation documents no scope parameter, so an authorized Imgur token carries full account access for the granting user and no scopes/ entries exist for it.
overview: 'MediaLab.AI publishes 4 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the MediaLab.AI API on a user''s behalf.


  Tokens are issued from https://api.genius.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MediaLab.AI
provider_slug: medialab-ai
schemes:
- api: Genius API
  flows:
  - authorizationUrl: https://api.genius.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.genius.com/oauth/token
  - authorizationUrl: https://api.genius.com/oauth/authorize
    flow: implicit
  name: GeniusOAuth2
  scope_delimiter: space
  source: https://docs.genius.com/#authentication
scope_count: 4
scope_names:
- me
- create_annotation
- manage_annotation
- vote
scopes:
- description: Read account information for the currently authenticated user.
  flows:
  - authorizationCode
  - implicit
  scope: me
- description: Create a new annotation on a public web page.
  flows:
  - authorizationCode
  - implicit
  scope: create_annotation
- description: Update or delete an annotation created by the authenticated user.
  flows:
  - authorizationCode
  - implicit
  scope: manage_annotation
- description: Upvote, downvote or remove the authenticated user's vote on an annotation.
  flows:
  - authorizationCode
  - implicit
  scope: vote
slug: medialab-ai-scopes
source_filename: medialab-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://docs.genius.com/#available-scopes\ndocs: https://docs.genius.com/#available-scopes\nnote: >-\n  Captured verbatim from the Genius API \"Available Scopes\" table. Only the Genius API\n  has an OAuth scope surface across the MediaLab.AI portfolio - Imgur's OAuth 2.0\n  implementation documents no scope parameter, so an authorized Imgur token carries\n  full account access for the granting user and no scopes/ entries exist for it.\nschemes:\n- name: GeniusOAuth2\n  api: Genius API\n  source: https://docs.genius.com/#authentication\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.genius.com/oauth/authorize\n    tokenUrl: https://api.genius.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://api.genius.com/oauth/authorize\n  scope_delimiter: space\nscopes:\n- scope: me\n  description: Read account information for the currently authenticated user.\n  endpoints:\n  - GET /account\n \
  \ flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - https://docs.genius.com/#available-scopes\n- scope: create_annotation\n  description: Create a new annotation on a public web page.\n  endpoints:\n  - POST /annotations\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - https://docs.genius.com/#available-scopes\n- scope: manage_annotation\n  description: Update or delete an annotation created by the authenticated user.\n  endpoints:\n  - PUT /annotations/:id\n  - DELETE /annotations/:id\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - https://docs.genius.com/#available-scopes\n- scope: vote\n  description: Upvote, downvote or remove the authenticated user's vote on an annotation.\n  endpoints:\n  - PUT /annotations/:id/upvote\n  - PUT /annotations/:id/downvote\n  - PUT /annotations/:id/unvote\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - https://docs.genius.com/#available-scopes\nunscoped_access:\n  api: Genius API\n  credential:\
  \ client access token\n  description: >-\n    Apps without user-specific behaviour can use the client access token generated on\n    the API Client management page. It is valid only for read-only endpoints that are\n    not restricted by a required scope - GET /annotations/:id, GET /referents,\n    GET /songs/:id, GET /artists/:id, GET /artists/:id/songs, GET /web_pages/lookup\n    and GET /search.\n  source: https://docs.genius.com/#access-for-apps-without-users\napis_without_scopes:\n- api: Imgur API\n  reason: >-\n    Imgur's documented OAuth 2.0 authorization request accepts only client_id,\n    response_type and state - there is no scope parameter. Account access is\n    all-or-nothing per authorized user.\n  source: https://apidocs.imgur.com/#authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medialab-ai/refs/heads/main/scopes/medialab-ai-scopes.yml
summary_line: 4 scopes · authorizationCode/implicit
tags:
- Company
- Media
- Social
- Advertising
- Content
- Image
- Music
- Messaging
- Communities
- Holding Company
token_urls:
- https://api.genius.com/oauth/token
---
