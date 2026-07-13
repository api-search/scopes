---
api_specs:
- filename: abacus-api-openapi.yaml
  format: yaml
  label: Abacus API
  slug: abacus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/openapi/abacus-api-openapi.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Abacus Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Abacus publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Abacus API on a user''s behalf.


  Tokens are issued from https://api.abacus.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Abacus
provider_slug: abacus
schemes:
- description: OAuth 2.0 client credentials flow for API authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.abacus.com/oauth/token
  name: OAuth2
  source: openapi/abacus-api-openapi.yaml
scope_count: 3
scope_names:
- expenses:read
- members:read
- members:write
scopes:
- description: Read expense reports
  flows:
  - clientCredentials
  scope: expenses:read
- description: Read member information
  flows:
  - clientCredentials
  scope: members:read
- description: Create and update members
  flows:
  - clientCredentials
  scope: members:write
slug: abacus-scopes
source_filename: abacus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/abacus-api-openapi.yaml\nschemes:\n- name: OAuth2\n  source: openapi/abacus-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.abacus.com/oauth/token\n  description: OAuth 2.0 client credentials flow for API authentication\nscopes:\n- scope: expenses:read\n  description: Read expense reports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/abacus-api-openapi.yaml\n- scope: members:read\n  description: Read member information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/abacus-api-openapi.yaml\n- scope: members:write\n  description: Create and update members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/abacus-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/scopes/abacus-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
token_urls:
- https://api.abacus.com/oauth/token
---
