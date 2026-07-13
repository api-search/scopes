---
api_specs:
- filename: fitness.yml
  format: yaml
  label: Google Fit REST API v1
  slug: google-fit-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-fitness/refs/heads/main/openapi/fitness.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Fitness Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Fit REST publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Fit REST API on a user''s behalf.


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
  source: openapi/fitness.yml
scope_count: 6
scope_names:
- https://www.googleapis.com/auth/fitness.activity.read
- https://www.googleapis.com/auth/fitness.activity.write
- https://www.googleapis.com/auth/fitness.body.read
- https://www.googleapis.com/auth/fitness.body.write
- https://www.googleapis.com/auth/fitness.location.read
- https://www.googleapis.com/auth/fitness.location.write
scopes:
- description: View your activity information in Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.activity.read
- description: Add to your activity information in Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.activity.write
- description: View body sensor information in Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.body.read
- description: Add body sensor information in Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.body.write
- description: View your stored location data in Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.location.read
- description: Add to your location data in Google Fit
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/fitness.location.write
slug: google-fitness-scopes
source_filename: google-fitness-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fitness.yml\nschemes:\n- name: oauth2\n  source: openapi/fitness.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/fitness.activity.read\n  description: View your activity information in Google Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitness.yml\n- scope: https://www.googleapis.com/auth/fitness.activity.write\n  description: Add to your activity information in Google Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitness.yml\n- scope: https://www.googleapis.com/auth/fitness.body.read\n  description: View body sensor information in Google Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitness.yml\n- scope: https://www.googleapis.com/auth/fitness.body.write\n  description: Add body sensor information in Google\
  \ Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitness.yml\n- scope: https://www.googleapis.com/auth/fitness.location.read\n  description: View your stored location data in Google Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitness.yml\n- scope: https://www.googleapis.com/auth/fitness.location.write\n  description: Add to your location data in Google Fit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fitness.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-fitness/refs/heads/main/scopes/google-fitness-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Activity Tracking
- Fitness
- Google
- Health
- Sessions
- Wearables
- Wellness
token_urls:
- https://oauth2.googleapis.com/token
---
