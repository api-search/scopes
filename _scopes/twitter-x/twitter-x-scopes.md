---
api_specs:
- filename: twitter-x-x-api-v2-openapi.json
  format: json
  label: X API v2
  slug: x-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter-x/refs/heads/main/openapi/twitter-x-x-api-v2-openapi.json
authorization_urls:
- https://api.x.com/2/oauth2/authorize
description: ''
docs: https://docs.x.com/resources/fundamentals/authentication/oauth-2-0/authorization-code
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Twitter X Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Twitter/X publishes 21 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Twitter/X API on a user''s behalf.


  Tokens are issued from https://api.x.com/2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Twitter/X
provider_slug: twitter-x
schemes:
- flows:
  - authorizationUrl: https://api.x.com/2/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.x.com/2/oauth2/token
  name: OAuth2UserToken
  source: openapi/twitter-x-x-api-v2-openapi.json
scope_count: 21
scope_names:
- block.read
- bookmark.read
- bookmark.write
- dm.read
- dm.write
- follows.read
- follows.write
- like.read
- like.write
- list.read
- list.write
- media.write
- mute.read
- mute.write
- offline.access
- space.read
- timeline.read
- tweet.moderate.write
- tweet.read
- tweet.write
- users.read
scopes:
- description: View accounts you have blocked.
  flows:
  - authorizationCode
  scope: block.read
- description: Read your bookmarked Posts.
  flows:
  - authorizationCode
  scope: bookmark.read
- description: Create and delete your bookmarks.
  flows:
  - authorizationCode
  scope: bookmark.write
- description: Read all your Direct Messages.
  flows:
  - authorizationCode
  scope: dm.read
- description: Send and manage your Direct Messages.
  flows:
  - authorizationCode
  scope: dm.write
- description: View accounts you follow and accounts following you.
  flows:
  - authorizationCode
  scope: follows.read
- description: Follow and unfollow accounts on your behalf.
  flows:
  - authorizationCode
  scope: follows.write
- description: View Posts you have liked and likes you can see.
  flows:
  - authorizationCode
  scope: like.read
- description: Like and unlike Posts on your behalf.
  flows:
  - authorizationCode
  scope: like.write
- description: View Lists, members, and followers of Lists you created or are a member of, including private Lists.
  flows:
  - authorizationCode
  scope: list.read
- description: Create and manage Lists on your behalf.
  flows:
  - authorizationCode
  scope: list.write
- description: Upload media, such as photos and videos, on your behalf.
  flows:
  - authorizationCode
  scope: media.write
- description: View accounts you have muted.
  flows:
  - authorizationCode
  scope: mute.read
- description: Mute and unmute accounts on your behalf.
  flows:
  - authorizationCode
  scope: mute.write
- description: Request a refresh token for the app.
  flows:
  - authorizationCode
  scope: offline.access
- description: View all Spaces you have access to.
  flows:
  - authorizationCode
  scope: space.read
- description: View all Custom Timelines you can see, including public Custom Timelines from other developers.
  flows:
  - authorizationCode
  scope: timeline.read
- description: Hide and unhide replies to your Posts.
  flows:
  - authorizationCode
  scope: tweet.moderate.write
- description: View all Posts you can see, including those from protected accounts.
  flows:
  - authorizationCode
  scope: tweet.read
- description: Post and repost on your behalf.
  flows:
  - authorizationCode
  scope: tweet.write
- description: View any account you can see, including protected accounts.
  flows:
  - authorizationCode
  scope: users.read
slug: twitter-x-scopes
source_filename: twitter-x-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/twitter-x-x-api-v2-openapi.json\ndocs: https://docs.x.com/resources/fundamentals/authentication/oauth-2-0/authorization-code\nnotes: >-\n  The 21 scopes and their descriptions in the live OpenAPI\n  (api.x.com/2/openapi.json) match the OAuth 2.0 scopes table in the\n  authorization-code docs. OAuth 2.0 fine-grained scopes also apply to the\n  Account Activity API v2 (since 2026-01-15); when OAuth 1.0a credentials are\n  present their all-or-nothing permissions override OAuth 2.0 scopes.\nschemes:\n- name: OAuth2UserToken\n  source: openapi/twitter-x-x-api-v2-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.x.com/2/oauth2/authorize\n    tokenUrl: https://api.x.com/2/oauth2/token\nscopes:\n- scope: block.read\n  description: View accounts you have blocked.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: bookmark.read\n  description:\
  \ Read your bookmarked Posts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: bookmark.write\n  description: Create and delete your bookmarks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: dm.read\n  description: Read all your Direct Messages.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: dm.write\n  description: Send and manage your Direct Messages.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: follows.read\n  description: View accounts you follow and accounts following you.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: follows.write\n  description: Follow and unfollow accounts on your behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: like.read\n  description: View\
  \ Posts you have liked and likes you can see.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: like.write\n  description: Like and unlike Posts on your behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: list.read\n  description: View Lists, members, and followers of Lists you created or are a member of, including\n    private Lists.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: list.write\n  description: Create and manage Lists on your behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: media.write\n  description: Upload media, such as photos and videos, on your behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: mute.read\n  description: View accounts you have muted.\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/twitter-x-x-api-v2-openapi.json\n- scope: mute.write\n  description: Mute and unmute accounts on your behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: offline.access\n  description: Request a refresh token for the app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: space.read\n  description: View all Spaces you have access to.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: timeline.read\n  description: View all Custom Timelines you can see, including public Custom Timelines from\n    other developers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: tweet.moderate.write\n  description: Hide and unhide replies to your Posts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: tweet.read\n  description: View all Posts\
  \ you can see, including those from protected accounts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: tweet.write\n  description: Post and repost on your behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n- scope: users.read\n  description: View any account you can see, including protected accounts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/twitter-x-x-api-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twitter-x/refs/heads/main/scopes/twitter-x-scopes.yml
summary_line: 21 scopes · authorizationCode
tags:
- Company
- Social
- Social Media
- Posts
- Real-Time
- Streaming
- News
- Developer Platform
token_urls:
- https://api.x.com/2/oauth2/token
---
