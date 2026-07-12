---
authorization_urls:
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Factorial Hr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Factorial publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Factorial API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Factorial
provider_slug: factorial-hr
schemes:
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: oauth2
  source: openapi/factorial-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Required for all operations
  flows:
  - authorizationCode
  scope: read
- description: Required for write operations
  flows:
  - authorizationCode
  scope: write
slug: factorial-hr-scopes
source_filename: factorial-hr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/factorial-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/factorial-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\nscopes:\n- scope: read\n  description: Required for all operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/factorial-openapi.yml\n- scope: write\n  description: Required for write operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/factorial-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factorial-hr/refs/heads/main/scopes/factorial-hr-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- HR
- Human Resources
- Payroll
- Time Off
- Time Tracking
- ATS
- Performance
- Finance
- Expenses
- Spain
- Barcelona
- All-in-One
token_urls:
- /oauth/token
---
