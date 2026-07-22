---
authorization_urls: []
description: ''
docs: https://dev.streamlabs.com/docs/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Stream Labs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Stream Labs publishes 13 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Stream Labs API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stream Labs
provider_slug: stream-labs
schemes:
- authorizationUrl: https://streamlabs.com/api/v2.0/authorize
  flow: authorizationCode
  name: OAuth2
  tokenUrl: https://streamlabs.com/api/v2.0/token
  type: oauth2
scope_count: 13
scope_names:
- donations.create
- donations.read
- alerts.create
- alerts.write
- legacy.token
- socket.token
- points.read
- points.write
- credits.write
- profiles.write
- jar.write
- wheel.write
- mediashare.control
scopes:
- description: Create donations (POST /donations).
  flows: []
  scope: donations.create
- description: Read donations (GET /donations).
  flows: []
  scope: donations.read
- description: Trigger custom alerts (POST /alerts).
  flows: []
  scope: alerts.create
- description: 'Manage the alert queue: skip, mute/unmute volume, pause/unpause queue, and send test alerts.'
  flows: []
  scope: alerts.write
- description: Retrieve a legacy token (GET /legacy/token).
  flows: []
  scope: legacy.token
- description: Retrieve a Socket API token for the real-time event stream (GET /socket/token).
  flows: []
  scope: socket.token
- description: Read loyalty points (GET /points).
  flows: []
  scope: points.read
- description: Modify loyalty points (subtract, import, add to all users).
  flows: []
  scope: points.write
- description: Roll the stream credits (POST /credits/roll).
  flows: []
  scope: credits.write
- description: Retrieve and activate alert profiles.
  flows: []
  scope: profiles.write
- description: Empty the tip jar (POST /jar/empty).
  flows: []
  scope: jar.write
- description: Spin the wheel (POST /wheel/spin).
  flows: []
  scope: wheel.write
- description: 'Control media share: play, pause, volume, skip, and moderation settings.'
  flows: []
  scope: mediashare.control
slug: stream-labs-scopes
source_filename: stream-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://dev.streamlabs.com/docs/scopes\ndocs: https://dev.streamlabs.com/docs/scopes\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://streamlabs.com/api/v2.0/authorize\n  tokenUrl: https://streamlabs.com/api/v2.0/token\nscopes:\n- scope: donations.create\n  description: Create donations (POST /donations).\n- scope: donations.read\n  description: Read donations (GET /donations).\n- scope: alerts.create\n  description: Trigger custom alerts (POST /alerts).\n- scope: alerts.write\n  description: >-\n    Manage the alert queue: skip, mute/unmute volume, pause/unpause queue, and\n    send test alerts.\n- scope: legacy.token\n  description: Retrieve a legacy token (GET /legacy/token).\n- scope: socket.token\n  description: Retrieve a Socket API token for the real-time event stream (GET /socket/token).\n- scope: points.read\n  description: Read loyalty points (GET /points).\n- scope:\
  \ points.write\n  description: Modify loyalty points (subtract, import, add to all users).\n- scope: credits.write\n  description: Roll the stream credits (POST /credits/roll).\n- scope: profiles.write\n  description: Retrieve and activate alert profiles.\n- scope: jar.write\n  description: Empty the tip jar (POST /jar/empty).\n- scope: wheel.write\n  description: Spin the wheel (POST /wheel/spin).\n- scope: mediashare.control\n  description: >-\n    Control media share: play, pause, volume, skip, and moderation settings.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stream-labs/refs/heads/main/scopes/stream-labs-scopes.yml
summary_line: 13 scopes
tags:
- Company
- Live Streaming
- Creator Economy
- Alerts
- Donations
- Loyalty Points
- Media Share
- OAuth
- Real-time
- Streaming Tools
token_urls: []
---
