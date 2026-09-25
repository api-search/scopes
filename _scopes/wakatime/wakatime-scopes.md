---
api_specs:
- filename: wakatime-commits-api-openapi.yml
  format: yaml
  label: WakaTime Commits API
  slug: wakatime-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-commits-api-openapi.yml
- filename: wakatime-custom-rules-api-openapi.yml
  format: yaml
  label: WakaTime Custom Rules API
  slug: wakatime-custom-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-custom-rules-api-openapi.yml
- filename: wakatime-data-dumps-api-openapi.yml
  format: yaml
  label: WakaTime Data Dumps API
  slug: wakatime-data-dumps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-data-dumps-api-openapi.yml
- filename: wakatime-durations-api-openapi.yml
  format: yaml
  label: WakaTime Durations API
  slug: wakatime-durations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-durations-api-openapi.yml
- filename: wakatime-editors-api-openapi.yml
  format: yaml
  label: WakaTime Editors API
  slug: wakatime-editors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-editors-api-openapi.yml
- filename: wakatime-external-durations-api-openapi.yml
  format: yaml
  label: WakaTime External Durations API
  slug: wakatime-external-durations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-external-durations-api-openapi.yml
- filename: wakatime-goals-api-openapi.yml
  format: yaml
  label: WakaTime Goals API
  slug: wakatime-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-goals-api-openapi.yml
- filename: wakatime-heartbeats-api-openapi.yml
  format: yaml
  label: WakaTime Heartbeats API
  slug: wakatime-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-heartbeats-api-openapi.yml
- filename: wakatime-insights-api-openapi.yml
  format: yaml
  label: WakaTime Insights API
  slug: wakatime-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-insights-api-openapi.yml
- filename: wakatime-languages-api-openapi.yml
  format: yaml
  label: WakaTime Languages API
  slug: wakatime-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-languages-api-openapi.yml
- filename: wakatime-leaderboards-api-openapi.yml
  format: yaml
  label: WakaTime Leaderboards API
  slug: wakatime-leaderboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-leaderboards-api-openapi.yml
- filename: wakatime-machines-api-openapi.yml
  format: yaml
  label: WakaTime Machines API
  slug: wakatime-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-machines-api-openapi.yml
- filename: wakatime-meta-api-openapi.yml
  format: yaml
  label: WakaTime Meta API
  slug: wakatime-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-meta-api-openapi.yml
- filename: wakatime-organizations-api-openapi.yml
  format: yaml
  label: WakaTime Organizations API
  slug: wakatime-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-organizations-api-openapi.yml
- filename: wakatime-projects-api-openapi.yml
  format: yaml
  label: WakaTime Projects API
  slug: wakatime-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-projects-api-openapi.yml
- filename: wakatime-stats-api-openapi.yml
  format: yaml
  label: WakaTime Stats API
  slug: wakatime-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-stats-api-openapi.yml
- filename: wakatime-status-bar-api-openapi.yml
  format: yaml
  label: WakaTime Status Bar API
  slug: wakatime-status-bar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-status-bar-api-openapi.yml
- filename: wakatime-summaries-api-openapi.yml
  format: yaml
  label: WakaTime Summaries API
  slug: wakatime-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-summaries-api-openapi.yml
- filename: wakatime-user-agents-api-openapi.yml
  format: yaml
  label: WakaTime User Agents API
  slug: wakatime-user-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-user-agents-api-openapi.yml
- filename: wakatime-users-api-openapi.yml
  format: yaml
  label: WakaTime Users API
  slug: wakatime-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-users-api-openapi.yml
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
