---
api_specs:
- filename: hoursquare-attendance-api-openapi.yml
  format: yaml
  label: HourSquare Attendance API
  slug: hoursquare-attendance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-attendance-api-openapi.yml
- filename: hoursquare-employees-api-openapi.yml
  format: yaml
  label: HourSquare Employees API
  slug: hoursquare-employees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-employees-api-openapi.yml
- filename: hoursquare-me-api-openapi.yml
  format: yaml
  label: HourSquare Me API
  slug: hoursquare-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-me-api-openapi.yml
- filename: hoursquare-oauth-api-openapi.yml
  format: yaml
  label: HourSquare OAuth API
  slug: hoursquare-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-oauth-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Hoursquare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HourSquare publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HourSquare API on a user''s behalf.


  Tokens are issued from https://api.hoursquare.com/api/public/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HourSquare
provider_slug: hoursquare
schemes:
- description: 'Client credentials (RFC 6749 §4.4): POST your API key as `client_secret` (or as the HTTP Basic password) to the token URL and use the returned token as a Bearer. Tokens live 15 minutes. Each operation lists the scope it requires; a key carries the scopes it was created with.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.hoursquare.com/api/public/v1/oauth/token
  name: OAuth2
  source: openapi/hoursquare-openapi.json
scope_count: 5
scope_names:
- attendance.read
- attendance.record
- attendance.reports
- employees.read
- leave.read
scopes:
- description: Read time entries (permission 47)
  flows:
  - clientCredentials
  scope: attendance.read
- description: Record clock events and completed shifts; set employee external ids (permission 86)
  flows:
  - clientCredentials
  scope: attendance.record
- description: Read time reports (permission 49)
  flows:
  - clientCredentials
  scope: attendance.reports
- description: Read employees (id, external id, name, email, status) (permission 52)
  flows:
  - clientCredentials
  scope: employees.read
- description: Read leave balances and requests (permission 72)
  flows:
  - clientCredentials
  scope: leave.read
slug: hoursquare-scopes
source_filename: hoursquare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/hoursquare-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/hoursquare-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.hoursquare.com/api/public/v1/oauth/token\n  description: 'Client credentials (RFC 6749 §4.4): POST your API key as `client_secret` (or\n    as the HTTP Basic password) to the token URL and use the returned token as a Bearer. Tokens\n    live 15 minutes. Each operation lists the scope it requires; a key carries the scopes it\n    was created with.'\nscopes:\n- scope: attendance.read\n  description: Read time entries (permission 47)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hoursquare-openapi.json\n- scope: attendance.record\n  description: Record clock events and completed shifts; set employee external ids (permission\n    86)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hoursquare-openapi.json\n- scope: attendance.reports\n  description:\
  \ Read time reports (permission 49)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hoursquare-openapi.json\n- scope: employees.read\n  description: Read employees (id, external id, name, email, status) (permission 52)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hoursquare-openapi.json\n- scope: leave.read\n  description: Read leave balances and requests (permission 72)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hoursquare-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hoursquare/scopes/hoursquare-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Human Resources
- Payroll
- Time Tracking
- Workforce Management
- Software-as-a-Service
token_bound: false
token_urls:
- https://api.hoursquare.com/api/public/v1/oauth/token
---
