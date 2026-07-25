---
api_specs:
- filename: 7shifts-availability-api-openapi.yml
  format: yaml
  label: 7shifts Availability API
  slug: 7shifts-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-availability-api-openapi.yml
- filename: 7shifts-companies-api-openapi.yml
  format: yaml
  label: 7shifts Companies API
  slug: 7shifts-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-companies-api-openapi.yml
- filename: 7shifts-departments-api-openapi.yml
  format: yaml
  label: 7shifts Departments API
  slug: 7shifts-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-departments-api-openapi.yml
- filename: 7shifts-identity-api-openapi.yml
  format: yaml
  label: 7shifts Identity API
  slug: 7shifts-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-identity-api-openapi.yml
- filename: 7shifts-locations-api-openapi.yml
  format: yaml
  label: 7shifts Locations API
  slug: 7shifts-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-locations-api-openapi.yml
- filename: 7shifts-oauth-api-openapi.yml
  format: yaml
  label: 7shifts OAuth API
  slug: 7shifts-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-oauth-api-openapi.yml
- filename: 7shifts-reporting-api-openapi.yml
  format: yaml
  label: 7shifts Reporting API
  slug: 7shifts-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-reporting-api-openapi.yml
- filename: 7shifts-roles-api-openapi.yml
  format: yaml
  label: 7shifts Roles API
  slug: 7shifts-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-roles-api-openapi.yml
- filename: 7shifts-sales-api-openapi.yml
  format: yaml
  label: 7shifts Sales API
  slug: 7shifts-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-sales-api-openapi.yml
- filename: 7shifts-shifts-api-openapi.yml
  format: yaml
  label: 7shifts Shifts API
  slug: 7shifts-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-shifts-api-openapi.yml
- filename: 7shifts-time-off-api-openapi.yml
  format: yaml
  label: 7shifts Time Off API
  slug: 7shifts-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-time-off-api-openapi.yml
- filename: 7shifts-time-punches-api-openapi.yml
  format: yaml
  label: 7shifts Time Punches API
  slug: 7shifts-time-punches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-time-punches-api-openapi.yml
- filename: 7shifts-users-api-openapi.yml
  format: yaml
  label: 7shifts Users API
  slug: 7shifts-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-users-api-openapi.yml
- filename: 7shifts-wages-api-openapi.yml
  format: yaml
  label: 7shifts Wages API
  slug: 7shifts-wages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-wages-api-openapi.yml
- filename: 7shifts-webhooks-api-openapi.yml
  format: yaml
  label: 7shifts Webhooks API
  slug: 7shifts-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.7shifts.com/docs/oauth-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: 7Shifts Scopes
name_suffix: OAuth Scopes
note: ''
overview: '7shifts publishes 18 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 7shifts API on a user''s behalf.


  Tokens are issued from https://api.7shifts.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 7shifts
provider_slug: 7shifts
schemes:
- description: OAuth 2.0 with client_credentials, password, authorization_code, and refresh_token grant types.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.7shifts.com/oauth2/token
  name: oauth2
  source: openapi/7shifts-openapi.yml
scope_count: 18
scope_names:
- companies:read
- companies:write
- departments:read
- departments:write
- locations:read
- locations:write
- roles:read
- roles:write
- users:read
- users:write
- sales:read
- sales:write
- shifts:read
- shifts:write
- time_punches:read
- time_punches:write
- events:read
- events:write
scopes:
- description: Reading or mutating company object.
  flows: []
  scope: companies:read
- description: Reading or mutating company object.
  flows: []
  scope: companies:write
- description: Reading or mutating departments.
  flows: []
  scope: departments:read
- description: Reading or mutating departments.
  flows: []
  scope: departments:write
- description: Reading or mutating locations.
  flows: []
  scope: locations:read
- description: Reading or mutating locations.
  flows: []
  scope: locations:write
- description: Reading or mutating roles.
  flows: []
  scope: roles:read
- description: Reading or mutating roles.
  flows: []
  scope: roles:write
- description: Reading or mutating users.
  flows: []
  scope: users:read
- description: Reading or mutating users.
  flows: []
  scope: users:write
- description: Reading or mutating sales.
  flows: []
  scope: sales:read
- description: Reading or mutating sales.
  flows: []
  scope: sales:write
- description: Reading or mutating shifts and schedule publishing.
  flows: []
  scope: shifts:read
- description: Reading or mutating shifts and schedule publishing.
  flows: []
  scope: shifts:write
- description: Reading or mutating time punches.
  flows: []
  scope: time_punches:read
- description: Reading or mutating time punches.
  flows: []
  scope: time_punches:write
- description: Reading or mutating schedule events.
  flows: []
  scope: events:read
- description: Reading or mutating schedule events.
  flows: []
  scope: events:write
slug: 7shifts-scopes
source_filename: 7shifts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/7shifts-openapi.yml\ndocs: https://developers.7shifts.com/docs/oauth-authentication\nschemes:\n- name: oauth2\n  source: openapi/7shifts-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.7shifts.com/oauth2/token\n  description: OAuth 2.0 with client_credentials, password, authorization_code, and refresh_token\n    grant types.\nscopes:\n- scope: companies:read\n  description: Reading or mutating company object.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: companies:write\n  description: Reading or mutating company object.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: departments:read\n  description: Reading or mutating departments.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: departments:write\n  description: Reading or mutating departments.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n\
  - scope: locations:read\n  description: Reading or mutating locations.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: locations:write\n  description: Reading or mutating locations.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: roles:read\n  description: Reading or mutating roles.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: roles:write\n  description: Reading or mutating roles.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: users:read\n  description: Reading or mutating users.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: users:write\n  description: Reading or mutating users.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: sales:read\n  description: Reading or mutating sales.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: sales:write\n\
  \  description: Reading or mutating sales.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: shifts:read\n  description: Reading or mutating shifts and schedule publishing.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: shifts:write\n  description: Reading or mutating shifts and schedule publishing.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: time_punches:read\n  description: Reading or mutating time punches.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: time_punches:write\n  description: Reading or mutating time punches.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: events:read\n  description: Reading or mutating schedule events.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n- scope: events:write\n  description: Reading or mutating schedule events.\n  sources:\n  - https://developers.7shifts.com/docs/oauth-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/scopes/7shifts-scopes.yml
summary_line: 18 scopes · clientCredentials
tags:
- Restaurant
- Scheduling
- Workforce Management
- Employee Scheduling
- Time Tracking
- HRIS
- Labor
token_urls:
- https://api.7shifts.com/oauth2/token
---
