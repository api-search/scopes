---
authorization_urls:
- https://api.g86racing.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: G86 Racing Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'G86 Racing publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the G86 Racing API on a user''s behalf.


  Tokens are issued from https://api.g86racing.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: G86 Racing
provider_slug: g86racing-com
schemes:
- flows:
  - authorizationUrl: https://api.g86racing.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.g86racing.com/oauth/token
  name: oauth
  source: openapi/g86racing-com-openapi.json
scope_count: 6
scope_names:
- billing
- live
- profile
- read
- teams
- write
scopes:
- description: Verify existing native store purchases
  flows:
  - authorizationCode
  scope: billing
- description: Publish/control authorized Pit Wall streams
  flows:
  - authorizationCode
  scope: live
- description: Edit public account profile
  flows:
  - authorizationCode
  scope: profile
- description: Read synchronized account records
  flows:
  - authorizationCode
  scope: read
- description: Manage authorized team workspace and membership
  flows:
  - authorizationCode
  scope: teams
- description: Create/change/delete cloud records
  flows:
  - authorizationCode
  scope: write
slug: g86racing-com-scopes
source_filename: g86racing-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/g86racing-com-openapi.json\nschemes:\n- name: oauth\n  source: openapi/g86racing-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.g86racing.com/oauth/authorize\n    tokenUrl: https://api.g86racing.com/oauth/token\nscopes:\n- scope: billing\n  description: Verify existing native store purchases\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/g86racing-com-openapi.json\n- scope: live\n  description: Publish/control authorized Pit Wall streams\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/g86racing-com-openapi.json\n- scope: profile\n  description: Edit public account profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/g86racing-com-openapi.json\n- scope: read\n  description: Read synchronized account records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/g86racing-com-openapi.json\n- scope: teams\n  description: Manage authorized team\
  \ workspace and membership\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/g86racing-com-openapi.json\n- scope: write\n  description: Create/change/delete cloud records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/g86racing-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/g86racing-com/scopes/g86racing-com-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Motorsports
- Telemetry
- Lap Timing
- Mobile App
- Data Export
token_bound: false
token_urls:
- https://api.g86racing.com/oauth/token
---
