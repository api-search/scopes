---
api_specs:
- filename: quinyx-api-v3-openapi.yml
  format: yaml
  label: Quinyx API v3
  slug: quinyx-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/openapi/quinyx-api-v3-openapi.yml
- filename: quinyx-api-v2-openapi.yml
  format: yaml
  label: Quinyx API v2
  slug: quinyx-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/openapi/quinyx-api-v2-openapi.yml
- filename: quinyx-userapi-v2-openapi.yml
  format: yaml
  label: Quinyx User API v2
  slug: quinyx-user-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/openapi/quinyx-userapi-v2-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.quinyx.com/api/v3/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Quinyx Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Quinyx publishes 14 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Quinyx API on a user''s behalf.


  Tokens are issued from /oauth/v3/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Quinyx
provider_slug: quinyx
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/v3/token
  name: OAuth2ClientCredentials (v3)
  source: openapi/quinyx-api-v3-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/v3/token
  members:
  - employee_OAuth2ClientCredentials
  - opening-hours_OAuth2ClientCredentials
  - organisation_OAuth2ClientCredentials
  - rest-api-uaa_OAuth2ClientCredentials
  - schedule-availability_OAuth2ClientCredentials
  - schedule_OAuth2ClientCredentials
  - statistics_OAuth2ClientCredentials
  name: v2 per-service OAuth2ClientCredentials
  source: openapi/quinyx-api-v2-openapi.yml
scope_count: 14
scope_names:
- hr:employees:read
- hr:employees:create
- hr:employees:update
- hr:employees:delete
- hr:role-assignments:read
- hr:role-assignments:create
- hr:role-assignments:update
- hr:role-assignments:delete
- organization:groups:read
- organization:groups:create
- organization:groups:update
- organization:groups:delete
- organization:roles:read
- schedule:shifts:read
scopes:
- description: Read employee (HR) records.
  flows:
  - clientCredentials
  scope: hr:employees:read
- description: Create employee records.
  flows:
  - clientCredentials
  scope: hr:employees:create
- description: Update employee records.
  flows:
  - clientCredentials
  scope: hr:employees:update
- description: Delete employee records.
  flows:
  - clientCredentials
  scope: hr:employees:delete
- description: Read role assignments.
  flows:
  - clientCredentials
  scope: hr:role-assignments:read
- description: Create role assignments.
  flows:
  - clientCredentials
  scope: hr:role-assignments:create
- description: Update role assignments.
  flows:
  - clientCredentials
  scope: hr:role-assignments:update
- description: Delete role assignments.
  flows:
  - clientCredentials
  scope: hr:role-assignments:delete
- description: Read organizational groups/units.
  flows:
  - clientCredentials
  scope: organization:groups:read
- description: Create organizational groups/units.
  flows:
  - clientCredentials
  scope: organization:groups:create
- description: Update organizational groups/units.
  flows:
  - clientCredentials
  scope: organization:groups:update
- description: Delete organizational groups/units.
  flows:
  - clientCredentials
  scope: organization:groups:delete
- description: Read role definitions.
  flows:
  - clientCredentials
  scope: organization:roles:read
- description: Read schedule shifts.
  flows:
  - clientCredentials
  scope: schedule:shifts:read
slug: quinyx-scopes
source_filename: quinyx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/quinyx-api-v2-openapi.yml, openapi/quinyx-api-v3-openapi.yml\ndocs: https://developer.quinyx.com/api/v3/authentication\nnotes: >-\n  Scopes are requested at token time in the OAuth 2.0 client-credentials grant.\n  Quinyx uses a resource:object:action naming scheme (e.g. hr:employees:read).\n  The scopes below are aggregated verbatim from the v2 and v3 OpenAPI security\n  schemes; the seven v2 service schemes share the same /oauth/v3/token endpoint.\nschemes:\n- name: OAuth2ClientCredentials (v3)\n  source: openapi/quinyx-api-v3-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/v3/token\n- name: v2 per-service OAuth2ClientCredentials\n  source: openapi/quinyx-api-v2-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/v3/token\n  members:\n  - employee_OAuth2ClientCredentials\n  - opening-hours_OAuth2ClientCredentials\n  - organisation_OAuth2ClientCredentials\n  - rest-api-uaa_OAuth2ClientCredentials\n\
  \  - schedule-availability_OAuth2ClientCredentials\n  - schedule_OAuth2ClientCredentials\n  - statistics_OAuth2ClientCredentials\nscopes:\n- scope: hr:employees:read\n  description: Read employee (HR) records.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v2-openapi.yml, openapi/quinyx-api-v3-openapi.yml]\n- scope: hr:employees:create\n  description: Create employee records.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v2-openapi.yml, openapi/quinyx-api-v3-openapi.yml]\n- scope: hr:employees:update\n  description: Update employee records.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v2-openapi.yml, openapi/quinyx-api-v3-openapi.yml]\n- scope: hr:employees:delete\n  description: Delete employee records.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v2-openapi.yml, openapi/quinyx-api-v3-openapi.yml]\n- scope: hr:role-assignments:read\n  description: Read role assignments.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v3-openapi.yml]\n\
  - scope: hr:role-assignments:create\n  description: Create role assignments.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v3-openapi.yml]\n- scope: hr:role-assignments:update\n  description: Update role assignments.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v3-openapi.yml]\n- scope: hr:role-assignments:delete\n  description: Delete role assignments.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v3-openapi.yml]\n- scope: organization:groups:read\n  description: Read organizational groups/units.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v2-openapi.yml, openapi/quinyx-api-v3-openapi.yml]\n- scope: organization:groups:create\n  description: Create organizational groups/units.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v2-openapi.yml, openapi/quinyx-api-v3-openapi.yml]\n- scope: organization:groups:update\n  description: Update organizational groups/units.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v2-openapi.yml,\
  \ openapi/quinyx-api-v3-openapi.yml]\n- scope: organization:groups:delete\n  description: Delete organizational groups/units.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v2-openapi.yml, openapi/quinyx-api-v3-openapi.yml]\n- scope: organization:roles:read\n  description: Read role definitions.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v3-openapi.yml]\n- scope: schedule:shifts:read\n  description: Read schedule shifts.\n  flows: [clientCredentials]\n  sources: [openapi/quinyx-api-v3-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/scopes/quinyx-scopes.yml
summary_line: 14 scopes · clientCredentials
tags:
- Workforce Management
- Scheduling
- Human Resources
- Time Tracking
- Forecasting
- Employee Engagement
- Retail
- Hospitality
- Company
token_urls:
- /oauth/v3/token
---
