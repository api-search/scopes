---
authorization_urls:
- https://www.strava.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Strava Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Strava publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Strava API on a user''s behalf.


  Tokens are issued from https://www.strava.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Strava
provider_slug: strava
schemes:
- description: OAuth 2.0 Bearer token. Obtain via the authorization code flow at https://www.strava.com/oauth/authorize.
  flows:
  - authorizationUrl: https://www.strava.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.strava.com/oauth/token
  name: stravaBearerAuth
  source: openapi/strava-openapi.yml
scope_count: 7
scope_names:
- activity:read
- activity:read_all
- activity:write
- profile:read_all
- profile:write
- read
- read_all
scopes:
- description: Read the user's activity data for activities that are visible to Everyone and Followers
  flows:
  - authorizationCode
  scope: activity:read
- description: Same access as activity:read with the addition of activities with visibility set to Only You
  flows:
  - authorizationCode
  scope: activity:read_all
- description: Access to create manual activities and uploads, and access to edit any activities that are visible to the app
  flows:
  - authorizationCode
  scope: activity:write
- description: Read all profile information even if the user has set their profile visibility to Followers or Only You
  flows:
  - authorizationCode
  scope: profile:read_all
- description: Update the user's weight and Functional Threshold Power (FTP), and access to star or unstar segments on their behalf
  flows:
  - authorizationCode
  scope: profile:write
- description: Read public segments, public routes, public profile data, public posts, public events, club feeds, and leaderboards
  flows:
  - authorizationCode
  scope: read
- description: Read private routes, private segments, and private events for the user
  flows:
  - authorizationCode
  scope: read_all
slug: strava-scopes
source_filename: strava-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/strava-openapi.yml\nschemes:\n- name: stravaBearerAuth\n  source: openapi/strava-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.strava.com/oauth/authorize\n    tokenUrl: https://www.strava.com/oauth/token\n  description: OAuth 2.0 Bearer token. Obtain via the authorization code flow at https://www.strava.com/oauth/authorize.\nscopes:\n- scope: activity:read\n  description: Read the user's activity data for activities that are visible to Everyone and\n    Followers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/strava-openapi.yml\n- scope: activity:read_all\n  description: Same access as activity:read with the addition of activities with visibility\n    set to Only You\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/strava-openapi.yml\n- scope: activity:write\n  description: Access to create manual activities and uploads, and access to edit any activities\n \
  \   that are visible to the app\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/strava-openapi.yml\n- scope: profile:read_all\n  description: Read all profile information even if the user has set their profile visibility\n    to Followers or Only You\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/strava-openapi.yml\n- scope: profile:write\n  description: Update the user's weight and Functional Threshold Power (FTP), and access to\n    star or unstar segments on their behalf\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/strava-openapi.yml\n- scope: read\n  description: Read public segments, public routes, public profile data, public posts, public\n    events, club feeds, and leaderboards\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/strava-openapi.yml\n- scope: read_all\n  description: Read private routes, private segments, and private events for the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/strava-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strava/refs/heads/main/scopes/strava-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Cycling
- Fitness
- Fitness Tracking
- Running
- Sports
token_urls:
- https://www.strava.com/oauth/token
---
