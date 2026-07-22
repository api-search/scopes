---
api_specs:
- filename: ninjaone-openapi-original.yml
  format: yaml
  label: NinjaOne Public API 2.0
  slug: ninjaone-public-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjaone/refs/heads/main/openapi/ninjaone-openapi-original.yml
authorization_urls:
- https://app.ninjarmm.com/ws/oauth/authorize
description: ''
docs: https://www.ninjaone.com/docs/application-programming-interface-api/oauth-token-configuration/
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ninjaone Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NinjaOne publishes 4 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the NinjaOne API on a user''s behalf.


  Tokens are issued from https://app.ninjarmm.com/ws/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NinjaOne
provider_slug: ninjaone
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.ninjarmm.com/ws/oauth/token
  - authorizationUrl: https://app.ninjarmm.com/ws/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.ninjarmm.com/ws/oauth/token
  name: oauth2
  source: openapi/ninjaone-openapi-original.yml
scope_count: 4
scope_names:
- monitoring
- management
- control
- offline_access
scopes:
- description: Read-only access to monitoring data and organization structure — devices, alerts, activities, and reports. Grants GET access across the platform.
  flows:
  - clientCredentials
  - authorizationCode
  scope: monitoring
- description: Modify device and organization information — create organizations, add devices, run scripts, manage policies, tickets, and custom fields.
  flows:
  - clientCredentials
  - authorizationCode
  scope: management
- description: Enable remote access / remote control of endpoints via the API.
  flows:
  - clientCredentials
  - authorizationCode
  scope: control
- description: Request a refresh token (authorization-code flow) so an access token can be renewed without re-authenticating.
  flows:
  - authorizationCode
  scope: offline_access
slug: ninjaone-scopes
source_filename: ninjaone-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://app.ninjarmm.com/.well-known/oauth-authorization-server\ndocs: https://www.ninjaone.com/docs/application-programming-interface-api/oauth-token-configuration/\nschemes:\n- name: oauth2\n  source: openapi/ninjaone-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.ninjarmm.com/ws/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://app.ninjarmm.com/ws/oauth/authorize\n    tokenUrl: https://app.ninjarmm.com/ws/oauth/token\nscopes:\n- scope: monitoring\n  description: >-\n    Read-only access to monitoring data and organization structure — devices,\n    alerts, activities, and reports. Grants GET access across the platform.\n  flows: [clientCredentials, authorizationCode]\n- scope: management\n  description: >-\n    Modify device and organization information — create organizations, add\n    devices, run scripts, manage policies, tickets, and custom fields.\n  flows:\
  \ [clientCredentials, authorizationCode]\n- scope: control\n  description: >-\n    Enable remote access / remote control of endpoints via the API.\n  flows: [clientCredentials, authorizationCode]\n- scope: offline_access\n  description: >-\n    Request a refresh token (authorization-code flow) so an access token can be\n    renewed without re-authenticating.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninjaone/refs/heads/main/scopes/ninjaone-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode
tags:
- Company
- Developer Tools
- IT Management
- RMM
- Endpoint Management
- MSP
- IT Operations
- Monitoring
- Automation
- Ticketing
token_urls:
- https://app.ninjarmm.com/ws/oauth/token
---
