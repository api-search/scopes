---
authorization_urls: []
description: ''
docs: https://docs.butlr.io/getting-started/mint-client-credentials
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Butlr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Butlr publishes 12 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Butlr API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Butlr
provider_slug: butlr
schemes:
- audience: https://butlrauth/
  flow: clientCredentials
  name: OAuth2 Client Credentials
scope_count: 12
scope_names:
- read:spaces
- write:spaces
- delete:spaces
- read:rooms
- write:rooms
- delete:rooms
- read:sensors
- write:sensors
- delete:sensors
- read:hives
- write:hives
- delete:hives
scopes:
- description: Read access to spaces (sites/buildings/floors).
  flows: []
  scope: read:spaces
- description: Create and update spaces.
  flows: []
  scope: write:spaces
- description: Delete spaces.
  flows: []
  scope: delete:spaces
- description: Read access to rooms.
  flows: []
  scope: read:rooms
- description: Create and update rooms.
  flows: []
  scope: write:rooms
- description: Delete rooms.
  flows: []
  scope: delete:rooms
- description: Read access to sensors.
  flows: []
  scope: read:sensors
- description: Create and update sensors.
  flows: []
  scope: write:sensors
- description: Delete sensors.
  flows: []
  scope: delete:sensors
- description: Read access to hives (sensor gateways/hubs).
  flows: []
  scope: read:hives
- description: Create and update hives.
  flows: []
  scope: write:hives
- description: Delete hives.
  flows: []
  scope: delete:hives
slug: butlr-scopes
source_filename: butlr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.butlr.io/getting-started/mint-client-credentials\ndocs: https://docs.butlr.io/getting-started/mint-client-credentials\naudience: https://butlrauth/\nidentity_provider: Auth0\nschemes:\n- name: OAuth2 Client Credentials\n  flow: clientCredentials\n  audience: https://butlrauth/\nscopes:\n- {scope: 'read:spaces',   description: Read access to spaces (sites/buildings/floors).}\n- {scope: 'write:spaces',  description: Create and update spaces.}\n- {scope: 'delete:spaces', description: Delete spaces.}\n- {scope: 'read:rooms',    description: Read access to rooms.}\n- {scope: 'write:rooms',   description: Create and update rooms.}\n- {scope: 'delete:rooms',  description: Delete rooms.}\n- {scope: 'read:sensors',  description: Read access to sensors.}\n- {scope: 'write:sensors', description: Create and update sensors.}\n- {scope: 'delete:sensors',description: Delete sensors.}\n- {scope: 'read:hives',    description: Read\
  \ access to hives (sensor gateways/hubs).}\n- {scope: 'write:hives',   description: Create and update hives.}\n- {scope: 'delete:hives',  description: Delete hives.}\nnotes: >-\n  Scopes are granted to Auth0 M2M clients created for the Butlr API audience\n  (https://butlrauth/). The documented default scope set covers the spaces,\n  rooms, sensors, and hives resource families with read/write/delete access.\n  The official MCP server is provisioned with read-only scopes only. Derived\n  from the client-credential minting docs (no OpenAPI oauth2 flow declaration\n  is published, so the derive-oauth-scopes.py baseline was not applicable).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butlr/refs/heads/main/scopes/butlr-scopes.yml
summary_line: 12 scopes
tags:
- Company
- Sensors
- Occupancy
- People Sensing
- Smart Buildings
- Spatial Intelligence
- IoT
- GraphQL
- Webhooks
- Real Estate
token_urls: []
---
