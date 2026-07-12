---
authorization_urls:
- https://oauth.trainingpeaks.com/OAuth/Authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Trainingpeaks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TrainingPeaks publishes 17 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TrainingPeaks API on a user''s behalf.


  Tokens are issued from https://oauth.trainingpeaks.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TrainingPeaks
provider_slug: trainingpeaks
schemes:
- description: OAuth 2.0 authorization code flow. Tokens are short-lived (expires_in seconds) and refreshed with the refresh_token grant. Scopes are not inclusive (e.g. workouts:details does not include workouts:read) and are limited to those granted to your application.
  flows:
  - authorizationUrl: https://oauth.trainingpeaks.com/OAuth/Authorize
    flow: authorizationCode
    tokenUrl: https://oauth.trainingpeaks.com/oauth/token
  name: OAuth2
  source: openapi/trainingpeaks-openapi.yml
scope_count: 17
scope_names:
- athlete:profile
- coach:athletes
- events:read
- events:write
- file:write
- metrics:read
- metrics:write
- nutrition:read
- nutrition:write
- routes:read
- routes:write
- webhook:read-subscriptions
- webhook:write-subscriptions
- workouts:details
- workouts:plan
- workouts:read
- workouts:wod
scopes:
- description: Read the authenticated athlete's profile and zones.
  flows:
  - authorizationCode
  scope: athlete:profile
- description: Read coach profile, athletes, and assistants.
  flows:
  - authorizationCode
  scope: coach:athletes
- description: Read athlete events.
  flows:
  - authorizationCode
  scope: events:read
- description: Create athlete events.
  flows:
  - authorizationCode
  scope: events:write
- description: Upload activity files.
  flows:
  - authorizationCode
  scope: file:write
- description: Read athlete metrics.
  flows:
  - authorizationCode
  scope: metrics:read
- description: Create athlete metrics.
  flows:
  - authorizationCode
  scope: metrics:write
- description: Read athlete nutrition entries.
  flows:
  - authorizationCode
  scope: nutrition:read
- description: Create, update, and delete nutrition entries.
  flows:
  - authorizationCode
  scope: nutrition:write
- description: Read athlete routes.
  flows:
  - authorizationCode
  scope: routes:read
- description: Create athlete routes.
  flows:
  - authorizationCode
  scope: routes:write
- description: List webhook subscriptions.
  flows:
  - authorizationCode
  scope: webhook:read-subscriptions
- description: Create, update, and delete webhook subscriptions.
  flows:
  - authorizationCode
  scope: webhook:write-subscriptions
- description: Read workout detail samples and post comments.
  flows:
  - authorizationCode
  scope: workouts:details
- description: Create, update, and delete planned workouts.
  flows:
  - authorizationCode
  scope: workouts:plan
- description: Read planned and completed workouts and analytics.
  flows:
  - authorizationCode
  scope: workouts:read
- description: Read Workout of the Day and structured workout files.
  flows:
  - authorizationCode
  scope: workouts:wod
slug: trainingpeaks-scopes
source_filename: trainingpeaks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trainingpeaks-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/trainingpeaks-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.trainingpeaks.com/OAuth/Authorize\n    tokenUrl: https://oauth.trainingpeaks.com/oauth/token\n  description: OAuth 2.0 authorization code flow. Tokens are short-lived (expires_in seconds)\n    and refreshed with the refresh_token grant. Scopes are not inclusive (e.g. workouts:details\n    does not include workouts:read) and are limited to those granted to your application.\nscopes:\n- scope: athlete:profile\n  description: Read the authenticated athlete's profile and zones.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: coach:athletes\n  description: Read coach profile, athletes, and assistants.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: events:read\n\
  \  description: Read athlete events.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: events:write\n  description: Create athlete events.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: file:write\n  description: Upload activity files.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: metrics:read\n  description: Read athlete metrics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: metrics:write\n  description: Create athlete metrics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: nutrition:read\n  description: Read athlete nutrition entries.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: nutrition:write\n  description: Create, update, and delete nutrition entries.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n\
  - scope: routes:read\n  description: Read athlete routes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: routes:write\n  description: Create athlete routes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: webhook:read-subscriptions\n  description: List webhook subscriptions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: webhook:write-subscriptions\n  description: Create, update, and delete webhook subscriptions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: workouts:details\n  description: Read workout detail samples and post comments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: workouts:plan\n  description: Create, update, and delete planned workouts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: workouts:read\n\
  \  description: Read planned and completed workouts and analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n- scope: workouts:wod\n  description: Read Workout of the Day and structured workout files.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trainingpeaks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trainingpeaks/refs/heads/main/scopes/trainingpeaks-scopes.yml
summary_line: 17 scopes · authorizationCode
tags:
- Fitness
- Endurance Training
- Workouts
- Coaching
- Sports
- Health
- Wearables
token_urls:
- https://oauth.trainingpeaks.com/oauth/token
---
