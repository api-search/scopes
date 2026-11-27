---
api_specs:
- filename: google-fitness-users-api-openapi.yml
  format: yaml
  label: Google Fit REST Users API
  slug: google-fitness-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-fitness/openapi/google-fitness-users-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Fit REST Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Fit REST publishes 22 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Fit REST API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Fit REST
provider_slug: google-fitness
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-fitness-users-api-openapi.yml
scope_count: 22
scope_names:
- https://www.googleapis.com/auth/fitness.activity.read
- https://www.googleapis.com/auth/fitness.activity.write
- https://www.googleapis.com/auth/fitness.blood_glucose.read
- https://www.googleapis.com/auth/fitness.blood_glucose.write
- https://www.googleapis.com/auth/fitness.blood_pressure.read
- https://www.googleapis.com/auth/fitness.blood_pressure.write
- https://www.googleapis.com/auth/fitness.body.read
- https://www.googleapis.com/auth/fitness.body.write
- https://www.googleapis.com/auth/fitness.body_temperature.read
- https://www.googleapis.com/auth/fitness.body_temperature.write
- https://www.googleapis.com/auth/fitness.heart_rate.read
- https://www.googleapis.com/auth/fitness.heart_rate.write
- https://www.googleapis.com/auth/fitness.location.read
- https://www.googleapis.com/auth/fitness.location.write
- https://www.googleapis.com/auth/fitness.nutrition.read
- https://www.googleapis.com/auth/fitness.nutrition.write
- https://www.googleapis.com/auth/fitness.oxygen_saturation.read
- https://www.googleapis.com/auth/fitness.oxygen_saturation.write
- https://www.googleapis.com/auth/fitness.reproductive_health.read
- https://www.googleapis.com/auth/fitness.reproductive_health.write
- https://www.googleapis.com/auth/fitness.sleep.read
- https://www.googleapis.com/auth/fitness.sleep.write
scopes:
- description: Use Google Fit to see and store your physical activity data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.activity.read
- description: Add to your Google Fit physical activity data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.activity.write
- description: See info about your blood glucose in Google Fit. I consent to Google sharing my blood glucose information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.blood_glucose.read
- description: Add info about your blood glucose to Google Fit. I consent to Google using my blood glucose information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.blood_glucose.write
- description: See info about your blood pressure in Google Fit. I consent to Google sharing my blood pressure information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.blood_pressure.read
- description: Add info about your blood pressure in Google Fit. I consent to Google using my blood pressure information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.blood_pressure.write
- description: See info about your body measurements in Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.body.read
- description: Add info about your body measurements to Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.body.write
- description: See info about your body temperature in Google Fit. I consent to Google sharing my body temperature information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.body_temperature.read
- description: Add to info about your body temperature in Google Fit. I consent to Google using my body temperature information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.body_temperature.write
- description: See your heart rate data in Google Fit. I consent to Google sharing my heart rate information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.heart_rate.read
- description: Add to your heart rate data in Google Fit. I consent to Google using my heart rate information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.heart_rate.write
- description: See your Google Fit speed and distance data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.location.read
- description: Add to your Google Fit location data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.location.write
- description: See info about your nutrition in Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.nutrition.read
- description: Add to info about your nutrition in Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.nutrition.write
- description: See info about your oxygen saturation in Google Fit. I consent to Google sharing my oxygen saturation information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.oxygen_saturation.read
- description: Add info about your oxygen saturation in Google Fit. I consent to Google using my oxygen saturation information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.oxygen_saturation.write
- description: See info about your reproductive health in Google Fit. I consent to Google sharing my reproductive health information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.reproductive_health.read
- description: Add info about your reproductive health in Google Fit. I consent to Google using my reproductive health information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.reproductive_health.write
- description: See your sleep data in Google Fit. I consent to Google sharing my sleep information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.sleep.read
- description: Add to your sleep data in Google Fit. I consent to Google using my sleep information with this app.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.sleep.write
slug: google-fitness-scopes
source_filename: google-fitness-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-fitness-users-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-fitness-users-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/fitness.activity.read\n  description: Use Google Fit to see and store your physical activity data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.activity.write\n  description: Add to your Google Fit physical activity data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.blood_glucose.read\n  description: See info about your blood glucose in Google Fit. I consent to Google sharing\n    my blood glucose information\
  \ with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.blood_glucose.write\n  description: Add info about your blood glucose to Google Fit. I consent to Google using my\n    blood glucose information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.blood_pressure.read\n  description: See info about your blood pressure in Google Fit. I consent to Google sharing\n    my blood pressure information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.blood_pressure.write\n  description: Add info about your blood pressure in Google Fit. I consent to Google using my\n    blood pressure information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/fitness.body.read\n  description: See info about your body measurements in Google Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.body.write\n  description: Add info about your body measurements to Google Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.body_temperature.read\n  description: See info about your body temperature in Google Fit. I consent to Google sharing\n    my body temperature information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.body_temperature.write\n  description: Add to info about your body temperature in Google Fit. I consent to Google using\n    my body temperature information with this app.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.heart_rate.read\n  description: See your heart rate data in Google Fit. I consent to Google sharing my heart\n    rate information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.heart_rate.write\n  description: Add to your heart rate data in Google Fit. I consent to Google using my heart\n    rate information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.location.read\n  description: See your Google Fit speed and distance data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.location.write\n  description: Add to your Google Fit location data\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.nutrition.read\n  description: See info about your nutrition in Google Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.nutrition.write\n  description: Add to info about your nutrition in Google Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.oxygen_saturation.read\n  description: See info about your oxygen saturation in Google Fit. I consent to Google sharing\n    my oxygen saturation information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.oxygen_saturation.write\n  description: Add info about your oxygen saturation in Google Fit. I consent to Google using\n    my\
  \ oxygen saturation information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.reproductive_health.read\n  description: See info about your reproductive health in Google Fit. I consent to Google sharing\n    my reproductive health information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.reproductive_health.write\n  description: Add info about your reproductive health in Google Fit. I consent to Google using\n    my reproductive health information with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.sleep.read\n  description: See your sleep data in Google Fit. I consent to Google sharing my sleep information\n    with this app.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n- scope: https://www.googleapis.com/auth/fitness.sleep.write\n  description: Add to your sleep data in Google Fit. I consent to Google using my sleep information\n    with this app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-fitness-users-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-fitness/scopes/google-fitness-scopes.yml
summary_line: 22 scopes · authorizationCode
tags:
- Activity Tracking
- Fitness
- Google
- Health
- Sessions
- Wearables
- Wellness
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
