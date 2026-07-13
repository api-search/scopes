---
api_specs:
- filename: zoho-people-openapi.yml
  format: yaml
  label: Zoho People REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/openapi/zoho-people-openapi.yml
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zoho People Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoho People publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoho People API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoho People
provider_slug: zoho-people
schemes:
- description: 'Zoho Accounts OAuth 2.0 — Authorization Code grant. Access tokens

    live for 1 hour; refresh tokens are long-lived until revoked.

    Scope syntax is `ZOHOPEOPLE.<scope>.<operation>` where scope is

    one of employee, forms, dashboard, automation, timetracker,

    attendance, leave; operation is ALL, READ, CREATE, UPDATE, or

    DELETE.'
  flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: ZohoOAuth2
  source: openapi/zoho-people-openapi.yml
scope_count: 13
scope_names:
- ZohoPeople.attendance.ALL
- ZohoPeople.automation.ALL
- ZohoPeople.dashboard.ALL
- ZohoPeople.employee.ALL
- ZohoPeople.forms.ALL
- ZohoPeople.forms.CREATE
- ZohoPeople.forms.READ
- ZohoPeople.forms.UPDATE
- ZohoPeople.leave.ALL
- ZohoPeople.leave.CREATE
- ZohoPeople.leave.READ
- ZohoPeople.leave.UPDATE
- ZohoPeople.timetracker.ALL
scopes:
- description: Full access to attendance operations
  flows:
  - authorizationCode
  scope: ZohoPeople.attendance.ALL
- description: Full access to automation / workflows
  flows:
  - authorizationCode
  scope: ZohoPeople.automation.ALL
- description: Full access to dashboard reads
  flows:
  - authorizationCode
  scope: ZohoPeople.dashboard.ALL
- description: Full access to employee records
  flows:
  - authorizationCode
  scope: ZohoPeople.employee.ALL
- description: Full access to form records
  flows:
  - authorizationCode
  scope: ZohoPeople.forms.ALL
- description: Create form records
  flows:
  - authorizationCode
  scope: ZohoPeople.forms.CREATE
- description: Read form records
  flows:
  - authorizationCode
  scope: ZohoPeople.forms.READ
- description: Update form records
  flows:
  - authorizationCode
  scope: ZohoPeople.forms.UPDATE
- description: Full access to leave operations
  flows:
  - authorizationCode
  scope: ZohoPeople.leave.ALL
- description: Submit leave requests
  flows:
  - authorizationCode
  scope: ZohoPeople.leave.CREATE
- description: Read leave records
  flows:
  - authorizationCode
  scope: ZohoPeople.leave.READ
- description: Update leave requests
  flows:
  - authorizationCode
  scope: ZohoPeople.leave.UPDATE
- description: Full access to time-tracker operations
  flows:
  - authorizationCode
  scope: ZohoPeople.timetracker.ALL
slug: zoho-people-scopes
source_filename: zoho-people-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zoho-people-openapi.yml\nschemes:\n- name: ZohoOAuth2\n  source: openapi/zoho-people-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n  description: |-\n    Zoho Accounts OAuth 2.0 — Authorization Code grant. Access tokens\n    live for 1 hour; refresh tokens are long-lived until revoked.\n    Scope syntax is `ZOHOPEOPLE.<scope>.<operation>` where scope is\n    one of employee, forms, dashboard, automation, timetracker,\n    attendance, leave; operation is ALL, READ, CREATE, UPDATE, or\n    DELETE.\nscopes:\n- scope: ZohoPeople.attendance.ALL\n  description: Full access to attendance operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.automation.ALL\n  description: Full access to automation / workflows\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.dashboard.ALL\n  description: Full access to dashboard reads\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.employee.ALL\n  description: Full access to employee records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.forms.ALL\n  description: Full access to form records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.forms.CREATE\n  description: Create form records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.forms.READ\n  description: Read form records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.forms.UPDATE\n  description: Update form records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.leave.ALL\n\
  \  description: Full access to leave operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.leave.CREATE\n  description: Submit leave requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.leave.READ\n  description: Read leave records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.leave.UPDATE\n  description: Update leave requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n- scope: ZohoPeople.timetracker.ALL\n  description: Full access to time-tracker operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-people-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/scopes/zoho-people-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- HR
- HRMS
- Human Resources
- HRIS
- Employee Management
- Attendance
- Leave Management
- Time Tracking
- Performance Management
- Onboarding
- Zoho
- OAuth 2.0
token_urls:
- https://accounts.zoho.com/oauth/v2/token
---
