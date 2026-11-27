---
api_specs:
- filename: google-nest-enterprises-api-openapi.yml
  format: yaml
  label: Google Nest Smart Device Management Nest Enterprises API
  slug: google-nest-enterprises-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-nest/openapi/google-nest-enterprises-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Nest Smart Device Management Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Nest Smart Device Management publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Nest Smart Device Management API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Nest Smart Device Management
provider_slug: google-nest
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-nest-enterprises-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/sdm.service
scopes:
- description: See and/or control the devices that you selected
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/sdm.service
slug: google-nest-scopes
source_filename: google-nest-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-nest-enterprises-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-nest-enterprises-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/sdm.service\n  description: See and/or control the devices that you selected\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-nest-enterprises-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-nest/scopes/google-nest-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Camera
- Device Management
- Doorbell
- Google Nest
- IoT
- Smart Home
- Thermostat
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
