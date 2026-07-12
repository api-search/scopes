---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Broadridge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'broadridge publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the broadridge API on a user''s behalf.


  Tokens are issued from https://auth.broadridge.example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: broadridge
provider_slug: broadridge
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.broadridge.example.com/oauth/token
  name: oauth2
  source: openapi/broadridge-wealth-openapi.yml
scope_count: 3
scope_names:
- accounts:read
- positions:read
- transactions:read
scopes:
- description: Read account data
  flows:
  - clientCredentials
  scope: accounts:read
- description: Read position data
  flows:
  - clientCredentials
  scope: positions:read
- description: Read transaction data
  flows:
  - clientCredentials
  scope: transactions:read
slug: broadridge-scopes
source_filename: broadridge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/broadridge-wealth-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/broadridge-wealth-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.broadridge.example.com/oauth/token\nscopes:\n- scope: accounts:read\n  description: Read account data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/broadridge-wealth-openapi.yml\n- scope: positions:read\n  description: Read position data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/broadridge-wealth-openapi.yml\n- scope: transactions:read\n  description: Read transaction data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/broadridge-wealth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broadridge/refs/heads/main/scopes/broadridge-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Fortune 1000
token_urls:
- https://auth.broadridge.example.com/oauth/token
---
