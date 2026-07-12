---
authorization_urls:
- https://pulsoid.net/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Pulsoid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pulsoid publishes 9 OAuth 2.0 scopes via the implicit and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pulsoid API on a user''s behalf.


  Tokens are issued from https://pulsoid.net/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pulsoid
provider_slug: pulsoid
schemes:
- flows:
  - authorizationUrl: https://pulsoid.net/oauth2/authorize
    flow: implicit
  - authorizationUrl: https://pulsoid.net/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://pulsoid.net/oauth2/token
  name: OAuth2
  source: openapi/pulsoid-openapi.yml
scope_count: 9
scope_names:
- data:heart_rate:read
- data:heart_rate:write
- data:room:read
- data:statistics:read
- geometry_dash_mod:configuration:read
- geometry_dash_mod:configuration:write
- profile:read
- widgets:read
- widgets:update
scopes:
- description: Read heart rate data
  flows:
  - authorizationCode
  - implicit
  scope: data:heart_rate:read
- description: Write heart rate data
  flows:
  - authorizationCode
  - implicit
  scope: data:heart_rate:write
- description: Read room real-time data
  flows:
  - implicit
  scope: data:room:read
- description: Read heart rate statistics
  flows:
  - authorizationCode
  - implicit
  scope: data:statistics:read
- description: Read GD mod config
  flows:
  - implicit
  scope: geometry_dash_mod:configuration:read
- description: Update GD mod config
  flows:
  - implicit
  scope: geometry_dash_mod:configuration:write
- description: Read profile
  flows:
  - authorizationCode
  - implicit
  scope: profile:read
- description: Read widgets
  flows:
  - authorizationCode
  - implicit
  scope: widgets:read
- description: Create or update widgets
  flows:
  - authorizationCode
  - implicit
  scope: widgets:update
slug: pulsoid-scopes
source_filename: pulsoid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pulsoid-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/pulsoid-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://pulsoid.net/oauth2/authorize\n  - flow: authorizationCode\n    authorizationUrl: https://pulsoid.net/oauth2/authorize\n    tokenUrl: https://pulsoid.net/oauth2/token\nscopes:\n- scope: data:heart_rate:read\n  description: Read heart rate data\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/pulsoid-openapi.yml\n- scope: data:heart_rate:write\n  description: Write heart rate data\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/pulsoid-openapi.yml\n- scope: data:room:read\n  description: Read room real-time data\n  flows:\n  - implicit\n  sources:\n  - openapi/pulsoid-openapi.yml\n- scope: data:statistics:read\n  description: Read heart rate statistics\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/pulsoid-openapi.yml\n\
  - scope: geometry_dash_mod:configuration:read\n  description: Read GD mod config\n  flows:\n  - implicit\n  sources:\n  - openapi/pulsoid-openapi.yml\n- scope: geometry_dash_mod:configuration:write\n  description: Update GD mod config\n  flows:\n  - implicit\n  sources:\n  - openapi/pulsoid-openapi.yml\n- scope: profile:read\n  description: Read profile\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/pulsoid-openapi.yml\n- scope: widgets:read\n  description: Read widgets\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/pulsoid-openapi.yml\n- scope: widgets:update\n  description: Create or update widgets\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/pulsoid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/scopes/pulsoid-scopes.yml
summary_line: 9 scopes · implicit/authorizationCode
tags:
- Heart Rate
- Health
- Wearables
- Real-Time
- Streaming
- WebSocket
- OAuth2
token_urls:
- https://pulsoid.net/oauth2/token
---
