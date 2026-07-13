---
api_specs:
- filename: cms-api-swagger.yaml
  format: yaml
  label: Brightcove CMS API
  slug: brightcove-cms-api
  spec_type: OpenAPI
  url: https://apis.support.brightcove.com/cms/references/cms-api-swagger.yaml
- filename: ssai-openapi.yaml
  format: yaml
  label: Brightcove SSAI API
  slug: brightcove-ssai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/openapi/ssai-openapi.yaml
- filename: delivery-rules-openapi.yaml
  format: yaml
  label: Brightcove Delivery Rules API
  slug: brightcove-delivery-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/openapi/delivery-rules-openapi.yaml
- filename: social-openapi.yaml
  format: yaml
  label: Brightcove Social API
  slug: brightcove-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/openapi/social-openapi.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Brightcove Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Brightcove publishes 33 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brightcove API on a user''s behalf.


  Tokens are issued from https://oauth.brightcove.com/v4/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brightcove
provider_slug: brightcove
schemes:
- description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  source: openapi/analytics-api-openapi.yaml
- description: Brightcove OAuth API. See the [support documentation](https://apis.support.brightcove.com/oauth/) or [Getting Access Tokens](https://apis.support.brightcove.com/oauth/guides/getting-access-tokens.html) to learn more
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  source: openapi/audience-openapi.yaml
- description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  source: openapi/cms-api-openapi.yaml
- description: Brightcove OAuth API. To learn more, see the [OAuth Overview](https://apis.support.brightcove.com/oauth/) or the [Getting Access Tokens](https://apis.support.brightcove.com/oauth/code-samples/oauth-api-sample-get-access-token.html) document.
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  source: openapi/delivery-rules-openapi.yaml
- description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  source: openapi/dynamic-ingest-openapi.yaml
- description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  source: openapi/ingest-profiles-openapi.yaml
- description: '**IMPORTANT:** Basic Authentication is no longer supported. You must use OAuth 2.0 for all authentication.


    Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  source: openapi/player-management-openapi.yaml
- description: Brightcove OAuth API. See the [support documentation](https://apis.support.brightcove.com/oauth/) or [Getting Access Tokens](https://apis.support.brightcove.com/oauth/guides/getting-access-tokens.html) to learn more
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  source: openapi/social-openapi.yaml
- description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting Access Tokens](/oauth/guides/getting-access-tokens.html) to learn more
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  source: openapi/ssai-openapi.yaml
scope_count: 33
scope_names:
- video-cloud/analytics/read
- video-cloud/asset/delete
- video-cloud/audience/read
- video-cloud/audience/write
- video-cloud/delivery-rules/all
- video-cloud/delivery-rules/read
- video-cloud/ingest-profiles/account/read
- video-cloud/ingest-profiles/account/write
- video-cloud/ingest-profiles/profile/read
- video-cloud/ingest-profiles/profile/write
- video-cloud/notifications/all
- video-cloud/player/all
- video-cloud/player/read
- video-cloud/playlist/all
- video-cloud/playlist/create
- video-cloud/playlist/delete
- video-cloud/playlist/read
- video-cloud/playlist/update
- video-cloud/sharing-relationships/all
- video-cloud/sharing-relationships/create
- video-cloud/sharing-relationships/delete
- video-cloud/sharing-relationships/read
- video-cloud/sharing-relationships/update
- video-cloud/social/status/read
- video-cloud/ssai/all
- video-cloud/ssai/read
- video-cloud/upload-urls/read
- video-cloud/video/all
- video-cloud/video/clear-sources
- video-cloud/video/create
- video-cloud/video/delete
- video-cloud/video/read
- video-cloud/video/update
scopes:
- description: Read analytics data
  flows:
  - clientCredentials
  scope: video-cloud/analytics/read
- description: Digital Master Delete
  flows:
  - clientCredentials
  scope: video-cloud/asset/delete
- description: Read Leads and Events data
  flows:
  - clientCredentials
  scope: video-cloud/audience/read
- description: Write Leads and Events data
  flows:
  - clientCredentials
  scope: video-cloud/audience/write
- description: Read, Write, Delete Delivery Rules
  flows:
  - clientCredentials
  scope: video-cloud/delivery-rules/all
- description: Read Delivery Rules
  flows:
  - clientCredentials
  scope: video-cloud/delivery-rules/read
- description: Read account default ingest profile
  flows:
  - clientCredentials
  scope: video-cloud/ingest-profiles/account/read
- description: Write account settings
  flows:
  - clientCredentials
  scope: video-cloud/ingest-profiles/account/write
- description: Read ingest profiles
  flows:
  - clientCredentials
  scope: video-cloud/ingest-profiles/profile/read
- description: Write profiles
  flows:
  - clientCredentials
  scope: video-cloud/ingest-profiles/profile/write
- description: Notifications All
  flows:
  - clientCredentials
  scope: video-cloud/notifications/all
- description: Read/write player data
  flows:
  - clientCredentials
  scope: video-cloud/player/all
- description: Read player data
  flows:
  - clientCredentials
  scope: video-cloud/player/read
- description: Playlist All
  flows:
  - clientCredentials
  scope: video-cloud/playlist/all
- description: Playlist Create
  flows:
  - clientCredentials
  scope: video-cloud/playlist/create
- description: Playlist Delete
  flows:
  - clientCredentials
  scope: video-cloud/playlist/delete
- description: Playlist Read
  flows:
  - clientCredentials
  scope: video-cloud/playlist/read
- description: Playlist Update
  flows:
  - clientCredentials
  scope: video-cloud/playlist/update
- description: Sharing Relationships All
  flows:
  - clientCredentials
  scope: video-cloud/sharing-relationships/all
- description: Sharing Relationships Create
  flows:
  - clientCredentials
  scope: video-cloud/sharing-relationships/create
- description: Sharing Relationships Delete
  flows:
  - clientCredentials
  scope: video-cloud/sharing-relationships/delete
- description: Sharing Relationships Read
  flows:
  - clientCredentials
  scope: video-cloud/sharing-relationships/read
- description: Sharing Relationships Update
  flows:
  - clientCredentials
  scope: video-cloud/sharing-relationships/update
- description: Read social sharing status and history
  flows:
  - clientCredentials
  scope: video-cloud/social/status/read
- description: Read and write SSAI metadata
  flows:
  - clientCredentials
  scope: video-cloud/ssai/all
- description: Read SSAI metadata
  flows:
  - clientCredentials
  scope: video-cloud/ssai/read
- description: Read upload URLs
  flows:
  - clientCredentials
  scope: video-cloud/upload-urls/read
- description: Video ALL
  flows:
  - clientCredentials
  scope: video-cloud/video/all
- description: Read clear sources
  flows:
  - clientCredentials
  scope: video-cloud/video/clear-sources
- description: Video Create
  flows:
  - clientCredentials
  scope: video-cloud/video/create
- description: Video Delete
  flows:
  - clientCredentials
  scope: video-cloud/video/delete
- description: Read video data
  flows:
  - clientCredentials
  scope: video-cloud/video/read
- description: Video Update
  flows:
  - clientCredentials
  scope: video-cloud/video/update
slug: brightcove-scopes
source_filename: brightcove-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/analytics-api-openapi.yaml, openapi/audience-openapi.yaml, openapi/cms-api-openapi.yaml,\n  openapi/delivery-rules-openapi.yaml, openapi/dynamic-ingest-openapi.yaml, openapi/ingest-profiles-openapi.yaml,\n  openapi/player-management-openapi.yaml, openapi/social-openapi.yaml, openapi/ssai-openapi.yaml\nschemes:\n- name: BC_OAuth2\n  source: openapi/analytics-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n  description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting\n    Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more\n- name: BC_OAuth2\n  source: openapi/audience-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n  description: Brightcove OAuth API. See the [support documentation](https://apis.support.brightcove.com/oauth/)\n\
  \    or [Getting Access Tokens](https://apis.support.brightcove.com/oauth/guides/getting-access-tokens.html)\n    to learn more\n- name: BC_OAuth2\n  source: openapi/cms-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n  description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting\n    Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more\n- name: BC_OAuth2\n  source: openapi/delivery-rules-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n  description: Brightcove OAuth API. To learn more, see the [OAuth Overview](https://apis.support.brightcove.com/oauth/)\n    or the [Getting Access Tokens](https://apis.support.brightcove.com/oauth/code-samples/oauth-api-sample-get-access-token.html)\n    document.\n- name: BC_OAuth2\n  source: openapi/dynamic-ingest-openapi.yaml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n  description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting\n    Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more\n- name: BC_OAuth2\n  source: openapi/ingest-profiles-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n  description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting\n    Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more\n- name: BC_OAuth2\n  source: openapi/player-management-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n  description: |-\n    **IMPORTANT:** Basic Authentication is no longer supported. You must use OAuth 2.0 for all authentication.\n\n    Brightcove OAuth API. See the [support documentation](/oauth/index.html)\
  \ or [Getting Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more.\n- name: BC_OAuth2\n  source: openapi/social-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n  description: Brightcove OAuth API. See the [support documentation](https://apis.support.brightcove.com/oauth/)\n    or [Getting Access Tokens](https://apis.support.brightcove.com/oauth/guides/getting-access-tokens.html)\n    to learn more\n- name: BC_OAuth2\n  source: openapi/ssai-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n  description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting\n    Access Tokens](/oauth/guides/getting-access-tokens.html) to learn more\nscopes:\n- scope: video-cloud/analytics/read\n  description: Read analytics data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/analytics-api-openapi.yaml\n\
  - scope: video-cloud/asset/delete\n  description: Digital Master Delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/audience/read\n  description: Read Leads and Events data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/audience-openapi.yaml\n- scope: video-cloud/audience/write\n  description: Write Leads and Events data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/audience-openapi.yaml\n- scope: video-cloud/delivery-rules/all\n  description: Read, Write, Delete Delivery Rules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/delivery-rules-openapi.yaml\n- scope: video-cloud/delivery-rules/read\n  description: Read Delivery Rules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/delivery-rules-openapi.yaml\n- scope: video-cloud/ingest-profiles/account/read\n  description: Read account default ingest profile\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dynamic-ingest-openapi.yaml\n\
  \  - openapi/ingest-profiles-openapi.yaml\n- scope: video-cloud/ingest-profiles/account/write\n  description: Write account settings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ingest-profiles-openapi.yaml\n- scope: video-cloud/ingest-profiles/profile/read\n  description: Read ingest profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dynamic-ingest-openapi.yaml\n  - openapi/ingest-profiles-openapi.yaml\n- scope: video-cloud/ingest-profiles/profile/write\n  description: Write profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ingest-profiles-openapi.yaml\n- scope: video-cloud/notifications/all\n  description: Notifications All\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/player/all\n  description: Read/write player data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/player-management-openapi.yaml\n- scope: video-cloud/player/read\n  description: Read player data\n  flows:\n \
  \ - clientCredentials\n  sources:\n  - openapi/player-management-openapi.yaml\n- scope: video-cloud/playlist/all\n  description: Playlist All\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/playlist/create\n  description: Playlist Create\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/playlist/delete\n  description: Playlist Delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/playlist/read\n  description: Playlist Read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/playlist/update\n  description: Playlist Update\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/sharing-relationships/all\n  description: Sharing Relationships All\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/sharing-relationships/create\n\
  \  description: Sharing Relationships Create\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/sharing-relationships/delete\n  description: Sharing Relationships Delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/sharing-relationships/read\n  description: Sharing Relationships Read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/sharing-relationships/update\n  description: Sharing Relationships Update\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/social/status/read\n  description: Read social sharing status and history\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/social-openapi.yaml\n- scope: video-cloud/ssai/all\n  description: Read and write SSAI metadata\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ssai-openapi.yaml\n- scope: video-cloud/ssai/read\n\
  \  description: Read SSAI metadata\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ssai-openapi.yaml\n- scope: video-cloud/upload-urls/read\n  description: Read upload URLs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dynamic-ingest-openapi.yaml\n- scope: video-cloud/video/all\n  description: Video ALL\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n  - openapi/dynamic-ingest-openapi.yaml\n- scope: video-cloud/video/clear-sources\n  description: Read clear sources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/video/create\n  description: Video Create\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/video/delete\n  description: Video Delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/video/read\n  description: Read video data\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/analytics-api-openapi.yaml\n  - openapi/cms-api-openapi.yaml\n- scope: video-cloud/video/update\n  description: Video Update\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cms-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/scopes/brightcove-scopes.yml
summary_line: 33 scopes · clientCredentials
tags:
- Video
- Media
- Streaming
- Live Streaming
- Analytics
- CDN
- OTT
- Player
- Ad Insertion
token_urls:
- https://oauth.brightcove.com/v4/access_token
---
