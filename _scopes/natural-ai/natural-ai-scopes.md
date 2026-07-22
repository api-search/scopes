---
api_specs:
- filename: natural-ai-openapi-original.json
  format: json
  label: Natural API
  slug: natural-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-openapi-original.json
authorization_urls:
- https://api.natural.com/oauth/authorize
description: ''
docs: https://docs.natural.com/api-reference/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Natural Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Natural AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.natural.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Natural AI
provider_slug: natural-ai
schemes:
- flows:
  - authorizationUrl: https://api.natural.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.natural.com/oauth/token
  name: OAuth2
  source: https://api.natural.com/.well-known/oauth-authorization-server
scope_count: 0
scope_names: []
scopes: []
slug: natural-ai-scopes
source_filename: natural-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.natural.com/.well-known/oauth-authorization-server\ndocs: https://docs.natural.com/api-reference/authentication\nschemes:\n- name: OAuth2\n  source: https://api.natural.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.natural.com/oauth/authorize\n    tokenUrl: https://api.natural.com/oauth/token\n# OAuth (MCP) scopes advertised by the authorization server\noauth_scopes:\n- scope: payments:move\n  description: Send, request, fulfill, and move money on behalf of the grant.\n- scope: external-accounts:link\n  description: Link and manage external bank accounts.\n- scope: agents:operate\n  description: Operate as / manage agents.\n- scope: customers:invite\n  description: Invite and manage connected customers.\n# Fine-grained API-key permission scopes (documented, resource.action form)\napi_key_scopes:\n- agents.read\n- agents.create\n- agents.update\n\
  - agent_keys.create\n- payments.read\n- payments.create\n- payment_requests.create\n- wallets.read\n- wallets.create\n- wallets.update\n- customers.create\n- external_accounts.create\n- party.read\n- party.update\nnotes:\n- OAuth (MCP) scopes and API-key permission scopes are distinct grant surfaces.\n- API keys can be scoped down to a subset of permissions (e.g. read-only, payments-only).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/scopes/natural-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Ai
- Payments
- Agents
- Fintech
- Money Movement
- Wallets
- Agentic Payments
- MCP
token_urls:
- https://api.natural.com/oauth/token
---
