---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Keka HR REST API
  slug: keka-hr-rest-api
  spec_type: OpenAPI
  url: https://apidocs.keka.com/
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
