---
api_specs:
- filename: onpay-company-api-openapi.yml
  format: yaml
  label: OnPay Company API
  slug: onpay-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-company-api-openapi.yml
- filename: onpay-deductions-api-openapi.yml
  format: yaml
  label: OnPay Deductions API
  slug: onpay-deductions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-deductions-api-openapi.yml
- filename: onpay-employees-api-openapi.yml
  format: yaml
  label: OnPay Employees API
  slug: onpay-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-employees-api-openapi.yml
- filename: onpay-pay-runs-api-openapi.yml
  format: yaml
  label: OnPay Pay Runs API
  slug: onpay-pay-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-pay-runs-api-openapi.yml
- filename: onpay-reports-api-openapi.yml
  format: yaml
  label: OnPay Reports API
  slug: onpay-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-reports-api-openapi.yml
- filename: onpay-user-api-openapi.yml
  format: yaml
  label: OnPay User API
  slug: onpay-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/openapi/onpay-user-api-openapi.yml
authorization_urls:
- https://app.onpay.com/app/oauth/authorize
description: ''
docs: https://onpay.readme.io/reference/authorization
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Onpay Scopes
name_suffix: OAuth Scopes
note: 'OnPay''s OAuth 2.0 "scopes" are not permission strings — they are the platform''s six USER ROLES, and the description on each in the OpenAPI is the numeric `access_type` code that the token response returns (Owner=1, Approver=2, Controller=3, Manager=4, Accountant=5, Employee=6). There is no read/write split, no resource-scoped grant, and no published scopes reference page: a partner receives whatever the authorizing user''s role allows. The operation counts below are derived from the per-operation security[] requirements across all 58 operations.'
overview: 'OnPay publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the OnPay API on a user''s behalf.


  Tokens are issued from https://app.onpay.com/app/oauth/authorize.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OnPay
provider_slug: onpay
schemes:
- flows:
  - authorizationUrl: https://app.onpay.com/app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.onpay.com/app/oauth/authorize
    tokenUrl_documented: https://app.onpay.com/app/oauth/token
  name: OAuth2
  source: openapi/onpay-api-openapi.json
scope_count: 6
scope_names:
- Owner
- Approver
- Controller
- Manager
- Accountant
- Employee
scopes:
- description: OnPay company owner. Accepted on all 58 operations.
  flows:
  - authorizationCode
  scope: Owner
- description: Payroll approver. Accepted on all 58 operations, same reach as Owner in this spec.
  flows:
  - authorizationCode
  scope: Approver
- description: Restricted role. Accepted on 8 operations only — employee deduction reads, recent notes, termination and rehire, worksite reads, and pay-schedule dates.
  flows:
  - authorizationCode
  scope: Controller
- description: Restricted role. Accepted on the same 8 operations as Controller.
  flows:
  - authorizationCode
  scope: Manager
- description: Declared in the securityScheme but required by ZERO operations in the published spec — an accountant-scoped token authorizes nothing the document describes.
  flows:
  - authorizationCode
  scope: Accountant
- description: Self-service role. Accepted on 2 operations only — GET /employees/{employee_id}/deductions and GET /user.
  flows:
  - authorizationCode
  scope: Employee
slug: onpay-scopes
source_filename: onpay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/onpay-api-openapi.json\ndocs: https://onpay.readme.io/reference/authorization\nmodel: role-based\nnote: >-\n  OnPay's OAuth 2.0 \"scopes\" are not permission strings — they are the platform's six USER ROLES, and\n  the description on each in the OpenAPI is the numeric `access_type` code that the token response\n  returns (Owner=1, Approver=2, Controller=3, Manager=4, Accountant=5, Employee=6). There is no\n  read/write split, no resource-scoped grant, and no published scopes reference page: a partner\n  receives whatever the authorizing user's role allows. The operation counts below are derived from\n  the per-operation security[] requirements across all 58 operations.\nschemes:\n- name: OAuth2\n  source: openapi/onpay-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.onpay.com/app/oauth/authorize\n    tokenUrl: https://app.onpay.com/app/oauth/authorize\n    tokenUrl_documented:\
  \ https://app.onpay.com/app/oauth/token\nscopes:\n- scope: Owner\n  access_type: 1\n  description: OnPay company owner. Accepted on all 58 operations.\n  operations: 58\n  flows: [authorizationCode]\n  sources: [openapi/onpay-api-openapi.json]\n- scope: Approver\n  access_type: 2\n  description: Payroll approver. Accepted on all 58 operations, same reach as Owner in this spec.\n  operations: 58\n  flows: [authorizationCode]\n  sources: [openapi/onpay-api-openapi.json]\n- scope: Controller\n  access_type: 3\n  description: >-\n    Restricted role. Accepted on 8 operations only — employee deduction reads, recent notes,\n    termination and rehire, worksite reads, and pay-schedule dates.\n  operations: 8\n  flows: [authorizationCode]\n  sources: [openapi/onpay-api-openapi.json]\n- scope: Manager\n  access_type: 4\n  description: Restricted role. Accepted on the same 8 operations as Controller.\n  operations: 8\n  flows: [authorizationCode]\n  sources: [openapi/onpay-api-openapi.json]\n- scope:\
  \ Accountant\n  access_type: 5\n  description: >-\n    Declared in the securityScheme but required by ZERO operations in the published spec — an\n    accountant-scoped token authorizes nothing the document describes.\n  operations: 0\n  flows: [authorizationCode]\n  sources: [openapi/onpay-api-openapi.json]\n- scope: Employee\n  access_type: 6\n  description: >-\n    Self-service role. Accepted on 2 operations only — GET /employees/{employee_id}/deductions and\n    GET /user.\n  operations: 2\n  flows: [authorizationCode]\n  sources: [openapi/onpay-api-openapi.json]\ngaps:\n- No scopes/permissions reference page exists in the docs; the ReadMe hub's llms.txt lists every page\n  it has and there is no permissions article.\n- Roles are coarse — Owner and Approver both unlock every write in the API, including\n  POST /employees/{employee_id}/termination and PUT /employees/{employee_id}/bank-accounts. There is\n  no read-only grant an integration can request.\n- The Accountant role is declared\
  \ but unused, so its meaning cannot be verified from the contract.\nx-evidence:\n- url: https://onpay.readme.io/reference/authorization.md\n  http_status: 200\n  fetched: '2026-08-04'\n- url: https://onpay.readme.io/llms.txt\n  http_status: 200\n  fetched: '2026-08-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onpay/refs/heads/main/scopes/onpay-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- payroll
- human-resources
- employee-benefits
- payroll-tax
- small-business
- workforce-management
- fintech
- hr-tech
- time-and-attendance
- retirement-401k
token_urls:
- https://app.onpay.com/app/oauth/authorize
---
