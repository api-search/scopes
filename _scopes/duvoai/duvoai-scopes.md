---
api_specs:
- filename: duvoai-openapi-original.json
  format: json
  label: Duvo Public API
  slug: duvo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duvoai/refs/heads/main/openapi/duvoai-openapi-original.json
authorization_urls: []
description: ''
docs: https://www.duvo.ai/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Duvoai Scopes
name_suffix: OAuth Scopes
note: The published OpenAPI declares only an `http bearer` (API-key) scheme, but Duvo documents enterprise OAuth 2.0 client-credentials with a scoped access model in auth.md and the agent-discovery card (well-known/duvoai-agent.json). Scopes below are captured verbatim from those sources. Standard OIDC scopes (openid, profile, email, offline_access, ...) are additionally advertised at login.duvo.ai/.well-known/oauth-authorization-server.
overview: 'duvo.ai publishes 8 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the duvo.ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: duvo.ai
provider_slug: duvoai
schemes: []
scope_count: 8
scope_names:
- runs:read
- runs:write
- queues:write
- approvals:write
- files:read
- sandboxes:write
- webhooks:manage
- mcp:call
scopes:
- description: Inspect run status, messages, tool calls, and audit events.
  flows: []
  scope: runs:read
- description: Start, pause, resume, or replay runs.
  flows: []
  scope: runs:write
- description: Create and update queue cases.
  flows: []
  scope: queues:write
- description: Respond to human approval requests.
  flows: []
  scope: approvals:write
- description: Read files attached to authorized runs or cases.
  flows: []
  scope: files:read
- description: Request governed browser, file, or desktop execution.
  flows: []
  scope: sandboxes:write
- description: Manage webhook subscriptions.
  flows: []
  scope: webhooks:manage
- description: Invoke the hosted Duvo MCP surface for approved workspaces.
  flows: []
  scope: mcp:call
slug: duvoai-scopes
source_filename: duvoai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.duvo.ai/auth.md\ndocs: https://www.duvo.ai/auth.md\nnote: >-\n  The published OpenAPI declares only an `http bearer` (API-key) scheme, but\n  Duvo documents enterprise OAuth 2.0 client-credentials with a scoped access\n  model in auth.md and the agent-discovery card\n  (well-known/duvoai-agent.json). Scopes below are captured verbatim from those\n  sources. Standard OIDC scopes (openid, profile, email, offline_access, ...)\n  are additionally advertised at login.duvo.ai/.well-known/oauth-authorization-server.\nauthorization_server: https://login.duvo.ai/\ntoken_endpoint: https://login.duvo.ai/oauth/token\nflows:\n- flow: clientCredentials\n  tokenUrl: https://login.duvo.ai/oauth/token\nscopes:\n- scope: runs:read\n  description: Inspect run status, messages, tool calls, and audit events.\n- scope: runs:write\n  description: Start, pause, resume, or replay runs.\n- scope: queues:write\n  description: Create and update\
  \ queue cases.\n- scope: approvals:write\n  description: Respond to human approval requests.\n- scope: files:read\n  description: Read files attached to authorized runs or cases.\n- scope: sandboxes:write\n  description: Request governed browser, file, or desktop execution.\n- scope: webhooks:manage\n  description: Manage webhook subscriptions.\n- scope: mcp:call\n  description: Invoke the hosted Duvo MCP surface for approved workspaces.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duvoai/refs/heads/main/scopes/duvoai-scopes.yml
summary_line: 8 scopes
tags:
- Company
- Ai Ml
- Process Intelligence
- Automation
- Agents
- MCP
- Enterprise Operations
- SAP Migration
- Workflow
token_urls: []
---
