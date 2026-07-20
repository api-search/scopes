---
api_specs:
- filename: allowance-openapi-original.json
  format: json
  label: Allowance API
  slug: allowance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allowance/refs/heads/main/openapi/allowance-openapi-original.json
authorization_urls:
- https://useallowance.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Allowance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allowance publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allowance API on a user''s behalf.


  Tokens are issued from https://useallowance.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allowance
provider_slug: allowance
schemes:
- description: OAuth2 authorization code flow (planned — not yet active)
  flows:
  - authorizationUrl: https://useallowance.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://useallowance.com/oauth/token
  name: OAuth2
  source: openapi/allowance-openapi-original.json
scope_count: 3
scope_names:
- credentials:request
- mandates:read
- mandates:write
scopes:
- description: Request payment credentials against active mandates
  flows:
  - authorizationCode
  scope: credentials:request
- description: Read mandate details and status
  flows:
  - authorizationCode
  scope: mandates:read
- description: Propose and manage spending mandates
  flows:
  - authorizationCode
  scope: mandates:write
slug: allowance-scopes
source_filename: allowance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/allowance-openapi-original.json\nschemes:\n- name: OAuth2\n  source: openapi/allowance-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://useallowance.com/oauth/authorize\n    tokenUrl: https://useallowance.com/oauth/token\n  description: OAuth2 authorization code flow (planned — not yet active)\nscopes:\n- scope: credentials:request\n  description: Request payment credentials against active mandates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/allowance-openapi-original.json\n- scope: mandates:read\n  description: Read mandate details and status\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/allowance-openapi-original.json\n- scope: mandates:write\n  description: Propose and manage spending mandates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/allowance-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allowance/refs/heads/main/scopes/allowance-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Payments
- Agentic Payments
- AI Agents
- Virtual Cards
- Fintech
- Model Context Protocol
- Consumer Trust
- Spending Controls
- AP2
token_urls:
- https://useallowance.com/oauth/token
---
