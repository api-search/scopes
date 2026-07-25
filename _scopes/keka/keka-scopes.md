---
api_specs:
- filename: keka-assets-api-openapi.yml
  format: yaml
  label: Keka HR Assets API
  slug: keka-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-assets-api-openapi.yml
- filename: keka-attendance-api-openapi.yml
  format: yaml
  label: Keka HR Attendance API
  slug: keka-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-attendance-api-openapi.yml
- filename: keka-authentication-api-openapi.yml
  format: yaml
  label: Keka HR Authentication API
  slug: keka-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-authentication-api-openapi.yml
- filename: keka-bgv-apis-api-openapi.yml
  format: yaml
  label: Keka HR BGV APIs API
  slug: keka-bgv-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-bgv-apis-api-openapi.yml
- filename: keka-core-hr-api-openapi.yml
  format: yaml
  label: Keka HR Core HR API
  slug: keka-core-hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-core-hr-api-openapi.yml
- filename: keka-documents-api-openapi.yml
  format: yaml
  label: Keka HR Documents API
  slug: keka-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-documents-api-openapi.yml
- filename: keka-expense-api-openapi.yml
  format: yaml
  label: Keka HR Expense API
  slug: keka-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-expense-api-openapi.yml
- filename: keka-hire-api-openapi.yml
  format: yaml
  label: Keka HR Hire API
  slug: keka-hire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-hire-api-openapi.yml
- filename: keka-leave-api-openapi.yml
  format: yaml
  label: Keka HR Leave API
  slug: keka-leave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-leave-api-openapi.yml
- filename: keka-payroll-api-openapi.yml
  format: yaml
  label: Keka HR Payroll API
  slug: keka-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-payroll-api-openapi.yml
- filename: keka-pms-api-openapi.yml
  format: yaml
  label: Keka HR PMS API
  slug: keka-pms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-pms-api-openapi.yml
- filename: keka-psa-api-openapi.yml
  format: yaml
  label: Keka HR PSA API
  slug: keka-psa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-psa-api-openapi.yml
- filename: keka-requisitions-api-openapi.yml
  format: yaml
  label: Keka HR Requisitions API
  slug: keka-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-requisitions-api-openapi.yml
- filename: keka-skills-api-openapi.yml
  format: yaml
  label: Keka HR Skills API
  slug: keka-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-skills-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Keka Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Keka HR publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Keka HR API on a user''s behalf.


  Tokens are issued from https://login.keka.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Keka HR
provider_slug: keka
schemes:
- description: OAuth 2.0 client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.keka.com/connect/token
  name: oauth2
  source: openapi/keka-hr-api-openapi.yaml
scope_count: 1
scope_names:
- kekaapi
scopes:
- description: Access to Keka HR API
  flows:
  - clientCredentials
  scope: kekaapi
slug: keka-scopes
source_filename: keka-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keka-hr-api-openapi.yaml\nschemes:\n- name: oauth2\n  source: openapi/keka-hr-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.keka.com/connect/token\n  description: OAuth 2.0 client credentials flow\nscopes:\n- scope: kekaapi\n  description: Access to Keka HR API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/keka-hr-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/scopes/keka-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- HR
- Human Resources
- Payroll
- Attendance
- Leave Management
- Performance Management
- Employee Management
- India
- HRMS
token_urls:
- https://login.keka.com/connect/token
---
