---
api_specs:
- filename: unsplash-openapi.yml
  format: yaml
  label: Unsplash API
  slug: unsplash
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unsplash/refs/heads/main/openapi/unsplash-openapi.yml
authorization_urls:
- https://unsplash.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Unsplash Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Unsplash publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unsplash API on a user''s behalf.


  Tokens are issued from https://unsplash.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unsplash
provider_slug: unsplash
schemes:
- flows:
  - authorizationUrl: https://unsplash.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://unsplash.com/oauth/token
  name: OAuth2
  source: openapi/unsplash-openapi.yml
scope_count: 8
scope_names:
- public
- read_collections
- read_photos
- read_user
- write_collections
- write_likes
- write_photos
- write_user
scopes:
- description: Read public data (default)
  flows:
  - authorizationCode
  scope: public
- description: Read collection data
  flows:
  - authorizationCode
  scope: read_collections
- description: Read photo data
  flows:
  - authorizationCode
  scope: read_photos
- description: Read user profile data
  flows:
  - authorizationCode
  scope: read_user
- description: Create, update, delete collections
  flows:
  - authorizationCode
  scope: write_collections
- description: Like/unlike photos
  flows:
  - authorizationCode
  scope: write_likes
- description: Write photo data (update metadata)
  flows:
  - authorizationCode
  scope: write_photos
- description: Write user profile data
  flows:
  - authorizationCode
  scope: write_user
slug: unsplash-scopes
source_filename: unsplash-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unsplash-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/unsplash-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://unsplash.com/oauth/authorize\n    tokenUrl: https://unsplash.com/oauth/token\nscopes:\n- scope: public\n  description: Read public data (default)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unsplash-openapi.yml\n- scope: read_collections\n  description: Read collection data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unsplash-openapi.yml\n- scope: read_photos\n  description: Read photo data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unsplash-openapi.yml\n- scope: read_user\n  description: Read user profile data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unsplash-openapi.yml\n- scope: write_collections\n  description: Create, update, delete collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unsplash-openapi.yml\n\
  - scope: write_likes\n  description: Like/unlike photos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unsplash-openapi.yml\n- scope: write_photos\n  description: Write photo data (update metadata)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unsplash-openapi.yml\n- scope: write_user\n  description: Write user profile data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unsplash-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unsplash/refs/heads/main/scopes/unsplash-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Photos
- Images
- Photography
- Stock Photos
- Creative
- Open Source
- Media
token_urls:
- https://unsplash.com/oauth/token
---
