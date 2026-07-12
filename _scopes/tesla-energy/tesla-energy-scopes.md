---
authorization_urls:
- https://auth.tesla.com/oauth2/v3/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Tesla Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tesla Energy publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tesla Energy API on a user''s behalf.


  Tokens are issued from https://auth.tesla.com/oauth2/v3/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tesla Energy
provider_slug: tesla-energy
schemes:
- description: Tesla Fleet API OAuth 2.0 with PKCE. Scopes energy_device_data (read) and energy_cmds (write) required for the energy_sites endpoints.
  flows:
  - authorizationUrl: https://auth.tesla.com/oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tesla.com/oauth2/v3/token
  name: BearerAuth
  source: openapi/tesla-energy-fleet-api-openapi.yml
scope_count: 3
scope_names:
- energy_cmds
- energy_device_data
- offline_access
scopes:
- description: Send commands to energy sites
  flows:
  - authorizationCode
  scope: energy_cmds
- description: Read energy site data
  flows:
  - authorizationCode
  scope: energy_device_data
- description: Refresh tokens
  flows:
  - authorizationCode
  scope: offline_access
slug: tesla-energy-scopes
source_filename: tesla-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tesla-energy-fleet-api-openapi.yml\nschemes:\n- name: BearerAuth\n  source: openapi/tesla-energy-fleet-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tesla.com/oauth2/v3/authorize\n    tokenUrl: https://auth.tesla.com/oauth2/v3/token\n  description: Tesla Fleet API OAuth 2.0 with PKCE. Scopes energy_device_data (read) and energy_cmds\n    (write) required for the energy_sites endpoints.\nscopes:\n- scope: energy_cmds\n  description: Send commands to energy sites\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tesla-energy-fleet-api-openapi.yml\n- scope: energy_device_data\n  description: Read energy site data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tesla-energy-fleet-api-openapi.yml\n- scope: offline_access\n  description: Refresh tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tesla-energy-fleet-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/scopes/tesla-energy-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Energy
- Clean Energy
- Solar
- Battery Storage
- Powerwall
- Megapack
- Solar Roof
- Virtual Power Plant
- IoT
- Grid Services
- Home Energy
- Utility Scale
token_urls:
- https://auth.tesla.com/oauth2/v3/token
---
