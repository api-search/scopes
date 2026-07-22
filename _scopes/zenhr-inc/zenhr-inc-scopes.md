---
api_specs:
- filename: zenhr-inc-openapi.yml
  format: yaml
  label: ZenHR API
  slug: zenhr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenhr-inc/refs/heads/main/openapi/zenhr-inc-openapi.yml
authorization_urls:
- https://api.zenhr.com/en/oauth/authorize
description: ''
docs: https://api-docs.zenhr.com/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Zenhr Inc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ZenHR Inc publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ZenHR Inc API on a user''s behalf.


  Tokens are issued from https://api.zenhr.com/en/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ZenHR Inc
provider_slug: zenhr-inc
schemes:
- flows:
  - authorizationUrl: https://api.zenhr.com/en/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.zenhr.com/en/oauth/token
  name: oauth2
  source: https://api.zenhr.com/.well-known/oauth-authorization-server
scope_count: 9
scope_names:
- read:branch
- read:employee
- accessed_employees_branches:employee
- read:professional_info
- read:termination
- read:employee_disciplinary_actions
- read:financial_transaction
- read:performance_evaluation
- read:timeoff_transaction
scopes:
- description: Read branch data
  flows:
  - authorizationCode
  scope: read:branch
- description: Read employee data
  flows:
  - authorizationCode
  scope: read:employee
- description: Access employees within the branches permitted to the app
  flows:
  - authorizationCode
  scope: accessed_employees_branches:employee
- description: Read employee professional information
  flows:
  - authorizationCode
  scope: read:professional_info
- description: Read termination data
  flows:
  - authorizationCode
  scope: read:termination
- description: Read employee disciplinary actions
  flows:
  - authorizationCode
  scope: read:employee_disciplinary_actions
- description: Read financial transactions
  flows:
  - authorizationCode
  scope: read:financial_transaction
- description: Read performance evaluations
  flows:
  - authorizationCode
  scope: read:performance_evaluation
- description: Read time-off transactions
  flows:
  - authorizationCode
  scope: read:timeoff_transaction
slug: zenhr-inc-scopes
source_filename: zenhr-inc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# API Evangelist enrichment artifact\ngenerated: '2026-07-21'\nmethod: searched\nsource: https://api.zenhr.com/.well-known/oauth-authorization-server\ndocs: https://api-docs.zenhr.com/\nnotes: Scopes are selected per integration app when registered at /en/oauth/applications. List is authoritative from the published\n  RFC 8414 authorization-server metadata (scopes_supported).\nschemes:\n- name: oauth2\n  source: https://api.zenhr.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.zenhr.com/en/oauth/authorize\n    tokenUrl: https://api.zenhr.com/en/oauth/token\nscopes:\n- scope: read:branch\n  description: Read branch data\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.zenhr.com/.well-known/oauth-authorization-server\n- scope: read:employee\n  description: Read employee data\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.zenhr.com/.well-known/oauth-authorization-server\n- scope: accessed_employees_branches:employee\n\
  \  description: Access employees within the branches permitted to the app\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.zenhr.com/.well-known/oauth-authorization-server\n- scope: read:professional_info\n  description: Read employee professional information\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.zenhr.com/.well-known/oauth-authorization-server\n- scope: read:termination\n  description: Read termination data\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.zenhr.com/.well-known/oauth-authorization-server\n- scope: read:employee_disciplinary_actions\n  description: Read employee disciplinary actions\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.zenhr.com/.well-known/oauth-authorization-server\n- scope: read:financial_transaction\n  description: Read financial transactions\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.zenhr.com/.well-known/oauth-authorization-server\n- scope: read:performance_evaluation\n \
  \ description: Read performance evaluations\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.zenhr.com/.well-known/oauth-authorization-server\n- scope: read:timeoff_transaction\n  description: Read time-off transactions\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.zenhr.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenhr-inc/refs/heads/main/scopes/zenhr-inc-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Company
- Human Resources
- HR
- Payroll
- HRMS
- Employee Management
- MENA
- Attendance
- Time Off
- SaaS
token_urls:
- https://api.zenhr.com/en/oauth/token
---
