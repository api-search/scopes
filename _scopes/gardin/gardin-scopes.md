---
authorization_urls: []
description: ''
docs: https://developers.gardin.ag/docs/gardin-api/gardin-api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Gardin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gardin publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gardin API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gardin
provider_slug: gardin
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  tokenUrl: https://login.gardin.ag/oauth2/token
scope_count: 11
scope_names:
- data.chf:query
- data.indices:query
- devices:command
- devices:control
- devices.registry:read
- devices.registry:write
- jobs:read
- jobs:write
- jobs:execute
- notifications:subscribe
- notifications.alerts:subscribe
scopes:
- description: Query chlorophyll-fluorescence (ChF) data via the Query API.
  flows:
  - clientCredentials
  scope: data.chf:query
- description: Query Gardin indices data via the Query API.
  flows:
  - clientCredentials
  scope: data.indices:query
- description: Send commands to Gardin sensors.
  flows:
  - clientCredentials
  scope: devices:command
- description: Control sensor hardware settings.
  flows:
  - clientCredentials
  scope: devices:control
- description: Read the device/sensor registry.
  flows:
  - clientCredentials
  scope: devices.registry:read
- description: Manage (write) the device/sensor registry.
  flows:
  - clientCredentials
  scope: devices.registry:write
- description: Read growth / measurement job status.
  flows:
  - clientCredentials
  scope: jobs:read
- description: Create or update growth / measurement jobs.
  flows:
  - clientCredentials
  scope: jobs:write
- description: Execute (start/stop) growth / measurement jobs.
  flows:
  - clientCredentials
  scope: jobs:execute
- description: Subscribe to general notifications.
  flows:
  - clientCredentials
  scope: notifications:subscribe
- description: Subscribe to plant-health alert notifications.
  flows:
  - clientCredentials
  scope: notifications.alerts:subscribe
slug: gardin-scopes
source_filename: gardin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.gardin.ag/docs/gardin-api/gardin-api\ndocs: https://developers.gardin.ag/docs/gardin-api/gardin-api\nschemes:\n- name: OAuth2ClientCredentials\n  flow: clientCredentials\n  tokenUrl: https://login.gardin.ag/oauth2/token\nscopes:\n- scope: data.chf:query\n  description: Query chlorophyll-fluorescence (ChF) data via the Query API.\n  service: Query API\n  flows: [clientCredentials]\n- scope: data.indices:query\n  description: Query Gardin indices data via the Query API.\n  service: Query API\n  flows: [clientCredentials]\n- scope: devices:command\n  description: Send commands to Gardin sensors.\n  service: Sensor Management API\n  flows: [clientCredentials]\n- scope: devices:control\n  description: Control sensor hardware settings.\n  service: Sensor Management API\n  flows: [clientCredentials]\n- scope: devices.registry:read\n  description: Read the device/sensor registry.\n  service: Sensor Management API\n\
  \  flows: [clientCredentials]\n- scope: devices.registry:write\n  description: Manage (write) the device/sensor registry.\n  service: Sensor Management API\n  flows: [clientCredentials]\n- scope: jobs:read\n  description: Read growth / measurement job status.\n  service: Sensor Management API\n  flows: [clientCredentials]\n- scope: jobs:write\n  description: Create or update growth / measurement jobs.\n  service: Sensor Management API\n  flows: [clientCredentials]\n- scope: jobs:execute\n  description: Execute (start/stop) growth / measurement jobs.\n  service: Sensor Management API\n  flows: [clientCredentials]\n- scope: notifications:subscribe\n  description: Subscribe to general notifications.\n  service: Notification API\n  flows: [clientCredentials]\n- scope: notifications.alerts:subscribe\n  description: Subscribe to plant-health alert notifications.\n  service: Notification API\n  flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gardin/refs/heads/main/scopes/gardin-scopes.yml
summary_line: 11 scopes
tags:
- Company
- Agriculture
- Agritech
- Precision Agriculture
- Plant Health
- Photosynthesis
- IoT
- Sensors
- Greenhouse
- Crop Intelligence
- Sustainability
- Data
token_urls: []
---
