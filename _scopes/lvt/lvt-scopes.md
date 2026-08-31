---
api_specs:
- filename: lvt-cameras-api-openapi.yml
  format: yaml
  label: LVT Cameras API
  slug: lvt-cameras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-cameras-api-openapi.yml
- filename: lvt-events-api-openapi.yml
  format: yaml
  label: LVT Events API
  slug: lvt-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-events-api-openapi.yml
- filename: lvt-liveunits-api-openapi.yml
  format: yaml
  label: LVT Live Units API
  slug: lvt-liveunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-liveunits-api-openapi.yml
- filename: lvt-locations-api-openapi.yml
  format: yaml
  label: LVT Locations API
  slug: lvt-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-locations-api-openapi.yml
- filename: lvt-media-api-openapi.yml
  format: yaml
  label: LVT Media API
  slug: lvt-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-media-api-openapi.yml
- filename: lvt-publickeys-api-openapi.yml
  format: yaml
  label: LVT Public Keys API
  slug: lvt-publickeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-publickeys-api-openapi.yml
- filename: lvt-streams-api-openapi.yml
  format: yaml
  label: LVT Streams API
  slug: lvt-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-streams-api-openapi.yml
- filename: lvt-talkdown-api-openapi.yml
  format: yaml
  label: LVT Talkdown API
  slug: lvt-talkdown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-talkdown-api-openapi.yml
- filename: lvt-webhooks-api-openapi.yml
  format: yaml
  label: LVT Webhooks API
  slug: lvt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Lvt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LVT publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LVT API on a user''s behalf.


  Tokens are issued from https://api.lvt.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LVT
provider_slug: lvt
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.lvt.com/oauth2/v1/token
  name: OAuth2
  source: openapi/lvt-partner-api-openapi.yml
scope_count: 3
scope_names:
- account.cameras.manage
- account.liveUnits.manage
- account.locations.manage
scopes:
- description: Edit a cameras data
  flows:
  - clientCredentials
  scope: account.cameras.manage
- description: Edit a live units data
  flows:
  - clientCredentials
  scope: account.liveUnits.manage
- description: Edit a locations data
  flows:
  - clientCredentials
  scope: account.locations.manage
slug: lvt-scopes
source_filename: lvt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: openapi/lvt-partner-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/lvt-partner-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.lvt.com/oauth2/v1/token\nscopes:\n- scope: account.cameras.manage\n  description: Edit a cameras data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lvt-partner-api-openapi.yml\n- scope: account.liveUnits.manage\n  description: Edit a live units data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lvt-partner-api-openapi.yml\n- scope: account.locations.manage\n  description: Edit a locations data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lvt-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/scopes/lvt-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Company
- Physical Security
- Video Surveillance
- Cameras
- Video Streaming
- WebRTC
- RTSP
- ONVIF
- IoT
- Alerts
- Webhooks
- Public Safety
- Retail
- Critical Infrastructure
token_urls:
- https://api.lvt.com/oauth2/v1/token
---
