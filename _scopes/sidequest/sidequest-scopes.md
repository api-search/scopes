---
api_specs:
- filename: sidequest-apps-api-openapi.yml
  format: yaml
  label: SideQuest Apps API
  slug: sidequest-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-apps-api-openapi.yml
- filename: sidequest-developers-api-openapi.yml
  format: yaml
  label: SideQuest Developers API
  slug: sidequest-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-developers-api-openapi.yml
- filename: sidequest-users-api-openapi.yml
  format: yaml
  label: SideQuest Users API
  slug: sidequest-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-users-api-openapi.yml
- filename: sidequest-usersapps-api-openapi.yml
  format: yaml
  label: SideQuest UsersApps API
  slug: sidequest-usersapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-usersapps-api-openapi.yml
- filename: sidequest-oauth2-api-openapi.yml
  format: yaml
  label: SideQuest O Auth2 API
  slug: sidequest-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-oauth2-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Sidequest Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SideQuest publishes 13 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the SideQuest API on a user''s behalf.


  Tokens are issued from https://api.sidequestvr.com/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SideQuest
provider_slug: sidequest
schemes: []
scope_count: 13
scope_names:
- user.basic_profile.read
- user.app_achievements.read
- user.app_achievements.write
- user.avatars.read
- user.avatars.write
- user.friends.read
- user.friends.write
- user.rich_presence.write
- user.communities.read
- user.communities.write
- user.messages.read
- user.messages.write
- user.messagehistory.read
scopes:
- description: Read a user's basic public profile (name, avatar preview, level, bio).
  flows: []
  scope: user.basic_profile.read
- description: Read the achievements a user has unlocked for an app.
  flows: []
  scope: user.app_achievements.read
- description: Grant or update a user's app achievements.
  flows: []
  scope: user.app_achievements.write
- description: Read a user's avatar(s).
  flows: []
  scope: user.avatars.read
- description: Create or update a user's avatar(s).
  flows: []
  scope: user.avatars.write
- description: Read a user's friends list.
  flows: []
  scope: user.friends.read
- description: Modify a user's friends (add/remove).
  flows: []
  scope: user.friends.write
- description: Publish rich-presence / activity status for a user.
  flows: []
  scope: user.rich_presence.write
- description: Read the communities a user belongs to.
  flows: []
  scope: user.communities.read
- description: Join, leave, or modify a user's communities.
  flows: []
  scope: user.communities.write
- description: Read a user's messages.
  flows: []
  scope: user.messages.read
- description: Send messages on behalf of a user.
  flows: []
  scope: user.messages.write
- description: Read a user's message history.
  flows: []
  scope: user.messagehistory.read
slug: sidequest-scopes
source_filename: sidequest-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: >-\n  Derived from openapi/sidequest-openapi.json — the scopes enum on\n  components.schemas.GetShortCodeRequest.scopes (the full set a client may\n  request) and the per-operation security requirements on the SideQuest Public\n  API (userAuth). No separate hosted scopes/permissions reference page was found\n  (sidequestvr.com is a single-page app; developer.sidequestvr.com does not\n  resolve), so descriptions are derived from the scope identifiers themselves.\napi: SideQuest Public API\ntoken_endpoint: https://api.sidequestvr.com/v2/oauth/token\nauthorization_flow: >-\n  Device-style short-code login: POST /v2/oauth/getshortcode (client_id + scopes)\n  returns a short code + verification_url the user approves; the client polls\n  POST /v2/oauth/checkshortcode to redeem it for an access_token + refresh_token.\n  Refresh via POST /v2/oauth/token (grant_type=refresh_token). Access tokens are\n  presented as HTTP bearer tokens\
  \ (userAuth).\nscopes:\n  - name: user.basic_profile.read\n    description: Read a user's basic public profile (name, avatar preview, level, bio).\n    used_by: [\"GET /v2/users/{route_users_id}\"]\n  - name: user.app_achievements.read\n    description: Read the achievements a user has unlocked for an app.\n    used_by: [\"GET /v2/users/{route_users_id}/apps/{apps_id}/achievements\"]\n  - name: user.app_achievements.write\n    description: Grant or update a user's app achievements.\n  - name: user.avatars.read\n    description: Read a user's avatar(s).\n  - name: user.avatars.write\n    description: Create or update a user's avatar(s).\n  - name: user.friends.read\n    description: Read a user's friends list.\n  - name: user.friends.write\n    description: Modify a user's friends (add/remove).\n  - name: user.rich_presence.write\n    description: Publish rich-presence / activity status for a user.\n  - name: user.communities.read\n    description: Read the communities a user belongs to.\n\
  \  - name: user.communities.write\n    description: Join, leave, or modify a user's communities.\n  - name: user.messages.read\n    description: Read a user's messages.\n  - name: user.messages.write\n    description: Send messages on behalf of a user.\n  - name: user.messagehistory.read\n    description: Read a user's message history.\nnotes: >-\n  Only user.basic_profile.read and user.app_achievements.read gate operations in\n  the currently published spec (0.2.0); the remaining scopes are requestable per\n  GetShortCodeRequest and correspond to product surfaces (avatars, friends,\n  communities, messaging, rich presence) not yet exposed as public REST paths.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/scopes/sidequest-scopes.yml
summary_line: 13 scopes
tags:
- Company
- Consumer
- Virtual Reality
- VR
- XR
- Gaming
- App Store
- Developers
token_bound: false
token_urls:
- https://api.sidequestvr.com/v2/oauth/token
---
