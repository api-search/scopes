---
api_specs:
- filename: blue-prism-calendars-api-openapi.yml
  format: yaml
  label: Blue Prism Calendars API
  slug: blue-prism-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-calendars-api-openapi.yml
- filename: blue-prism-dashboards-api-openapi.yml
  format: yaml
  label: Blue Prism Dashboards API
  slug: blue-prism-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-dashboards-api-openapi.yml
- filename: blue-prism-encryption-schemes-api-openapi.yml
  format: yaml
  label: Blue Prism Encryption Schemes API
  slug: blue-prism-encryption-schemes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-encryption-schemes-api-openapi.yml
- filename: blue-prism-environment-variables-api-openapi.yml
  format: yaml
  label: Blue Prism Environment Variables API
  slug: blue-prism-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-environment-variables-api-openapi.yml
- filename: blue-prism-health-api-openapi.yml
  format: yaml
  label: Blue Prism Health API
  slug: blue-prism-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-health-api-openapi.yml
- filename: blue-prism-licenses-api-openapi.yml
  format: yaml
  label: Blue Prism Licenses API
  slug: blue-prism-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-licenses-api-openapi.yml
- filename: blue-prism-pools-api-openapi.yml
  format: yaml
  label: Blue Prism Pools API
  slug: blue-prism-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-pools-api-openapi.yml
- filename: blue-prism-processes-api-openapi.yml
  format: yaml
  label: Blue Prism Processes API
  slug: blue-prism-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-processes-api-openapi.yml
- filename: blue-prism-resources-api-openapi.yml
  format: yaml
  label: Blue Prism Resources API
  slug: blue-prism-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-resources-api-openapi.yml
- filename: blue-prism-schedulelogs-api-openapi.yml
  format: yaml
  label: Blue Prism Schedule Logs API
  slug: blue-prism-schedulelogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-schedulelogs-api-openapi.yml
- filename: blue-prism-schedules-api-openapi.yml
  format: yaml
  label: Blue Prism Schedules API
  slug: blue-prism-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-schedules-api-openapi.yml
- filename: blue-prism-sessions-api-openapi.yml
  format: yaml
  label: Blue Prism Sessions API
  slug: blue-prism-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-sessions-api-openapi.yml
- filename: blue-prism-subscriptions-api-openapi.yml
  format: yaml
  label: Blue Prism Subscriptions API
  slug: blue-prism-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-subscriptions-api-openapi.yml
- filename: blue-prism-user-api-openapi.yml
  format: yaml
  label: Blue Prism User API
  slug: blue-prism-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-user-api-openapi.yml
- filename: blue-prism-work-queue-groups-api-openapi.yml
  format: yaml
  label: Blue Prism Work Queue Groups API
  slug: blue-prism-work-queue-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-work-queue-groups-api-openapi.yml
- filename: blue-prism-work-queues-api-openapi.yml
  format: yaml
  label: Blue Prism Work Queues API
  slug: blue-prism-work-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-work-queues-api-openapi.yml
- filename: blue-prism-timezones-api-openapi.yml
  format: yaml
  label: Blue Prism Timezones API
  slug: blue-prism-timezones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-timezones-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Blue Prism Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Blue Prism publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Blue Prism API on a user''s behalf.


  Tokens are issued from https://auth-server/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blue Prism
provider_slug: blue-prism
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth-server/connect/token
  name: OAuth2
  source: openapi/blue-prism-enterprise-api-openapi.yml
scope_count: 2
scope_names:
- bp-api
- bpserver
scopes:
- description: API scope
  flows:
  - clientCredentials
  scope: bp-api
- description: Blue Prism Application scope
  flows:
  - clientCredentials
  scope: bpserver
slug: blue-prism-scopes
source_filename: blue-prism-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/blue-prism-enterprise-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/blue-prism-enterprise-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-server/connect/token\nscopes:\n- scope: bp-api\n  description: API scope\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/blue-prism-enterprise-api-openapi.yml\n- scope: bpserver\n  description: Blue Prism Application scope\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/blue-prism-enterprise-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/scopes/blue-prism-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- AI Automation
- RPA
- Intelligent Automation
- Business Process Management
- Process Orchestration
- AI Agents
- Workflow Automation
- Enterprise Software
token_urls:
- https://auth-server/connect/token
---
