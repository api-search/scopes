---
api_specs:
- filename: airthings-accounts-api-openapi.yml
  format: yaml
  label: Airthings Accounts API
  slug: airthings-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-accounts-api-openapi.yml
- filename: airthings-device-api-openapi.yml
  format: yaml
  label: Airthings Device API
  slug: airthings-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-device-api-openapi.yml
- filename: airthings-devices-api-openapi.yml
  format: yaml
  label: Airthings Devices API
  slug: airthings-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-devices-api-openapi.yml
- filename: airthings-health-api-openapi.yml
  format: yaml
  label: Airthings Health API
  slug: airthings-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-health-api-openapi.yml
- filename: airthings-locations-api-openapi.yml
  format: yaml
  label: Airthings Locations API
  slug: airthings-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-locations-api-openapi.yml
- filename: airthings-organizations-api-openapi.yml
  format: yaml
  label: Airthings Organizations API
  slug: airthings-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-organizations-api-openapi.yml
- filename: airthings-segments-api-openapi.yml
  format: yaml
  label: Airthings Segments API
  slug: airthings-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-segments-api-openapi.yml
- filename: airthings-sensor-api-openapi.yml
  format: yaml
  label: Airthings Sensor API
  slug: airthings-sensor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-sensor-api-openapi.yml
- filename: airthings-spaces-api-openapi.yml
  format: yaml
  label: Airthings Spaces API
  slug: airthings-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-spaces-api-openapi.yml
- filename: airthings-thresholds-api-openapi.yml
  format: yaml
  label: Airthings Thresholds API
  slug: airthings-thresholds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-thresholds-api-openapi.yml
- filename: airthings-webhooks-api-openapi.yml
  format: yaml
  label: Airthings Webhooks API
  slug: airthings-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-webhooks-api-openapi.yml
authorization_urls:
- https://accounts.airthings.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Airthings Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Airthings publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Airthings API on a user''s behalf.


  Tokens are issued from https://accounts-api.airthings.com/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Airthings
provider_slug: airthings
schemes:
- flows:
  - authorizationUrl: https://accounts.airthings.com/authorize
    flow: authorizationCode
    tokenUrl: https://accounts-api.airthings.com/v1/token
  - flow: clientCredentials
    tokenUrl: https://accounts-api.airthings.com/v1/token
  name: AirthingsAccounts
  source: openapi/airthings-api-openapi.yml
scope_count: 2
scope_names:
- read:device
- write:device
scopes:
- description: Allowing a user to read data from devices in their account
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:device
- description: Allowing a user to manage devices within their account
  flows:
  - authorizationCode
  - clientCredentials
  scope: write:device
slug: airthings-scopes
source_filename: airthings-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/airthings-api-openapi.yml\nschemes:\n- name: AirthingsAccounts\n  source: openapi/airthings-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.airthings.com/authorize\n    tokenUrl: https://accounts-api.airthings.com/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://accounts-api.airthings.com/v1/token\nscopes:\n- scope: read:device\n  description: Allowing a user to read data from devices in their account\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/airthings-api-openapi.yml\n- scope: write:device\n  description: Allowing a user to manage devices within their account\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/airthings-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/airthings/scopes/airthings-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Company
- AirQuality
- Radon
- Sensors
- IoT
token_bound: false
token_urls:
- https://accounts-api.airthings.com/v1/token
---
