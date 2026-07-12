---
authorization_urls:
- https://slack.com/oauth/v2/authorize
- https://slack.com/openid/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Slack Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Slack publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Slack API on a user''s behalf.


  Tokens are issued from https://slack.com/api/oauth.v2.access.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Slack
provider_slug: slack
schemes:
- flows:
  - authorizationUrl: https://slack.com/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://slack.com/api/oauth.v2.access
  name: slackAuth
  source: openapi/slack-assistant-openapi.yml
- flows:
  - authorizationUrl: https://slack.com/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://slack.com/api/oauth.v2.access
  name: slackAuth
  source: openapi/slack-bookmarks-openapi.yml
- flows:
  - authorizationUrl: https://slack.com/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://slack.com/api/oauth.v2.access
  name: slackAuth
  source: openapi/slack-canvases-openapi.yml
- flows:
  - authorizationUrl: https://slack.com/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://slack.com/api/oauth.v2.access
  name: slackAuth
  source: openapi/slack-emoji-openapi.yml
- flows:
  - authorizationUrl: https://slack.com/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://slack.com/api/oauth.v2.access
  name: slackAuth
  source: openapi/slack-functions-openapi.yml
- flows:
  - authorizationUrl: https://slack.com/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://slack.com/api/oauth.v2.access
  name: slackAuth
  source: openapi/slack-lists-openapi.yml
- flows:
  - authorizationUrl: https://slack.com/openid/connect/authorize
    flow: authorizationCode
    tokenUrl: https://slack.com/api/openid.connect.token
  name: slackAuth
  source: openapi/slack-openid-connect-openapi.yml
scope_count: 13
scope_names:
- assistant:write
- bookmarks:read
- bookmarks:write
- canvases:read
- canvases:write
- email
- emoji:read
- functions:read
- functions:write
- lists:read
- lists:write
- openid
- profile
scopes:
- description: Write access to assistant threads
  flows:
  - authorizationCode
  scope: assistant:write
- description: Read bookmarks
  flows:
  - authorizationCode
  scope: bookmarks:read
- description: Write bookmarks
  flows:
  - authorizationCode
  scope: bookmarks:write
- description: Read canvases
  flows:
  - authorizationCode
  scope: canvases:read
- description: Write canvases
  flows:
  - authorizationCode
  scope: canvases:write
- description: Access user email address
  flows:
  - authorizationCode
  scope: email
- description: Access emoji data
  flows:
  - authorizationCode
  scope: emoji:read
- description: Read function data
  flows:
  - authorizationCode
  scope: functions:read
- description: Write function data
  flows:
  - authorizationCode
  scope: functions:write
- description: Read lists data
  flows:
  - authorizationCode
  scope: lists:read
- description: Write lists data
  flows:
  - authorizationCode
  scope: lists:write
- description: Authenticate using Sign in with Slack
  flows:
  - authorizationCode
  scope: openid
- description: Access user profile information
  flows:
  - authorizationCode
  scope: profile
slug: slack-scopes
source_filename: slack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/slack-assistant-openapi.yml, openapi/slack-bookmarks-openapi.yml, openapi/slack-canvases-openapi.yml,\n  openapi/slack-emoji-openapi.yml, openapi/slack-functions-openapi.yml, openapi/slack-lists-openapi.yml,\n  openapi/slack-openid-connect-openapi.yml\nschemes:\n- name: slackAuth\n  source: openapi/slack-assistant-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://slack.com/oauth/v2/authorize\n    tokenUrl: https://slack.com/api/oauth.v2.access\n- name: slackAuth\n  source: openapi/slack-bookmarks-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://slack.com/oauth/v2/authorize\n    tokenUrl: https://slack.com/api/oauth.v2.access\n- name: slackAuth\n  source: openapi/slack-canvases-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://slack.com/oauth/v2/authorize\n    tokenUrl: https://slack.com/api/oauth.v2.access\n- name: slackAuth\n\
  \  source: openapi/slack-emoji-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://slack.com/oauth/v2/authorize\n    tokenUrl: https://slack.com/api/oauth.v2.access\n- name: slackAuth\n  source: openapi/slack-functions-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://slack.com/oauth/v2/authorize\n    tokenUrl: https://slack.com/api/oauth.v2.access\n- name: slackAuth\n  source: openapi/slack-lists-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://slack.com/oauth/v2/authorize\n    tokenUrl: https://slack.com/api/oauth.v2.access\n- name: slackAuth\n  source: openapi/slack-openid-connect-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://slack.com/openid/connect/authorize\n    tokenUrl: https://slack.com/api/openid.connect.token\nscopes:\n- scope: assistant:write\n  description: Write access to assistant threads\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-assistant-openapi.yml\n\
  - scope: bookmarks:read\n  description: Read bookmarks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-bookmarks-openapi.yml\n- scope: bookmarks:write\n  description: Write bookmarks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-bookmarks-openapi.yml\n- scope: canvases:read\n  description: Read canvases\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-canvases-openapi.yml\n- scope: canvases:write\n  description: Write canvases\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-canvases-openapi.yml\n- scope: email\n  description: Access user email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-openid-connect-openapi.yml\n- scope: emoji:read\n  description: Access emoji data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-emoji-openapi.yml\n- scope: functions:read\n  description: Read function data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-functions-openapi.yml\n-\
  \ scope: functions:write\n  description: Write function data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-functions-openapi.yml\n- scope: lists:read\n  description: Read lists data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-lists-openapi.yml\n- scope: lists:write\n  description: Write lists data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-lists-openapi.yml\n- scope: openid\n  description: Authenticate using Sign in with Slack\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-openid-connect-openapi.yml\n- scope: profile\n  description: Access user profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/slack-openid-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slack/refs/heads/main/scopes/slack-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Bots
- Chat
- Collaboration
- Messaging
- Productivity
- T1
- Team Communication
token_urls:
- https://slack.com/api/oauth.v2.access
- https://slack.com/api/openid.connect.token
---
