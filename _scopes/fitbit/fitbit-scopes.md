---
api_specs:
- filename: fitbit-activity-api-openapi.yml
  format: yaml
  label: Fitbit Activity API
  slug: fitbit-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-activity-api-openapi.yml
- filename: fitbit-heart-rate-api-openapi.yml
  format: yaml
  label: Fitbit Heart Rate API
  slug: fitbit-heart-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-heart-rate-api-openapi.yml
- filename: fitbit-sleep-api-openapi.yml
  format: yaml
  label: Fitbit Sleep API
  slug: fitbit-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-sleep-api-openapi.yml
- filename: fitbit-body-api-openapi.yml
  format: yaml
  label: Fitbit Body API
  slug: fitbit-body-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-body-api-openapi.yml
- filename: fitbit-nutrition-api-openapi.yml
  format: yaml
  label: Fitbit Nutrition API
  slug: fitbit-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-nutrition-api-openapi.yml
- filename: fitbit-user-api-openapi.yml
  format: yaml
  label: Fitbit User API
  slug: fitbit-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-user-api-openapi.yml
- filename: fitbit-devices-api-openapi.yml
  format: yaml
  label: Fitbit Devices API
  slug: fitbit-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-devices-api-openapi.yml
- filename: fitbit-subscriptions-api-openapi.yml
  format: yaml
  label: Fitbit Subscriptions API
  slug: fitbit-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-subscriptions-api-openapi.yml
- filename: fitbit-friends-api-openapi.yml
  format: yaml
  label: Fitbit Friends API
  slug: fitbit-friends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-friends-api-openapi.yml
- filename: fitbit-spo2-breathing-temperature-api-openapi.yml
  format: yaml
  label: Fitbit SpO2, Breathing Rate, Temperature, HRV, and Cardio Fitness API
  slug: fitbit-spo2-breathing-temperature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-spo2-breathing-temperature-api-openapi.yml
- filename: fitbit-ecg-irn-api-openapi.yml
  format: yaml
  label: Fitbit ECG and Irregular Rhythm Notifications API
  slug: fitbit-ecg-irn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-ecg-irn-api-openapi.yml
- filename: fitbit-authorization-api-openapi.yml
  format: yaml
  label: Fitbit Authorization API
  slug: fitbit-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/openapi/fitbit-authorization-api-openapi.yml
authorization_urls:
- https://www.fitbit.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Fitbit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fitbit publishes 15 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fitbit API on a user''s behalf.


  Tokens are issued from https://api.fitbit.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fitbit
provider_slug: fitbit
schemes:
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-activity-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-body-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-devices-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-ecg-irn-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-friends-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-heart-rate-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-nutrition-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-sleep-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-spo2-breathing-temperature-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-subscriptions-api-openapi.yml
- flows:
  - authorizationUrl: https://www.fitbit.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.fitbit.com/oauth2/token
  name: OAuth2
  source: openapi/fitbit-user-api-openapi.yml
scope_count: 15
scope_names:
- activity
- cardio_fitness
- electrocardiogram
- heartrate
- irregular_rhythm_notifications
- location
- nutrition
- oxygen_saturation
- profile
- respiratory_rate
- settings
- sleep
- social
- temperature
- weight
scopes:
- description: Activity and exercise data
  flows:
  - authorizationCode
  scope: activity
- description: Cardio fitness (VO2 Max) data
  flows:
  - authorizationCode
  scope: cardio_fitness
- description: ECG readings
  flows:
  - authorizationCode
  scope: electrocardiogram
- description: Heart rate data
  flows:
  - authorizationCode
  scope: heartrate
- description: IRN data
  flows:
  - authorizationCode
  scope: irregular_rhythm_notifications
- description: GPS and other location data
  flows:
  - authorizationCode
  scope: location
- description: Food and nutrition data
  flows:
  - authorizationCode
  scope: nutrition
- description: SpO2 data
  flows:
  - authorizationCode
  scope: oxygen_saturation
- description: User profile
  flows:
  - authorizationCode
  scope: profile
- description: Breathing rate data
  flows:
  - authorizationCode
  scope: respiratory_rate
