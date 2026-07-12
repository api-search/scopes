---
authorization_urls:
- https://api.wahooligan.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wahoo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wahoo Fitness publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wahoo Fitness API on a user''s behalf.


  Tokens are issued from https://api.wahooligan.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wahoo Fitness
provider_slug: wahoo
schemes:
- description: OAuth 2.0 Authorization Code (with PKCE option for public apps). Access tokens are bearer tokens with a 2-hour TTL; refresh tokens are single-use. Starting 2026-01-01, apps are limited to 10 unrevoked access tokens per user.
  flows:
  - authorizationUrl: https://api.wahooligan.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.wahooligan.com/oauth/token
  name: OAuth2
  source: openapi/wahoo-cloud-api-openapi.yml
scope_count: 12
scope_names:
- email
- offline_data
- plans_read
- plans_write
- power_zones_read
- power_zones_write
- routes_read
- routes_write
- user_read
- user_write
- workouts_read
- workouts_write
scopes:
- description: Access the user's email address
  flows:
  - authorizationCode
  scope: email
- description: Receive webhook events while the app is closed
  flows:
  - authorizationCode
  scope: offline_data
- description: Read workout plans
  flows:
  - authorizationCode
  scope: plans_read
- description: Manage workout plans
  flows:
  - authorizationCode
  scope: plans_write
- description: Read cycling power zones
  flows:
  - authorizationCode
  scope: power_zones_read
- description: Manage cycling power zones
  flows:
  - authorizationCode
  scope: power_zones_write
- description: Read GPS routes
  flows:
  - authorizationCode
  scope: routes_read
- description: Manage GPS routes
  flows:
  - authorizationCode
  scope: routes_write
- description: Read user profile
  flows:
  - authorizationCode
  scope: user_read
- description: Update user profile
  flows:
  - authorizationCode
  scope: user_write
- description: Read workouts and summaries
  flows:
  - authorizationCode
  scope: workouts_read
- description: Create/update/delete workouts and uploads
  flows:
  - authorizationCode
  scope: workouts_write
slug: wahoo-scopes
source_filename: wahoo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wahoo-cloud-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/wahoo-cloud-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.wahooligan.com/oauth/authorize\n    tokenUrl: https://api.wahooligan.com/oauth/token\n  description: OAuth 2.0 Authorization Code (with PKCE option for public apps). Access tokens\n    are bearer tokens with a 2-hour TTL; refresh tokens are single-use. Starting 2026-01-01,\n    apps are limited to 10 unrevoked access tokens per user.\nscopes:\n- scope: email\n  description: Access the user's email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: offline_data\n  description: Receive webhook events while the app is closed\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: plans_read\n  description: Read workout plans\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: plans_write\n  description: Manage workout plans\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: power_zones_read\n  description: Read cycling power zones\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: power_zones_write\n  description: Manage cycling power zones\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: routes_read\n  description: Read GPS routes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: routes_write\n  description: Manage GPS routes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: user_read\n  description: Read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: user_write\n  description: Update user profile\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: workouts_read\n  description: Read workouts and summaries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n- scope: workouts_write\n  description: Create/update/delete workouts and uploads\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/scopes/wahoo-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Fitness
- Cycling
- Endurance Training
- Bike Computers
- Smart Trainers
- Indoor Cycling
- Heart Rate
- Power Meters
- GPS
- Wearables
- Hardware
- FIT Files
- Webhooks
- OAuth
token_urls:
- https://api.wahooligan.com/oauth/token
---
