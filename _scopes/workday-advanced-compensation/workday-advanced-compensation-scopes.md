---
api_specs:
- filename: workday-advanced-compensation-bonus-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Bonus Plans API
  slug: workday-advanced-compensation-bonus-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-bonus-plans-api-openapi.yml
- filename: workday-advanced-compensation-compensation-budgets-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Compensation Budgets API
  slug: workday-advanced-compensation-compensation-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-compensation-budgets-api-openapi.yml
- filename: workday-advanced-compensation-compensation-grades-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Compensation Grades API
  slug: workday-advanced-compensation-compensation-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-compensation-grades-api-openapi.yml
- filename: workday-advanced-compensation-compensation-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Compensation Plans API
  slug: workday-advanced-compensation-compensation-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-compensation-plans-api-openapi.yml
- filename: workday-advanced-compensation-compensation-reviews-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Compensation Reviews API
  slug: workday-advanced-compensation-compensation-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-compensation-reviews-api-openapi.yml
- filename: workday-advanced-compensation-employee-compensation-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Employee Compensation API
  slug: workday-advanced-compensation-employee-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-employee-compensation-api-openapi.yml
- filename: workday-advanced-compensation-merit-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Merit Plans API
  slug: workday-advanced-compensation-merit-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-merit-plans-api-openapi.yml
- filename: workday-advanced-compensation-stock-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Stock Plans API
  slug: workday-advanced-compensation-stock-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-stock-plans-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Workday Advanced Compensation Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Advanced Compensation publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Advanced Compensation API on a user''s behalf.


  Tokens are issued from https://{tenant}.workday.com/ccx/oauth2/{tenant}/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Advanced Compensation
provider_slug: workday-advanced-compensation
schemes:
- description: Workday OAuth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-advanced-compensation-openapi.yml
scope_count: 2
scope_names:
- compensation.read
- compensation.write
scopes:
- description: Read compensation data
  flows:
  - clientCredentials
  scope: compensation.read
- description: Write compensation data
  flows:
  - clientCredentials
  scope: compensation.write
slug: workday-advanced-compensation-scopes
source_filename: workday-advanced-compensation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-advanced-compensation-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/workday-advanced-compensation-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n  description: Workday OAuth 2.0 authentication\nscopes:\n- scope: compensation.read\n  description: Read compensation data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/workday-advanced-compensation-openapi.yml\n- scope: compensation.write\n  description: Write compensation data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/workday-advanced-compensation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/scopes/workday-advanced-compensation-scopes.yml
summary_line: 2 scopes · clientCredentials
tags: []
token_urls:
- https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
---
