---
api_specs:
- filename: streamyard-openapi.yml
  format: yaml
  label: StreamYard API
  slug: streamyard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamyard/refs/heads/main/openapi/streamyard-openapi.yml
authorization_urls:
- https://streamyard.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Streamyard Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'StreamYard publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the StreamYard API on a user''s behalf.


  Tokens are issued from https://streamyard.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: StreamYard
provider_slug: streamyard
schemes:
- description: OAuth 2.0 Bearer token. Authenticate via StreamYard's OAuth flow at https://streamyard.com/oauth/authorize.
  flows:
  - authorizationUrl: https://streamyard.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://streamyard.com/oauth/token
  name: streamyardBearerAuth
  source: openapi/streamyard-openapi.yml
scope_count: 3
scope_names:
- broadcasts
- destinations
- recordings
scopes:
- description: Create and manage broadcasts
  flows:
  - authorizationCode
  scope: broadcasts
- description: View and manage streaming destinations
  flows:
  - authorizationCode
  scope: destinations
- description: Access and download recordings
  flows:
  - authorizationCode
  scope: recordings
slug: streamyard-scopes
source_filename: streamyard-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/streamyard-openapi.yml\nschemes:\n- name: streamyardBearerAuth\n  source: openapi/streamyard-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://streamyard.com/oauth/authorize\n    tokenUrl: https://streamyard.com/oauth/token\n  description: OAuth 2.0 Bearer token. Authenticate via StreamYard's OAuth flow at https://streamyard.com/oauth/authorize.\nscopes:\n- scope: broadcasts\n  description: Create and manage broadcasts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamyard-openapi.yml\n- scope: destinations\n  description: View and manage streaming destinations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamyard-openapi.yml\n- scope: recordings\n  description: Access and download recordings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/streamyard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamyard/refs/heads/main/scopes/streamyard-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Broadcasting
- Live Streaming
- Multi-Streaming
- Recordings
- Video
token_urls:
- https://streamyard.com/oauth/token
---
