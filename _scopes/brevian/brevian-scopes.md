---
authorization_urls:
- https://app.brevian.ai/mcp/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Brevian Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Brevian publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brevian API on a user''s behalf.


  Tokens are issued from https://app.brevian.ai/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brevian
provider_slug: brevian
schemes:
- flows:
  - authorizationUrl: https://app.brevian.ai/mcp/authorize
    flow: authorizationCode
    tokenUrl: https://app.brevian.ai/mcp/token
  name: BrevianMCPOAuth
  source: well-known/brevian-oauth-authorization-server.json
scope_count: 1
scope_names:
- brevian:read
scopes:
- description: Read access to Brevian revenue-execution context (knowledge, deals, conversations, pipeline) exposed through the hosted MCP server.
  flows:
  - authorizationCode
  scope: brevian:read
slug: brevian-scopes
source_filename: brevian-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.brevian.ai/.well-known/oauth-authorization-server\nschemes:\n- name: BrevianMCPOAuth\n  source: well-known/brevian-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.brevian.ai/mcp/authorize\n    tokenUrl: https://app.brevian.ai/mcp/token\nscopes:\n- scope: brevian:read\n  description: >-\n    Read access to Brevian revenue-execution context (knowledge, deals,\n    conversations, pipeline) exposed through the hosted MCP server.\n  flows: [authorizationCode]\n  sources: [well-known/brevian-oauth-authorization-server.json]\nnotes: >-\n  brevian:read is the only scope advertised in scopes_supported of the OAuth\n  Authorization Server metadata. No broader write/admin scopes are published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brevian/refs/heads/main/scopes/brevian-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Artificial Intelligence
- Sales
- Revenue Execution
- AI Agents
- CRM
- Model Context Protocol
- Enterprise
token_urls:
- https://app.brevian.ai/mcp/token
---
