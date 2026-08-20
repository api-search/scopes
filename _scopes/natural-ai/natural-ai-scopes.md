---
api_specs:
- filename: natural-ai-agent-keys-api-openapi.yml
  format: yaml
  label: Natural AI Agent Keys API
  slug: natural-ai-agent-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-agent-keys-api-openapi.yml
- filename: natural-ai-agents-api-openapi.yml
  format: yaml
  label: Natural AI Agents API
  slug: natural-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-agents-api-openapi.yml
- filename: natural-ai-api-keys-api-openapi.yml
  format: yaml
  label: Natural AI API Keys API
  slug: natural-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-api-keys-api-openapi.yml
- filename: natural-ai-approvals-api-openapi.yml
  format: yaml
  label: Natural AI Approvals API
  slug: natural-ai-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-approvals-api-openapi.yml
- filename: natural-ai-customers-api-openapi.yml
  format: yaml
  label: Natural AI Customers API
  slug: natural-ai-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-customers-api-openapi.yml
- filename: natural-ai-events-api-openapi.yml
  format: yaml
  label: Natural AI Events API
  slug: natural-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-events-api-openapi.yml
- filename: natural-ai-external-accounts-api-openapi.yml
  format: yaml
  label: Natural AI External Accounts API
  slug: natural-ai-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-external-accounts-api-openapi.yml
- filename: natural-ai-invitations-api-openapi.yml
  format: yaml
  label: Natural AI Invitations API
  slug: natural-ai-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-invitations-api-openapi.yml
- filename: natural-ai-parties-api-openapi.yml
  format: yaml
  label: Natural AI Parties API
  slug: natural-ai-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-parties-api-openapi.yml
- filename: natural-ai-paymentrequests-api-openapi.yml
  format: yaml
  label: Natural AI PaymentRequests API
  slug: natural-ai-paymentrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-paymentrequests-api-openapi.yml
- filename: natural-ai-payments-api-openapi.yml
  format: yaml
  label: Natural AI Payments API
  slug: natural-ai-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-payments-api-openapi.yml
- filename: natural-ai-transactions-api-openapi.yml
  format: yaml
  label: Natural AI Transactions API
  slug: natural-ai-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-transactions-api-openapi.yml
- filename: natural-ai-transfers-api-openapi.yml
  format: yaml
  label: Natural AI Transfers API
  slug: natural-ai-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-transfers-api-openapi.yml
- filename: natural-ai-wallets-api-openapi.yml
  format: yaml
  label: Natural AI Wallets API
  slug: natural-ai-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-wallets-api-openapi.yml
- filename: natural-ai-webhooks-api-openapi.yml
  format: yaml
  label: Natural AI Webhooks API
  slug: natural-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-webhooks-api-openapi.yml
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
- Artificial Intelligence
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
