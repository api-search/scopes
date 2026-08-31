---
api_specs:
- filename: virtual-peaker-commands-api-openapi.yml
  format: yaml
  label: Virtual Peaker Commands API
  slug: virtual-peaker-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-commands-api-openapi.yml
- filename: virtual-peaker-devices-api-openapi.yml
  format: yaml
  label: Virtual Peaker Devices API
  slug: virtual-peaker-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-devices-api-openapi.yml
- filename: virtual-peaker-energy-interval-endpoint-api-openapi.yml
  format: yaml
  label: Virtual Peaker Energy Interval Endpoint API
  slug: virtual-peaker-energy-interval-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-energy-interval-endpoint-api-openapi.yml
- filename: virtual-peaker-group-management-api-openapi.yml
  format: yaml
  label: Virtual Peaker Group Management API
  slug: virtual-peaker-group-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-group-management-api-openapi.yml
- filename: virtual-peaker-oauth-device-discovery-preferred-api-openapi.yml
  format: yaml
  label: Virtual Peaker OAuth Device Discovery (Preferred) API
  slug: virtual-peaker-oauth-device-discovery-preferred-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-oauth-device-discovery-preferred-api-openapi.yml
- filename: virtual-peaker-pairing-code-device-discovery-end-user-app-api-openapi.yml
  format: yaml
  label: Virtual Peaker Pairing Code Device Discovery - End User App API
  slug: virtual-peaker-pairing-code-device-discovery-end-user-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-pairing-code-device-discovery-end-user-app-api-openapi.yml
- filename: virtual-peaker-pairing-code-device-discovery-utility-commissioned-installation-api-openapi.yml
  format: yaml
  label: Virtual Peaker Pairing Code Device Discovery - Utility Commissioned Installation API
  slug: virtual-peaker-pairing-code-device-discovery-utility-commissioned-installation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-pairing-code-device-discovery-utility-commissioned-installation-api-openapi.yml
- filename: virtual-peaker-publishing-api-openapi.yml
  format: yaml
  label: Virtual Peaker Publishing API
  slug: virtual-peaker-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-publishing-api-openapi.yml
authorization_urls:
- https://example.com/oauth/authorize
description: ''
docs: https://assets.virtualpeaker.io/gravity-connect/device-partner-api.html#section/Authentication
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Virtual Peaker Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Virtual Peaker publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Virtual Peaker API on a user''s behalf.


  Tokens are issued from https://example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Virtual Peaker
provider_slug: virtual-peaker
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/oauth/token
    tokenUrl_note: OEM-hosted; the published value is a placeholder
  name: device_partner_api_auth
  source: openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml
- description: If using the OAuth onboarding method, this authentication method is used for the respective endpoints. Please the the FAQ for more details.
  flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/oauth/token
  name: device_partner_user_auth
  source: openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml
scope_count: 3
scope_names:
- basic_partner_read_write
- user_read
- device_partner_basic_auth
scopes:
- description: conducts all actions on the partners behalf
  flows:
  - clientCredentials
  scope: basic_partner_read_write
- description: read details about new user
  flows:
  - authorizationCode
  scope: user_read
- description: ''
  flows: []
  scope: device_partner_basic_auth
slug: virtual-peaker-scopes
source_filename: virtual-peaker-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml\ndocs: https://assets.virtualpeaker.io/gravity-connect/device-partner-api.html#section/Authentication\ndocs_note: >-\n  Virtual Peaker publishes no scopes/permissions reference page. The Redoc guide renders the same\n  securitySchemes captured below and adds no scope beyond them, so this stays a derived artifact.\n  Scopes apply only to the device-partner half of Gravity Connect (VPP -> OEM); the publishing half\n  uses HMAC signatures and has no scope surface at all.\nschemes:\n- name: device_partner_api_auth\n  source: openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth/token\n    tokenUrl_note: OEM-hosted; the published value is a placeholder\n- name: device_partner_user_auth\n  source: openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\n  description: If using the OAuth onboarding method, this authentication method is used for\n    the respective endpoints. Please the the FAQ for more details.\nscopes:\n- scope: basic_partner_read_write\n  description: conducts all actions on the partners behalf\n  flows:\n  - clientCredentials\n  operations: 16\n  note: >-\n    A single coarse read/write scope covering every platform-to-partner operation — device reads,\n    signal/setting writes, commands, subscription changes and group management. There is no\n    read-only scope and no per-resource separation.\n  sources:\n  - openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml\n- scope: user_read\n  description: read details about new user\n  flows:\n  - authorizationCode\n  operations: [readCurrentUser, readCurrentUserDevices]\n  note: The homeowner-consented scope used\
  \ by OAuth Device Discovery.\n  sources:\n  - openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml\n- scope: device_partner_basic_auth\n  description: null\n  flows: []\n  status: spec-defect\n  note: >-\n    Referenced by the document's root `security` requirement\n    ({device_partner_api_auth: [device_partner_basic_auth]}) but declared by no flow. Every\n    operation-level requirement uses basic_partner_read_write instead. Treat this as a\n    documentation bug, not a real scope — do not request it.\n  sources:\n  - openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/scopes/virtual-peaker-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Energy
- United States
- Utilities
- Electricity
- Grid
- Demand Response
- DER
- DERMS
- Virtual Power Plant
- EV Charging
- Smart Thermostats
- Energy Storage
token_urls:
- https://example.com/oauth/token
---
