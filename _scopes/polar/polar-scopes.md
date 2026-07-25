---
api_specs:
- filename: polar-cardio-load-api-openapi.yml
  format: yaml
  label: Polar Cardio load API
  slug: polar-cardio-load-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-cardio-load-api-openapi.yml
- filename: polar-continuous-heart-rate-api-openapi.yml
  format: yaml
  label: Polar Continuous Heart Rate API
  slug: polar-continuous-heart-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-continuous-heart-rate-api-openapi.yml
- filename: polar-daily-activity-api-openapi.yml
  format: yaml
  label: Polar Daily activity API
  slug: polar-daily-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-daily-activity-api-openapi.yml
- filename: polar-daily-activity-deprecated-api-openapi.yml
  format: yaml
  label: Polar Daily activity (deprecated) API
  slug: polar-daily-activity-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-daily-activity-deprecated-api-openapi.yml
- filename: polar-elixir-trade-biosensing-api-openapi.yml
  format: yaml
  label: Polar Elixir&trade; Biosensing API
  slug: polar-elixir-trade-biosensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-elixir-trade-biosensing-api-openapi.yml
- filename: polar-exercises-api-openapi.yml
  format: yaml
  label: Polar Exercises API
  slug: polar-exercises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-exercises-api-openapi.yml
- filename: polar-exercises-deprecated-api-openapi.yml
  format: yaml
  label: Polar Exercises (deprecated) API
  slug: polar-exercises-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-exercises-deprecated-api-openapi.yml
- filename: polar-nightly-recharge-api-openapi.yml
  format: yaml
  label: Polar Nightly Recharge API
  slug: polar-nightly-recharge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-nightly-recharge-api-openapi.yml
- filename: polar-physical-info-api-openapi.yml
  format: yaml
  label: Polar Physical info API
  slug: polar-physical-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-physical-info-api-openapi.yml
- filename: polar-physical-info-deprecated-api-openapi.yml
  format: yaml
  label: Polar Physical info (deprecated) API
  slug: polar-physical-info-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-physical-info-deprecated-api-openapi.yml
- filename: polar-player-training-sessions-api-openapi.yml
  format: yaml
  label: Polar Player training sessions API
  slug: polar-player-training-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-player-training-sessions-api-openapi.yml
- filename: polar-pull-notifications-api-openapi.yml
  format: yaml
  label: Polar Pull notifications API
  slug: polar-pull-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-pull-notifications-api-openapi.yml
- filename: polar-sleep-api-openapi.yml
  format: yaml
  label: Polar Sleep API
  slug: polar-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-sleep-api-openapi.yml
- filename: polar-sleepwise-trade-api-openapi.yml
  format: yaml
  label: Polar SleepWise&trade; API
  slug: polar-sleepwise-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-sleepwise-trade-api-openapi.yml
- filename: polar-team-api-openapi.yml
  format: yaml
  label: Polar Team API
  slug: polar-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-team-api-openapi.yml
- filename: polar-team-training-sessions-api-openapi.yml
  format: yaml
  label: Polar Team training sessions API
  slug: polar-team-training-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-team-training-sessions-api-openapi.yml
- filename: polar-users-api-openapi.yml
  format: yaml
  label: Polar Users API
  slug: polar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-users-api-openapi.yml
- filename: polar-webhooks-api-openapi.yml
  format: yaml
  label: Polar Webhooks API
  slug: polar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-webhooks-api-openapi.yml
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
