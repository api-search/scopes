---
api_specs:
- filename: ev-energy-api-v2-openapi.yaml
  format: yaml
  label: ev.energy v2 API
  slug: ev-energy-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ev-energy/refs/heads/main/openapi/ev-energy-api-v2-openapi.yaml
authorization_urls: []
description: ''
docs: https://developers.ev.energy/docs/auth
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Ev Energy Scopes
name_suffix: OAuth Scopes
note: 'Scopes read verbatim from components.securitySchemes.oauth2.flows.clientCredentials.scopes in the published OpenAPI. The developer portal documents the OAuth flows but publishes NO scope reference page, so 26 of the 35 scopes ship with an empty description string in the spec and are recorded here as description_published: false rather than being given an invented meaning. The authorizationCode flow declares an empty scopes object in the spec even though the authentication page describes per-user consent to named scopes — the two flows are not consistently described. Scopes are assigned by ev.energy when it provisions the OAuth application; there is no self-service scope selection.'
overview: 'ev.energy publishes 35 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ev.energy API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ev.energy
provider_slug: ev-energy
schemes: []
scope_count: 35
scope_names:
- boundary_meter:read
- carbon:read
- charging_session:read
- charging_session:write
- debug:read
- dispatch_coordinator:read
- dispatch_event:write
- evse:read
- evse:write
- grid:read
- home_battery:read
- home_energy:read
- inverter:read
- inverter:write
- notification_preferences:read
- notification_preferences:write
- payout_method:read
- payout_method:write
- region:read
- region:write
- route_planner_preferences:read
- route_planner_preferences:write
- saved_routes:read
- saved_routes:write
- solar:read
- solar:write
- solar_forecast:read
- subscription:read
- tariff:prices:read
- tariff:read
- user:read
- user:write
- vehicle:read
- vehicle:write
- vehicle_catalogue:write
scopes:
- description: ''
  flows:
  - clientCredentials
  scope: boundary_meter:read
- description: ''
  flows:
  - clientCredentials
  scope: carbon:read
- description: ''
  flows:
  - clientCredentials
  scope: charging_session:read
- description: ''
  flows:
  - clientCredentials
  scope: charging_session:write
- description: ''
  flows:
  - clientCredentials
  scope: debug:read
- description: ''
  flows:
  - clientCredentials
  scope: dispatch_coordinator:read
- description: ''
  flows:
  - clientCredentials
  scope: dispatch_event:write
- description: ''
  flows:
  - clientCredentials
  scope: evse:read
- description: ''
  flows:
  - clientCredentials
  scope: evse:write
- description: ''
  flows:
  - clientCredentials
  scope: grid:read
- description: ''
  flows:
  - clientCredentials
  scope: home_battery:read
- description: ''
  flows:
  - clientCredentials
  scope: home_energy:read
- description: ''
  flows:
  - clientCredentials
  scope: inverter:read
- description: ''
  flows:
  - clientCredentials
  scope: inverter:write
- description: Read a user's notification group opt-in state
  flows:
  - clientCredentials
  scope: notification_preferences:read
- description: Update a user's notification group opt-in state
  flows:
  - clientCredentials
  scope: notification_preferences:write
- description: Read a user's preferred payout method
  flows:
  - clientCredentials
  scope: payout_method:read
- description: Set, update, or clear a user's preferred payout method
  flows:
  - clientCredentials
  scope: payout_method:write
- description: Read region and region group boundary data
  flows:
  - clientCredentials
  scope: region:read
- description: Create regions and region groups
  flows:
  - clientCredentials
  scope: region:write
- description: Read a user's EV Route Planner preferences
  flows:
  - clientCredentials
  scope: route_planner_preferences:read
- description: Update a user's EV Route Planner preferences
  flows:
  - clientCredentials
  scope: route_planner_preferences:write
- description: Read a user's saved route-planner routes
  flows:
  - clientCredentials
  scope: saved_routes:read
- description: Create, update, or delete a user's saved routes
  flows:
  - clientCredentials
  scope: saved_routes:write
- description: ''
  flows:
  - clientCredentials
  scope: solar:read
- description: ''
  flows:
  - clientCredentials
  scope: solar:write
- description: ''
  flows:
  - clientCredentials
  scope: solar_forecast:read
