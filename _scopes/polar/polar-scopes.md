---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: Polar AccessLink API
  slug: polar-accesslink-api
  spec_type: OpenAPI
  url: https://www.polar.com/accesslink-api/swagger.yaml
- filename: swagger.yaml
  format: yaml
  label: Polar TeamPro API
  slug: polar-teampro-api
  spec_type: OpenAPI
  url: https://www.polar.com/teampro-api/swagger.yaml
authorization_urls:
- https://flow.polar.com/oauth2/authorization
- https://auth.polar.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Polar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Polar publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Polar API on a user''s behalf.


  Tokens are issued from https://polarremote.com/v2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Polar
provider_slug: polar
schemes:
- flows:
  - authorizationUrl: https://flow.polar.com/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://polarremote.com/v2/oauth2/token
  name: OAuth2
  source: openapi/polar-accesslink-api-openapi.yml
- flows:
  - authorizationUrl: https://auth.polar.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.polar.com/oauth/token
  name: OAuth2
  source: openapi/polar-teampro-api-openapi.yml
scope_count: 2
scope_names:
- accesslink.read_all
- team_read
scopes:
- description: Allows read access to user's data
  flows:
  - authorizationCode
  scope: accesslink.read_all
- description: Allows read access to user's data
  flows:
  - authorizationCode
  scope: team_read
slug: polar-scopes
source_filename: polar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polar-accesslink-api-openapi.yml, openapi/polar-teampro-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/polar-accesslink-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://flow.polar.com/oauth2/authorization\n    tokenUrl: https://polarremote.com/v2/oauth2/token\n- name: OAuth2\n  source: openapi/polar-teampro-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.polar.com/oauth/authorize\n    tokenUrl: https://auth.polar.com/oauth/token\nscopes:\n- scope: accesslink.read_all\n  description: Allows read access to user's data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/polar-accesslink-api-openapi.yml\n- scope: team_read\n  description: Allows read access to user's data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/polar-teampro-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/scopes/polar-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Fitness
- Health
- Wearables
- Heart Rate
- Sports
- Training
- Sleep
- Activity Tracking
- Sensors
- Bluetooth
token_urls:
- https://polarremote.com/v2/oauth2/token
- https://auth.polar.com/oauth/token
---
