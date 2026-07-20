---
api_specs:
- filename: duvo-ai-openapi-original.json
  format: json
  label: Duvo Public API
  slug: duvo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duvo-ai/refs/heads/main/openapi/duvo-ai-openapi-original.json
authorization_urls: []
description: ''
docs: https://www.duvo.ai/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Duvo Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Duvo Ai publishes 8 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Duvo Ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Duvo Ai
provider_slug: duvo-ai
schemes:
- authorization_server_metadata: https://login.duvo.ai/.well-known/oauth-authorization-server
  flow: clientCredentials
  name: oauth2ClientCredentials
  protected_resource_metadata: https://api.duvo.ai/.well-known/oauth-protected-resource
  token_url: https://login.duvo.ai/oauth/token
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
- description: Manage webhook subscriptions for a workspace.
  flows: []
  scope: webhooks:manage
- description: Call governed Duvo tools over the hosted MCP surface.
  flows: []
  scope: mcp:call
slug: duvo-ai-scopes
source_filename: duvo-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.duvo.ai/auth.md\ndocs: https://www.duvo.ai/auth.md\nnotes: >-\n  The public OpenAPI declares only an http bearer scheme, so scopes are not\n  spec-derivable. Duvo documents OAuth client-credential scopes in its auth\n  guide (https://www.duvo.ai/auth.md) and advertises them in its agent\n  discovery manifest (well-known/duvo-ai-agent.json). Scopes apply to enterprise\n  workspaces where Duvo has enabled OAuth for the tenant.\nschemes:\n- name: oauth2ClientCredentials\n  flow: clientCredentials\n  token_url: https://login.duvo.ai/oauth/token\n  authorization_server_metadata: https://login.duvo.ai/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://api.duvo.ai/.well-known/oauth-protected-resource\nscopes:\n- scope: runs:read\n  description: Inspect run status, messages, tool calls, and audit events.\n- scope: runs:write\n  description: Start, pause, resume, or replay runs.\n- scope: queues:write\n\
  \  description: Create and update queue cases.\n- scope: approvals:write\n  description: Respond to human approval requests.\n- scope: files:read\n  description: Read files attached to authorized runs or cases.\n- scope: sandboxes:write\n  description: Request governed browser, file, or desktop execution.\n- scope: webhooks:manage\n  description: Manage webhook subscriptions for a workspace.\n- scope: mcp:call\n  description: Call governed Duvo tools over the hosted MCP surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duvo-ai/refs/heads/main/scopes/duvo-ai-scopes.yml
summary_line: 8 scopes
tags:
- Company
- Enterprise; Ai
- Process Intelligence
- Automation
- Agents
- SAP Migration
- Operations
- ERP
- Transformation
- Approvals
- Audit
- MCP
token_urls: []
---
