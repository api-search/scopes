---
api_specs:
- filename: factorial-openapi.yml
  format: yaml
  label: Factorial Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factorial/refs/heads/main/openapi/factorial-openapi.yml
authorization_urls:
- https://api.factorialhr.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Factorial Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Factorial publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Factorial API on a user''s behalf.


  Tokens are issued from https://api.factorialhr.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Factorial
provider_slug: factorial
schemes:
- flows:
  - authorizationUrl: https://api.factorialhr.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.factorialhr.com/oauth/token
  name: OAuth2
  source: openapi/factorial-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read HR data
  flows:
  - authorizationCode
  scope: read
- description: Modify HR data
  flows:
  - authorizationCode
  scope: write
slug: factorial-scopes
source_filename: factorial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/factorial-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/factorial-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.factorialhr.com/oauth/authorize\n    tokenUrl: https://api.factorialhr.com/oauth/token\nscopes:\n- scope: read\n  description: Read HR data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/factorial-openapi.yml\n- scope: write\n  description: Modify HR data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/factorial-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factorial/refs/heads/main/scopes/factorial-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Human Resources
- HRIS
- Employee Management
- Time Tracking
- Payroll
- Time Off
- Performance Management
token_urls:
- https://api.factorialhr.com/oauth/token
---
