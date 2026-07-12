---
authorization_urls:
- https://api.vimeo.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Vimeo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vimeo publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vimeo API on a user''s behalf.


  Tokens are issued from https://api.vimeo.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vimeo
provider_slug: vimeo
schemes:
- flows:
  - authorizationUrl: https://api.vimeo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.vimeo.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.vimeo.com/oauth/authorize/client
  name: oauth2
  source: openapi/vimeo-openapi.yml
scope_count: 6
scope_names:
- create
- delete
- edit
- private
- public
- upload
scopes:
- description: Create albums, channels, etc.
  flows:
  - authorizationCode
  scope: create
- description: Delete videos, albums, channels
  flows:
  - authorizationCode
  scope: delete
- description: Edit videos, albums, channels
  flows:
  - authorizationCode
  scope: edit
- description: Access private data
  flows:
  - authorizationCode
  scope: private
- description: Access public data
  flows:
  - authorizationCode
  - clientCredentials
  scope: public
- description: Upload videos
  flows:
  - authorizationCode
  scope: upload
slug: vimeo-scopes
source_filename: vimeo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vimeo-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/vimeo-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.vimeo.com/oauth/authorize\n    tokenUrl: https://api.vimeo.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.vimeo.com/oauth/authorize/client\nscopes:\n- scope: create\n  description: Create albums, channels, etc.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vimeo-openapi.yml\n- scope: delete\n  description: Delete videos, albums, channels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vimeo-openapi.yml\n- scope: edit\n  description: Edit videos, albums, channels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vimeo-openapi.yml\n- scope: private\n  description: Access private data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vimeo-openapi.yml\n- scope: public\n  description: Access public data\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/vimeo-openapi.yml\n- scope: upload\n  description: Upload videos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vimeo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vimeo/refs/heads/main/scopes/vimeo-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Video
- Streaming
- Video Hosting
- Live Streaming
- Media
- OTT
token_urls:
- https://api.vimeo.com/oauth/access_token
- https://api.vimeo.com/oauth/authorize/client
---