- description: Account settings
  flows:
  - authorizationCode
  scope: settings
- description: Sleep data
  flows:
  - authorizationCode
  scope: sleep
- description: Friends and leaderboard data
  flows:
  - authorizationCode
  scope: social
- description: Skin and core body temperature data
  flows:
  - authorizationCode
  scope: temperature
- description: Weight, BMI, and body fat data
  flows:
  - authorizationCode
  scope: weight
slug: fitbit-scopes
source_filename: fitbit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fitbit-activity-api-openapi.yml, openapi/fitbit-body-api-openapi.yml, openapi/fitbit-devices-api-openapi.yml,\n  openapi/fitbit-ecg-irn-api-openapi.yml, openapi/fitbit-friends-api-openapi.yml, openapi/fitbit-heart-rate-api-openapi.yml,\n  openapi/fitbit-nutrition-api-openapi.yml, openapi/fitbit-sleep-api-openapi.yml, openapi/fitbit-spo2-breathing-temperature-api-openapi.yml,\n  openapi/fitbit-subscriptions-api-openapi.yml, openapi/fitbit-user-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/fitbit-activity-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source: openapi/fitbit-body-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source:\
  \ openapi/fitbit-devices-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source: openapi/fitbit-ecg-irn-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source: openapi/fitbit-friends-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source: openapi/fitbit-heart-rate-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source: openapi/fitbit-nutrition-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n\
  \    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source: openapi/fitbit-sleep-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source: openapi/fitbit-spo2-breathing-temperature-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source: openapi/fitbit-subscriptions-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\n- name: OAuth2\n  source: openapi/fitbit-user-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fitbit.com/oauth2/authorize\n    tokenUrl: https://api.fitbit.com/oauth2/token\nscopes:\n- scope: activity\n  description: Activity\
  \ and exercise data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-subscriptions-api-openapi.yml\n- scope: cardio_fitness\n  description: Cardio fitness (VO2 Max) data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-spo2-breathing-temperature-api-openapi.yml\n- scope: electrocardiogram\n  description: ECG readings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-ecg-irn-api-openapi.yml\n- scope: heartrate\n  description: Heart rate data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-heart-rate-api-openapi.yml\n  - openapi/fitbit-spo2-breathing-temperature-api-openapi.yml\n  - openapi/fitbit-subscriptions-api-openapi.yml\n- scope: irregular_rhythm_notifications\n  description: IRN data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n\
  \  - openapi/fitbit-ecg-irn-api-openapi.yml\n- scope: location\n  description: GPS and other location data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n- scope: nutrition\n  description: Food and nutrition data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-nutrition-api-openapi.yml\n  - openapi/fitbit-subscriptions-api-openapi.yml\n- scope: oxygen_saturation\n  description: SpO2 data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-spo2-breathing-temperature-api-openapi.yml\n- scope: profile\n  description: User profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-user-api-openapi.yml\n- scope: respiratory_rate\n  description: Breathing rate data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-spo2-breathing-temperature-api-openapi.yml\n\
  - scope: settings\n  description: Account settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-devices-api-openapi.yml\n  - openapi/fitbit-user-api-openapi.yml\n- scope: sleep\n  description: Sleep data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-sleep-api-openapi.yml\n  - openapi/fitbit-subscriptions-api-openapi.yml\n- scope: social\n  description: Friends and leaderboard data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-friends-api-openapi.yml\n- scope: temperature\n  description: Skin and core body temperature data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n  - openapi/fitbit-spo2-breathing-temperature-api-openapi.yml\n- scope: weight\n  description: Weight, BMI, and body fat data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitbit-activity-api-openapi.yml\n\
  \  - openapi/fitbit-body-api-openapi.yml\n  - openapi/fitbit-subscriptions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fitbit/refs/heads/main/scopes/fitbit-scopes.yml
summary_line: 15 scopes · authorizationCode
tags:
- Wearable
- Health
- Fitness
- Activity Tracking
- Heart Rate
- Sleep
- Google
- IoT
token_urls:
- https://api.fitbit.com/oauth2/token
---
