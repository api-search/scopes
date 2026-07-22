---
api_specs:
- filename: volteras-connect-openapi-original.json
  format: json
  label: Volteras Connect API
  slug: volteras-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volteras/refs/heads/main/openapi/volteras-connect-openapi-original.json
authorization_urls: []
description: Volteras consent scopes control what data/capabilities an integration gets from a connected end-user account; they are passed via the scopes parameter when constructing the account connect URL (POST /v1/accounts:connect). The API-client credential itself uses OAuth 2.0 client-credentials with no client-level scopes. The docs scopes page documents the five vehicle scopes; the OpenAPI ScopeEnum additionally declares battery and geofence scopes.
docs: https://docs.volteras.com/overview/scopes
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Volteras Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Volteras publishes 12 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Volteras API on a user''s behalf.


  Tokens are issued from /v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Volteras
provider_slug: volteras
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: OAuth2ClientCredentialsBearer
  source: openapi/volteras-connect-openapi-original.json
scope_count: 12
scope_names:
- vehicle:all
- vehicle:information
- vehicle:charging_history
- vehicle:telemetry
- vehicle:commands
- vehicle:driving_behavior
- vehicle:location_history
- battery:all
- battery:telemetry
- geofences:all
- geofences:read
- geofences:write
scopes:
- description: Access to everything (all vehicle scopes).
  flows: []
  scope: vehicle:all
- description: Access to vehicle specifications, options, vin and registration plate.
  flows: []
  scope: vehicle:information
- description: Access to vehicle charging history.
  flows: []
  scope: vehicle:charging_history
- description: Access to location and odometer.
  flows: []
  scope: vehicle:telemetry
- description: Access to remote commands.
  flows: []
  scope: vehicle:commands
- description: ''
  flows: []
  scope: vehicle:driving_behavior
- description: ''
  flows: []
  scope: vehicle:location_history
- description: ''
  flows: []
  scope: battery:all
- description: ''
  flows: []
  scope: battery:telemetry
- description: ''
  flows: []
  scope: geofences:all
- description: ''
  flows: []
  scope: geofences:read
- description: ''
  flows: []
  scope: geofences:write
slug: volteras-scopes
source_filename: volteras-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/volteras-connect-openapi-original.json\ndocs: https://docs.volteras.com/overview/scopes\ndescription: >-\n  Volteras consent scopes control what data/capabilities an integration gets\n  from a connected end-user account; they are passed via the scopes parameter\n  when constructing the account connect URL (POST /v1/accounts:connect). The\n  API-client credential itself uses OAuth 2.0 client-credentials with no\n  client-level scopes. The docs scopes page documents the five vehicle scopes;\n  the OpenAPI ScopeEnum additionally declares battery and geofence scopes.\nschemes:\n  - name: OAuth2ClientCredentialsBearer\n    source: openapi/volteras-connect-openapi-original.json\n    flows:\n      - flow: clientCredentials\n        tokenUrl: /v1/oauth2/token\nscopes:\n  - scope: vehicle:all\n    description: Access to everything (all vehicle scopes).\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum,\
  \ docs]\n  - scope: vehicle:information\n    description: Access to vehicle specifications, options, vin and registration plate.\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum, docs]\n  - scope: vehicle:charging_history\n    description: Access to vehicle charging history.\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum, docs]\n  - scope: vehicle:telemetry\n    description: Access to location and odometer.\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum, docs]\n  - scope: vehicle:commands\n    description: Access to remote commands.\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum, docs]\n  - scope: vehicle:driving_behavior\n    description: null\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum]\n  - scope: vehicle:location_history\n    description: null\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum]\n  - scope: battery:all\n    description: null\n\
  \    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum]\n  - scope: battery:telemetry\n    description: null\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum]\n  - scope: geofences:all\n    description: null\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum]\n  - scope: geofences:read\n    description: null\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum]\n  - scope: geofences:write\n    description: null\n    sources: [openapi/volteras-connect-openapi-original.json#ScopeEnum]\nscoped_endpoints:\n  - {endpoint: '/vehicles/[id]', scopes: [vehicle:information], required: false, effect_without_scope: 'Fields excluded: vin, registrationPlate'}\n  - {endpoint: '/vehicles/', scopes: [vehicle:information], required: false, effect_without_scope: 'Fields excluded: vin, registrationPlate'}\n  - {endpoint: '/vehicles/[id]/options', scopes: [vehicle:information], required: true, effect_without_scope: 401 Response}\n\
  \  - {endpoint: '/vehicles/[id]/specifications', scopes: [vehicle:information], required: true, effect_without_scope: 401 Response}\n  - {endpoint: '/vehicles/[id]/telemetry', scopes: [vehicle:telemetry], required: true, effect_without_scope: 401 Response}\n  - {endpoint: '/vehicles/[id]/charging-history', scopes: [vehicle:charging_history], required: true, effect_without_scope: 401 Response}\n  - {endpoint: '/vehicles/[id]/charging-history/[id]', scopes: [vehicle:charging_history], required: true, effect_without_scope: 401 Response}\n  - {endpoint: '/vehicles/[id]/command-executions/', scopes: [vehicle:commands], required: true, effect_without_scope: 401 Response}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volteras/refs/heads/main/scopes/volteras-scopes.yml
summary_line: 12 scopes · clientCredentials
tags:
- Company
- Electric Vehicles
- Connected Vehicles
- Automotive
- Vehicle Telemetry
- EV Charging
- Energy
- Mobility
- Fleet Management
token_urls:
- /v1/oauth2/token
---
