---
api_specs:
- filename: monday-com-webhooks-asyncapi.yml
  format: yaml
  label: Monday.com API
  slug: monday-com
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/monday-com/refs/heads/main/asyncapi/monday-com-webhooks-asyncapi.yml
authorization_urls:
- https://auth.monday.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Monday Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Monday.com publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Monday.com API on a user''s behalf.


  Tokens are issued from https://auth.monday.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Monday.com
provider_slug: monday-com
schemes:
- flows:
  - authorizationUrl: https://auth.monday.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.monday.com/oauth2/token
  name: oauth2
  source: openapi/monday-com-openapi.yml
scope_count: 7
scope_names:
- boards:read
- boards:write
- notifications:write
- updates:write
- users:read
- webhooks:write
- workspaces:read
scopes:
- description: Read boards, items, columns, groups
  flows:
  - authorizationCode
  scope: boards:read
- description: Create and update boards, items, columns, groups
  flows:
  - authorizationCode
  scope: boards:write
- description: Create notifications
  flows:
  - authorizationCode
  scope: notifications:write
- description: Create updates and replies
  flows:
  - authorizationCode
  scope: updates:write
- description: Read user, team, and account information
  flows:
  - authorizationCode
  scope: users:read
- description: Create and manage webhooks
  flows:
  - authorizationCode
  scope: webhooks:write
- description: Read workspaces
  flows:
  - authorizationCode
  scope: workspaces:read
slug: monday-com-scopes
source_filename: monday-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/monday-com-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/monday-com-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.monday.com/oauth2/authorize\n    tokenUrl: https://auth.monday.com/oauth2/token\nscopes:\n- scope: boards:read\n  description: Read boards, items, columns, groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/monday-com-openapi.yml\n- scope: boards:write\n  description: Create and update boards, items, columns, groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/monday-com-openapi.yml\n- scope: notifications:write\n  description: Create notifications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/monday-com-openapi.yml\n- scope: updates:write\n  description: Create updates and replies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/monday-com-openapi.yml\n- scope: users:read\n  description: Read user, team, and\
  \ account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/monday-com-openapi.yml\n- scope: webhooks:write\n  description: Create and manage webhooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/monday-com-openapi.yml\n- scope: workspaces:read\n  description: Read workspaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/monday-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monday-com/refs/heads/main/scopes/monday-com-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Work Management
- CRM
- Automation
- GraphQL
token_urls:
- https://auth.monday.com/oauth2/token
---
