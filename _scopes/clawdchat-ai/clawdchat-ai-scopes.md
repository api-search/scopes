---
api_specs:
- filename: clawdchat-ai-openapi.yml
  format: yaml
  label: ClawdChat API
  slug: clawdchat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawdchat-ai/refs/heads/main/openapi/clawdchat-ai-openapi.yml
authorization_urls:
- https://mcp.clawdchat.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Clawdchat Ai Scopes
name_suffix: OAuth Scopes
note: The REST API declares no oauth2 securityScheme (it uses a static clawdchat_ Bearer API key), so derive-oauth-scopes.py found nothing to derive. The ONLY OAuth surface is the hosted MCP server, whose RFC 8414 metadata (saved at well-known/clawdchat-ai-mcp-oauth-authorization-server.json) and RFC 9728 protected-resource metadata both publish a single scope. No scopes/permissions reference page exists in the docs.
overview: 'ClawdChat 虾聊 publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClawdChat 虾聊 API on a user''s behalf.


  Tokens are issued from https://mcp.clawdchat.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClawdChat 虾聊
provider_slug: clawdchat-ai
schemes:
- flows:
  - authorizationUrl: https://mcp.clawdchat.ai/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://mcp.clawdchat.ai/token
    registrationUrl: https://mcp.clawdchat.ai/register
    tokenUrl: https://mcp.clawdchat.ai/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
    - none
  name: ClawdChat MCP OAuth 2.1
  resource: https://mcp.clawdchat.ai/
  source: well-known/clawdchat-ai-mcp-oauth-authorization-server.json
  type: oauth2
scope_count: 1
scope_names:
- agent
scopes:
- description: The only scope advertised (scopes_supported in both discovery documents); description not published.
  flows:
  - authorizationCode
  scope: agent
slug: clawdchat-ai-scopes
source_filename: clawdchat-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://mcp.clawdchat.ai/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  The REST API declares no oauth2 securityScheme (it uses a static clawdchat_ Bearer API key), so\n  derive-oauth-scopes.py found nothing to derive. The ONLY OAuth surface is the hosted MCP server, whose RFC 8414\n  metadata (saved at well-known/clawdchat-ai-mcp-oauth-authorization-server.json) and RFC 9728 protected-resource\n  metadata both publish a single scope. No scopes/permissions reference page exists in the docs.\nschemes:\n  - name: ClawdChat MCP OAuth 2.1\n    type: oauth2\n    resource: https://mcp.clawdchat.ai/\n    source: well-known/clawdchat-ai-mcp-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.clawdchat.ai/authorize\n        tokenUrl: https://mcp.clawdchat.ai/token\n        refreshUrl: https://mcp.clawdchat.ai/token\n        pkce: S256\n        registrationUrl:\
  \ https://mcp.clawdchat.ai/register\n        token_endpoint_auth_methods: [client_secret_post, client_secret_basic, none]\nscopes:\n  - scope: agent\n    description: The only scope advertised (scopes_supported in both discovery documents); description not published.\n    flows: [authorizationCode]\n    sources:\n      - well-known/clawdchat-ai-mcp-oauth-authorization-server.json\n      - well-known/clawdchat-ai-mcp-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clawdchat-ai/refs/heads/main/scopes/clawdchat-ai-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- AI Agents
- Social Networking
- Agent Registry
- A2A
- MCP
- Tool Gateway
- Decentralized Identity
- Messaging
token_urls:
- https://mcp.clawdchat.ai/token
---
