---
authorization_urls:
- https://cloud.ouraring.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Oura Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Oura Ring publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Oura Ring API on a user''s behalf.


  Tokens are issued from https://api.ouraring.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oura Ring
provider_slug: oura
schemes:
- flows:
  - authorizationUrl: https://cloud.ouraring.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.ouraring.com/oauth/token
  name: OAuth2
  source: openapi/oura-oura-ring-api-openapi.yml
scope_count: 8
scope_names:
- daily
- email
- heartrate
- personal
- session
- spo2Daily
- tag
- workout
scopes:
- description: Daily summaries of sleep, activity and readiness
  flows:
  - authorizationCode
  scope: daily
- description: Email address of the user
  flows:
  - authorizationCode
  scope: email
- description: Time series heart rate for Gen 3 users
  flows:
  - authorizationCode
  scope: heartrate
- description: Personal information (gender, age, height, weight)
  flows:
  - authorizationCode
  scope: personal
- description: Guided and unguided sessions in the Oura app
  flows:
  - authorizationCode
  scope: session
- description: SpO2 Average recorded during sleep
  flows:
  - authorizationCode
  scope: spo2Daily
- description: User entered tags
  flows:
  - authorizationCode
  scope: tag
- description: Summaries for auto-detected and user entered workouts
  flows:
  - authorizationCode
  scope: workout
slug: oura-scopes
source_filename: oura-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oura-oura-ring-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/oura-oura-ring-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloud.ouraring.com/oauth/authorize\n    tokenUrl: https://api.ouraring.com/oauth/token\nscopes:\n- scope: daily\n  description: Daily summaries of sleep, activity and readiness\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n- scope: email\n  description: Email address of the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n- scope: heartrate\n  description: Time series heart rate for Gen 3 users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n- scope: personal\n  description: Personal information (gender, age, height, weight)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n\
  - scope: session\n  description: Guided and unguided sessions in the Oura app\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n- scope: spo2Daily\n  description: SpO2 Average recorded during sleep\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n- scope: tag\n  description: User entered tags\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n- scope: workout\n  description: Summaries for auto-detected and user entered workouts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oura/refs/heads/main/scopes/oura-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Health
- Wearables
- Sleep
- Fitness
- Heart Rate
- Readiness
- Smart Ring
- Biometrics
token_urls:
- https://api.ouraring.com/oauth/token
---
