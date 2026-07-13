---
api_specs:
- filename: gridshare-partner-api-openapi.yml
  format: yaml
  label: Gridshare Partner API
  slug: gridshare-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/gridshare-partner-api-openapi.yml
- filename: gridshare-customer-api-openapi.yml
  format: yaml
  label: Gridshare Customer API
  slug: gridshare-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/openapi/gridshare-customer-api-openapi.yml
authorization_urls:
- https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Lunar Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lunar Energy publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lunar Energy API on a user''s behalf.


  Tokens are issued from https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lunar Energy
provider_slug: lunar-energy
schemes:
- description: 'OAuth 2.0 Authorization Code flow against the lunar-customer

    Amazon Cognito user pool.'
  flows:
  - authorizationUrl: https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/token
  name: bearerAuth
  source: openapi/gridshare-customer-api-openapi.yml
scope_count: 4
scope_names:
- lunar/device.read
- lunar/device.write
- lunar/plan.read
- lunar/plan.write
scopes:
- description: Read device metadata and telemetry (excluding plans)
  flows:
  - authorizationCode
  scope: lunar/device.read
- description: Modify devices including operation mode
  flows:
  - authorizationCode
  scope: lunar/device.write
- description: Read existing device plans
  flows:
  - authorizationCode
  scope: lunar/plan.read
- description: Send plans to a device
  flows:
  - authorizationCode
  scope: lunar/plan.write
slug: lunar-energy-scopes
source_filename: lunar-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gridshare-customer-api-openapi.yml\nschemes:\n- name: bearerAuth\n  source: openapi/gridshare-customer-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/token\n  description: |-\n    OAuth 2.0 Authorization Code flow against the lunar-customer\n    Amazon Cognito user pool.\nscopes:\n- scope: lunar/device.read\n  description: Read device metadata and telemetry (excluding plans)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gridshare-customer-api-openapi.yml\n- scope: lunar/device.write\n  description: Modify devices including operation mode\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gridshare-customer-api-openapi.yml\n- scope: lunar/plan.read\n  description: Read existing device plans\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/gridshare-customer-api-openapi.yml\n- scope: lunar/plan.write\n  description: Send plans to a device\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gridshare-customer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunar-energy/refs/heads/main/scopes/lunar-energy-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Energy
- Home Battery
- Solar
- Virtual Power Plant
- DERMS
- Distributed Energy Resources
- Grid Services
- Demand Response
- Storage
- Inverter
- Smart Home
- Energy Management
- Tariffs
- Telemetry
- VPP
- Flex Events
token_urls:
- https://lunar-customer-prod-us-west-1.auth.us-west-1.amazoncognito.com/oauth2/token
---
