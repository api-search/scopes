---
api_specs:
- filename: zoom-chat--openapi-original.yml
  format: yaml
  label: Zoom Chat API
  slug: zoom-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-chat--openapi-original.yml
- filename: zoom-group--openapi-original.yml
  format: yaml
  label: Zoom Group API
  slug: zoom-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-group--openapi-original.yml
- filename: zoom-device--openapi-original.yml
  format: yaml
  label: Zoom Device API
  slug: zoom-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-device--openapi-original.yml
- filename: zoom-im--openapi-original.yml
  format: yaml
  label: Zoom Instant Message API
  slug: zoom-instant-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-im--openapi-original.yml
- filename: zoom-account--openapi-original.yml
  format: yaml
  label: Zoom Account API
  slug: zoom-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-account--openapi-original.yml
- filename: zoom-recording--openapi-original.yml
  format: yaml
  label: Zoom Recording API
  slug: zoom-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-recording--openapi-original.yml
- filename: zoom-meeting--openapi-original.yml
  format: yaml
  label: Zoom Meeting API
  slug: zoom-meeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-meeting--openapi-original.yml
- filename: zoom-metrics--openapi-original.yml
  format: yaml
  label: Zoom Metrics API
  slug: zoom-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-metrics--openapi-original.yml
- filename: zoom-report--openapi-original.yml
  format: yaml
  label: Zoom Report API
  slug: zoom-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-report--openapi-original.yml
- filename: zoom-user--openapi-original.yml
  format: yaml
  label: Zoom User API
  slug: zoom-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-user--openapi-original.yml
- filename: zoom-webinar--openapi-original.yml
  format: yaml
  label: Zoom Webinar API
  slug: zoom-webinar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/openapi/zoom-webinar--openapi-original.yml
authorization_urls:
- https://zoom.us/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zoom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoom publishes 19 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoom API on a user''s behalf.


  Tokens are issued from https://zoom.us/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoom
provider_slug: zoom
schemes:
- description: Zoom uses OAuth 2.0 for authentication. Server-to-Server OAuth and standard OAuth apps are supported.
  flows:
  - authorizationUrl: https://zoom.us/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://zoom.us/oauth/token
  name: oauth2
  source: openapi/zoom-meeting-api-openapi.yml
scope_count: 19
scope_names:
- cloud_recording:read:list_recording_files:admin
- meeting:delete:meeting
- meeting:delete:poll:admin
- meeting:read:invitation:admin
- meeting:read:list_meetings:admin
- meeting:read:list_past_participants:admin
- meeting:read:list_registrants:admin
- meeting:read:meeting
- meeting:read:meeting:admin
- meeting:read:meeting:master
- meeting:read:participant:admin
- meeting:read:poll:admin
- meeting:update:livestream:admin
- meeting:update:registrant:admin
- meeting:write:meeting
- meeting:write:meeting:admin
- meeting:write:meeting:master
- meeting:write:poll:admin
- meeting:write:registrant:admin
scopes:
- description: Read recording files (admin)
  flows:
  - authorizationCode
  scope: cloud_recording:read:list_recording_files:admin
- description: Delete meetings
  flows:
  - authorizationCode
  scope: meeting:delete:meeting
- description: Delete meeting polls (admin)
  flows:
  - authorizationCode
  scope: meeting:delete:poll:admin
- description: Read meeting invitation (admin)
  flows:
  - authorizationCode
  scope: meeting:read:invitation:admin
- description: List meetings (admin)
  flows:
  - authorizationCode
  scope: meeting:read:list_meetings:admin
- description: List past meeting participants (admin)
  flows:
  - authorizationCode
  scope: meeting:read:list_past_participants:admin
- description: List registrants (admin)
  flows:
  - authorizationCode
  scope: meeting:read:list_registrants:admin
- description: Read meeting details
  flows:
  - authorizationCode
  scope: meeting:read:meeting
- description: Read meeting details (admin)
  flows:
  - authorizationCode
  scope: meeting:read:meeting:admin
- description: Read meeting details (master)
  flows:
  - authorizationCode
  scope: meeting:read:meeting:master
- description: Read meeting participants (admin)
  flows:
  - authorizationCode
  scope: meeting:read:participant:admin
- description: Read meeting polls (admin)
  flows:
  - authorizationCode
  scope: meeting:read:poll:admin
- description: Update live stream (admin)
  flows:
  - authorizationCode
  scope: meeting:update:livestream:admin
- description: Update registrant status (admin)
  flows:
  - authorizationCode
  scope: meeting:update:registrant:admin
- description: Create and update meetings
  flows:
  - authorizationCode
  scope: meeting:write:meeting
- description: Write meeting details (admin)
  flows:
  - authorizationCode
  scope: meeting:write:meeting:admin
- description: Write meeting details (master)
  flows:
  - authorizationCode
  scope: meeting:write:meeting:master
- description: Write meeting polls (admin)
  flows:
  - authorizationCode
  scope: meeting:write:poll:admin
- description: Add registrants (admin)
  flows:
  - authorizationCode
  scope: meeting:write:registrant:admin
slug: zoom-scopes
source_filename: zoom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zoom-meeting-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/zoom-meeting-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://zoom.us/oauth/authorize\n    tokenUrl: https://zoom.us/oauth/token\n  description: Zoom uses OAuth 2.0 for authentication. Server-to-Server OAuth and standard OAuth\n    apps are supported.\nscopes:\n- scope: cloud_recording:read:list_recording_files:admin\n  description: Read recording files (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:delete:meeting\n  description: Delete meetings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:delete:poll:admin\n  description: Delete meeting polls (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:read:invitation:admin\n  description:\
  \ Read meeting invitation (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:read:list_meetings:admin\n  description: List meetings (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:read:list_past_participants:admin\n  description: List past meeting participants (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:read:list_registrants:admin\n  description: List registrants (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:read:meeting\n  description: Read meeting details\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:read:meeting:admin\n  description: Read meeting details (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:read:meeting:master\n\
  \  description: Read meeting details (master)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:read:participant:admin\n  description: Read meeting participants (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:read:poll:admin\n  description: Read meeting polls (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:update:livestream:admin\n  description: Update live stream (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:update:registrant:admin\n  description: Update registrant status (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:write:meeting\n  description: Create and update meetings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:write:meeting:admin\n\
  \  description: Write meeting details (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:write:meeting:master\n  description: Write meeting details (master)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:write:poll:admin\n  description: Write meeting polls (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n- scope: meeting:write:registrant:admin\n  description: Add registrants (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-meeting-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/scopes/zoom-scopes.yml
summary_line: 19 scopes · authorizationCode
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
token_urls:
- https://zoom.us/oauth/token
---
