---
api_specs:
- filename: workstream-public-api-openapi-original.json
  format: json
  label: Workstream Public API
  slug: workstream-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-public-api-openapi-original.json
authorization_urls:
- https://public-api.workstream.us/
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Workstream Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workstream publishes 10 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workstream API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workstream
provider_slug: workstream
schemes:
- flows:
  - authorizationUrl: https://public-api.workstream.us/
    flow: implicit
  name: oauth2
  source: openapi/workstream-public-api-openapi-original.json
scope_count: 10
scope_names:
- Applicants
- Company Roles
- Company Users
- Custom Field
- Departments
- Employees
- Imported Employee Infos
- Locations
- Positions
- TeamMember
scopes:
- description: Read Applicant records
  flows:
  - implicit
  scope: Applicants
- description: Read Company Role records
  flows:
  - implicit
  scope: Company Roles
- description: Read Company User records
  flows:
  - implicit
  scope: Company Users
- description: Read, update custom field and custom field values
  flows:
  - implicit
  scope: Custom Field
- description: Read Department records
  flows:
  - implicit
  scope: Departments
- description: Read Employee records
  flows:
  - implicit
  scope: Employees
- description: Read Imported Employee Info records
  flows:
  - implicit
  scope: Imported Employee Infos
- description: Read Location records
  flows:
  - implicit
  scope: Locations
- description: Read Position records
  flows:
  - implicit
  scope: Positions
- description: Read Team Member records
  flows:
  - implicit
  scope: TeamMember
slug: workstream-scopes
source_filename: workstream-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/workstream-public-api-openapi-original.json\nschemes:\n- name: oauth2\n  source: openapi/workstream-public-api-openapi-original.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://public-api.workstream.us/\nscopes:\n- scope: Applicants\n  description: Read Applicant records\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- scope: Company Roles\n  description: Read Company Role records\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- scope: Company Users\n  description: Read Company User records\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- scope: Custom Field\n  description: Read, update custom field and custom field values\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- scope: Departments\n  description: Read Department\
  \ records\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- scope: Employees\n  description: Read Employee records\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- scope: Imported Employee Infos\n  description: Read Imported Employee Info records\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- scope: Locations\n  description: Read Location records\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- scope: Positions\n  description: Read Position records\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n- scope: TeamMember\n  description: Read Team Member records\n  flows:\n  - implicit\n  sources:\n  - openapi/workstream-public-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/scopes/workstream-scopes.yml
summary_line: 10 scopes · implicit
tags:
- Company
- Hr Tech
- Hiring
- Payroll
- Onboarding
- Applicant Tracking
- Hourly Workforce
- Restaurants
token_urls: []
---
