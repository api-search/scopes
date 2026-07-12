---
authorization_urls:
- https://{instance}/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Pixelfed Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pixelfed publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pixelfed API on a user''s behalf.


  Tokens are issued from https://{instance}/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pixelfed
provider_slug: pixelfed
schemes:
- flows:
  - authorizationUrl: https://{instance}/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{instance}/oauth/token
  name: OAuth2
  source: openapi/openapi.yml
scope_count: 4
scope_names:
- follow
- push
- read
- write
scopes:
- description: Manage follows, blocks, and mutes
  flows:
  - authorizationCode
  scope: follow
- description: Manage Web Push subscriptions
  flows:
  - authorizationCode
  scope: push
- description: Read-only access to account data and timelines
  flows:
  - authorizationCode
  scope: read
- description: Write access to post statuses and manage account
  flows:
  - authorizationCode
  scope: write
slug: pixelfed-scopes
source_filename: pixelfed-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{instance}/oauth/authorize\n    tokenUrl: https://{instance}/oauth/token\nscopes:\n- scope: follow\n  description: Manage follows, blocks, and mutes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n- scope: push\n  description: Manage Web Push subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n- scope: read\n  description: Read-only access to account data and timelines\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n- scope: write\n  description: Write access to post statuses and manage account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/scopes/pixelfed-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Fediverse
- ActivityPub
- Photo Sharing
- Social Media
- Open Source
- Decentralized
- Mastodon Compatible
- Federation
token_urls:
- https://{instance}/oauth/token
---