- description: ''
  flows:
  - clientCredentials
  scope: subscription:read
- description: ''
  flows:
  - clientCredentials
  scope: tariff:prices:read
- description: ''
  flows:
  - clientCredentials
  scope: tariff:read
- description: ''
  flows:
  - clientCredentials
  scope: user:read
- description: ''
  flows:
  - clientCredentials
  scope: user:write
- description: ''
  flows:
  - clientCredentials
  scope: vehicle:read
- description: ''
  flows:
  - clientCredentials
  scope: vehicle:write
- description: Update shared vehicle-catalogue reference data (e.g. a model's default connector type)
  flows:
  - clientCredentials
  scope: vehicle_catalogue:write
slug: ev-energy-scopes
source_filename: ev-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/ev-energy-api-v2-openapi.yaml\ndocs: https://developers.ev.energy/docs/auth\nnote: 'Scopes read verbatim from components.securitySchemes.oauth2.flows.clientCredentials.scopes in the\n  published OpenAPI. The developer portal documents the OAuth flows but publishes NO scope reference page,\n  so 26 of the 35 scopes ship with an empty description string in the spec and are recorded here as description_published:\n  false rather than being given an invented meaning. The authorizationCode flow declares an empty scopes\n  object in the spec even though the authentication page describes per-user consent to named scopes —\n  the two flows are not consistently described. Scopes are assigned by ev.energy when it provisions the\n  OAuth application; there is no self-service scope selection.'\nscheme:\n  name: oauth2\n  type: oauth2\n  authorizationUrl: https://api.ev.energy/o/authorize/\n  tokenUrl: https://api.ev.energy/o/token/\n\
  \  refreshUrl: https://api.ev.energy/o/token/\n  revocationUrl: https://api.ev.energy/o/revoke_token\n  flows:\n  - clientCredentials\n  - authorizationCode\nscope_count: 35\ndescribed_count: 11\nscopes:\n- scope: boundary_meter:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: carbon:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: charging_session:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: charging_session:write\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: debug:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n\
  \  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: dispatch_coordinator:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: dispatch_event:write\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: evse:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: evse:write\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: grid:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: home_battery:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n\
  \  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: home_energy:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: inverter:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: inverter:write\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: notification_preferences:read\n  flows:\n  - clientCredentials\n  description: Read a user's notification group opt-in state\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: notification_preferences:write\n  flows:\n  - clientCredentials\n  description: Update a user's notification group opt-in state\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: payout_method:read\n\
  \  flows:\n  - clientCredentials\n  description: Read a user's preferred payout method\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: payout_method:write\n  flows:\n  - clientCredentials\n  description: Set, update, or clear a user's preferred payout method\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: region:read\n  flows:\n  - clientCredentials\n  description: Read region and region group boundary data\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: region:write\n  flows:\n  - clientCredentials\n  description: Create regions and region groups\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: route_planner_preferences:read\n  flows:\n  - clientCredentials\n  description: Read a user's EV Route Planner preferences\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n\
  - scope: route_planner_preferences:write\n  flows:\n  - clientCredentials\n  description: Update a user's EV Route Planner preferences\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: saved_routes:read\n  flows:\n  - clientCredentials\n  description: Read a user's saved route-planner routes\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: saved_routes:write\n  flows:\n  - clientCredentials\n  description: Create, update, or delete a user's saved routes\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: solar:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: solar:write\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: solar_forecast:read\n  flows:\n\
  \  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: subscription:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: tariff:prices:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: tariff:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: user:read\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: user:write\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: vehicle:read\n  flows:\n  - clientCredentials\n\
  \  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: vehicle:write\n  flows:\n  - clientCredentials\n  description: null\n  description_published: false\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n- scope: vehicle_catalogue:write\n  flows:\n  - clientCredentials\n  description: Update shared vehicle-catalogue reference data (e.g. a model's default connector type)\n  description_published: true\n  sources:\n  - openapi/ev-energy-api-v2-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ev-energy/refs/heads/main/scopes/ev-energy-scopes.yml
summary_line: 35 scopes
tags:
- Company
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Utilities
- Sustainability
- Virtual Power Plant
- Demand Response
- Solar
- Home Energy
- Internet of Things
token_urls: []
---
