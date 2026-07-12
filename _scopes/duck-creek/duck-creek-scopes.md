---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Duck Creek Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'duck-creek publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the duck-creek API on a user''s behalf.


  Tokens are issued from https://api.duckcreek.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: duck-creek
provider_slug: duck-creek
schemes:
- description: OAuth 2.0 for Duck Creek Anywhere API authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.duckcreek.com/oauth/token
  name: oauth2
  source: openapi/duck-creek-policy-openapi.yml
scope_count: 5
scope_names:
- billing:read
- claims:read
- claims:write
- policies:read
- policies:write
scopes:
- description: Read billing data
  flows:
  - clientCredentials
  scope: billing:read
- description: Read claim data
  flows:
  - clientCredentials
  scope: claims:read
- description: Create and update claims
  flows:
  - clientCredentials
  scope: claims:write
- description: Read policy data
  flows:
  - clientCredentials
  scope: policies:read
- description: Create and modify policies
  flows:
  - clientCredentials
  scope: policies:write
slug: duck-creek-scopes
source_filename: duck-creek-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/duck-creek-policy-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/duck-creek-policy-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.duckcreek.com/oauth/token\n  description: OAuth 2.0 for Duck Creek Anywhere API authentication\nscopes:\n- scope: billing:read\n  description: Read billing data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/duck-creek-policy-openapi.yml\n- scope: claims:read\n  description: Read claim data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/duck-creek-policy-openapi.yml\n- scope: claims:write\n  description: Create and update claims\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/duck-creek-policy-openapi.yml\n- scope: policies:read\n  description: Read policy data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/duck-creek-policy-openapi.yml\n- scope: policies:write\n  description: Create and modify policies\n \
  \ flows:\n  - clientCredentials\n  sources:\n  - openapi/duck-creek-policy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/scopes/duck-creek-scopes.yml
summary_line: 5 scopes · clientCredentials
tags: []
token_urls:
- https://api.duckcreek.com/oauth/token
---
