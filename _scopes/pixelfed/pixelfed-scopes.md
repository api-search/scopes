---
api_specs:
- filename: pixelfed-accounts-api-openapi.yml
  format: yaml
  label: Pixelfed Accounts API
  slug: pixelfed-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-accounts-api-openapi.yml
- filename: pixelfed-blocks-and-mutes-api-openapi.yml
  format: yaml
  label: Pixelfed Blocks and Mutes API
  slug: pixelfed-blocks-and-mutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-blocks-and-mutes-api-openapi.yml
- filename: pixelfed-bookmarks-api-openapi.yml
  format: yaml
  label: Pixelfed Bookmarks API
  slug: pixelfed-bookmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-bookmarks-api-openapi.yml
- filename: pixelfed-collections-api-openapi.yml
  format: yaml
  label: Pixelfed Collections API
  slug: pixelfed-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-collections-api-openapi.yml
- filename: pixelfed-direct-messages-api-openapi.yml
  format: yaml
  label: Pixelfed Direct Messages API
  slug: pixelfed-direct-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-direct-messages-api-openapi.yml
- filename: pixelfed-discovery-api-openapi.yml
  format: yaml
  label: Pixelfed Discovery API
  slug: pixelfed-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-discovery-api-openapi.yml
- filename: pixelfed-favourites-api-openapi.yml
  format: yaml
  label: Pixelfed Favourites API
  slug: pixelfed-favourites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-favourites-api-openapi.yml
- filename: pixelfed-follow-requests-api-openapi.yml
  format: yaml
  label: Pixelfed Follow Requests API
  slug: pixelfed-follow-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-follow-requests-api-openapi.yml
- filename: pixelfed-instance-api-openapi.yml
  format: yaml
  label: Pixelfed Instance API
  slug: pixelfed-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-instance-api-openapi.yml
- filename: pixelfed-lists-api-openapi.yml
  format: yaml
  label: Pixelfed Lists API
  slug: pixelfed-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-lists-api-openapi.yml
- filename: pixelfed-media-api-openapi.yml
  format: yaml
  label: Pixelfed Media API
  slug: pixelfed-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-media-api-openapi.yml
- filename: pixelfed-notifications-api-openapi.yml
  format: yaml
  label: Pixelfed Notifications API
  slug: pixelfed-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-notifications-api-openapi.yml
- filename: pixelfed-push-notifications-api-openapi.yml
  format: yaml
  label: Pixelfed Push Notifications API
  slug: pixelfed-push-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-push-notifications-api-openapi.yml
- filename: pixelfed-search-api-openapi.yml
  format: yaml
  label: Pixelfed Search API
  slug: pixelfed-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-search-api-openapi.yml
- filename: pixelfed-statuses-api-openapi.yml
  format: yaml
  label: Pixelfed Statuses API
  slug: pixelfed-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-statuses-api-openapi.yml
- filename: pixelfed-stories-api-openapi.yml
  format: yaml
  label: Pixelfed Stories API
  slug: pixelfed-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-stories-api-openapi.yml
- filename: pixelfed-timelines-api-openapi.yml
  format: yaml
  label: Pixelfed Timelines API
  slug: pixelfed-timelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-timelines-api-openapi.yml
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
