---
api_specs:
- filename: restream-openapi.yml
  format: yaml
  label: Restream API
  slug: restream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/openapi/restream-openapi.yml
authorization_urls:
- https://api.restream.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Restream Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Restream publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Restream API on a user''s behalf.


  Tokens are issued from https://api.restream.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Restream
provider_slug: restream
schemes:
- flows:
  - authorizationUrl: https://api.restream.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.restream.io/oauth/token
  name: OAuth2
  source: openapi/restream-openapi.yml
scope_count: 7
scope_names:
- channels.read
- channels.write
- chat.read
- events.read
- events.write
- profile.read
- stream.read
scopes:
- description: Read channel information
  flows:
  - authorizationCode
  scope: channels.read
- description: Update channel settings
  flows:
  - authorizationCode
  scope: channels.write
- description: Read chat messages
  flows:
  - authorizationCode
  scope: chat.read
- description: Read event information
  flows:
  - authorizationCode
  scope: events.read
- description: Create and update events
  flows:
  - authorizationCode
  scope: events.write
- description: Read user profile information
  flows:
  - authorizationCode
  scope: profile.read
- description: Read stream key information
  flows:
  - authorizationCode
  scope: stream.read
slug: restream-scopes
source_filename: restream-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/restream-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/restream-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.restream.io/oauth/authorize\n    tokenUrl: https://api.restream.io/oauth/token\nscopes:\n- scope: channels.read\n  description: Read channel information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/restream-openapi.yml\n- scope: channels.write\n  description: Update channel settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/restream-openapi.yml\n- scope: chat.read\n  description: Read chat messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/restream-openapi.yml\n- scope: events.read\n  description: Read event information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/restream-openapi.yml\n- scope: events.write\n  description: Create and update events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/restream-openapi.yml\n\
  - scope: profile.read\n  description: Read user profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/restream-openapi.yml\n- scope: stream.read\n  description: Read stream key information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/restream-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/scopes/restream-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Broadcast
- Chat
- Content Delivery
- Live Streaming
- Multistreaming
- Video Streaming
token_urls:
- https://api.restream.io/oauth/token
---
