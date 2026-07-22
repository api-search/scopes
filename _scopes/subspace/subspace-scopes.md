---
api_specs:
- filename: subspace-openapi-original.yml
  format: yaml
  label: Subspace Product API
  slug: subspace-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subspace/refs/heads/main/openapi/subspace-openapi-original.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Subspace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Subspace publishes 9 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Subspace API on a user''s behalf.


  Tokens are issued from https://id.subspace.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Subspace
provider_slug: subspace
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://id.subspace.com/oauth/token
  name: accessCode
  source: openapi/subspace-openapi-original.yml
scope_count: 9
scope_names:
- accelerators:read
- accelerators:write
- console:access
- projects:read
- rtpspeed:read
- rtpspeed:write
- sipteleport:read
- sipteleport:write
- webrtccdn:access
scopes:
- description: allows reading details about provisioned PacketAccelerators
  flows:
  - clientCredentials
  scope: accelerators:read
- description: allows administration of PacketAccelerators
  flows:
  - clientCredentials
  scope: accelerators:write
- description: allows access to the console
  flows:
  - clientCredentials
  scope: console:access
- description: allows reading details about projects
  flows:
  - clientCredentials
  scope: projects:read
- description: allows reading details about rtpspeed
  flows:
  - clientCredentials
  scope: rtpspeed:read
- description: allows administration of rtpspeed
  flows:
  - clientCredentials
  scope: rtpspeed:write
- description: allows reading details about provisioned SIPTeleport
  flows:
  - clientCredentials
  scope: sipteleport:read
- description: allows administration of SIPTeleport
  flows:
  - clientCredentials
  scope: sipteleport:write
- description: allows administration of WebRTC-CDN
  flows:
  - clientCredentials
  scope: webrtccdn:access
slug: subspace-scopes
source_filename: subspace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/subspace-openapi-original.yml\nschemes:\n- name: accessCode\n  source: openapi/subspace-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.subspace.com/oauth/token\nscopes:\n- scope: accelerators:read\n  description: allows reading details about provisioned PacketAccelerators\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/subspace-openapi-original.yml\n- scope: accelerators:write\n  description: allows administration of PacketAccelerators\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/subspace-openapi-original.yml\n- scope: console:access\n  description: allows access to the console\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/subspace-openapi-original.yml\n- scope: projects:read\n  description: allows reading details about projects\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/subspace-openapi-original.yml\n- scope: rtpspeed:read\n  description:\
  \ allows reading details about rtpspeed\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/subspace-openapi-original.yml\n- scope: rtpspeed:write\n  description: allows administration of rtpspeed\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/subspace-openapi-original.yml\n- scope: sipteleport:read\n  description: allows reading details about provisioned SIPTeleport\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/subspace-openapi-original.yml\n- scope: sipteleport:write\n  description: allows administration of SIPTeleport\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/subspace-openapi-original.yml\n- scope: webrtccdn:access\n  description: allows administration of WebRTC-CDN\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/subspace-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subspace/refs/heads/main/scopes/subspace-scopes.yml
summary_line: 9 scopes · clientCredentials
tags:
- Company
- Networking
- Real-Time
- WebRTC
- VoIP
- SIP
- CDN
- Gaming
- Latency
- Infrastructure
token_urls:
- https://id.subspace.com/oauth/token
---
