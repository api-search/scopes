---
api_specs:
- filename: wakatime-api-v1-openapi.yml
  format: yaml
  label: WakaTime API v1
  slug: wakatime-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-api-v1-openapi.yml
authorization_urls:
- https://wakatime.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Wakatime Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'WakaTime publishes 8 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the WakaTime API on a user''s behalf.


  Tokens are issued from https://wakatime.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: WakaTime
provider_slug: wakatime
schemes:
- description: OAuth 2.0 authorization code flow.
  flows:
  - authorizationUrl: https://wakatime.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://wakatime.com/oauth/token
  - authorizationUrl: https://wakatime.com/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/wakatime-api-v1-openapi.yml
scope_count: 8
scope_names:
- email
- read_goals
- read_heartbeats
- read_orgs
- read_stats
- read_summaries
- write_heartbeats
- write_orgs
scopes:
- description: Read user email.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Read coding goals.
  flows:
  - authorizationCode
  - implicit
  scope: read_goals
- description: Read raw heartbeats.
  flows:
  - authorizationCode
  - implicit
  scope: read_heartbeats
- description: Read organization data.
  flows:
  - authorizationCode
  - implicit
  scope: read_orgs
- description: Read aggregate stats.
  flows:
  - authorizationCode
  - implicit
  scope: read_stats
- description: Read coding-activity summaries.
  flows:
  - authorizationCode
  - implicit
  scope: read_summaries
- description: Send heartbeats.
  flows:
  - authorizationCode
  - implicit
  scope: write_heartbeats
- description: Modify organization data.
  flows:
  - authorizationCode
  - implicit
  scope: write_orgs
slug: wakatime-scopes
source_filename: wakatime-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wakatime-api-v1-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/wakatime-api-v1-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wakatime.com/oauth/authorize\n    tokenUrl: https://wakatime.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://wakatime.com/oauth/authorize\n  description: OAuth 2.0 authorization code flow.\nscopes:\n- scope: email\n  description: Read user email.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n- scope: read_goals\n  description: Read coding goals.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n- scope: read_heartbeats\n  description: Read raw heartbeats.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n- scope: read_orgs\n  description: Read organization data.\n  flows:\n  -\
  \ authorizationCode\n  - implicit\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n- scope: read_stats\n  description: Read aggregate stats.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n- scope: read_summaries\n  description: Read coding-activity summaries.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n- scope: write_heartbeats\n  description: Send heartbeats.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n- scope: write_orgs\n  description: Modify organization data.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/scopes/wakatime-scopes.yml
summary_line: 8 scopes · authorizationCode/implicit
tags:
- Developer Productivity
- Developer Tools
- Time Tracking
- Coding Analytics
- Leaderboards
- IDE Plugins
- Open Source
- Public APIs
token_urls:
- https://wakatime.com/oauth/token
---
