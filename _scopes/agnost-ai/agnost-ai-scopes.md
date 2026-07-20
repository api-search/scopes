---
api_specs:
- filename: agnost-ai-openapi-original.yml
  format: yaml
  label: Agnost AI API
  slug: agnost-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/openapi/agnost-ai-openapi-original.yml
authorization_urls:
- https://mcp.agnost.ai/authorize
description: ''
docs: https://docs.agnost.ai/agnost-mcp-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Agnost Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Agnost AI publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agnost AI API on a user''s behalf.


  Tokens are issued from https://mcp.agnost.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agnost AI
provider_slug: agnost-ai
schemes:
- flows:
  - authorizationUrl: https://mcp.agnost.ai/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://mcp.agnost.ai/register
    tokenUrl: https://mcp.agnost.ai/token
  name: MCP OAuth 2.1
  source: https://mcp.agnost.ai/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- agnost
scopes:
- description: Grants an OAuth-authenticated MCP client read access to the signed-in user's Agnost dashboard data (errors, intents, conversations, SOPs, sentiments) for the organization they are logged into.
  flows:
  - authorizationCode
  scope: agnost
slug: agnost-ai-scopes
source_filename: agnost-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://mcp.agnost.ai/.well-known/oauth-authorization-server\ndocs: https://docs.agnost.ai/agnost-mcp-server\n# The Agnost REST API itself uses header apiKey auth (x-org-id / x-api-key) and\n# JWT bearer, not OAuth2 — so there are no REST OAuth scopes. The only OAuth\n# surface is the hosted MCP server (OAuth 2.1, dynamic client registration),\n# which advertises a single scope.\nschemes:\n- name: MCP OAuth 2.1\n  source: https://mcp.agnost.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.agnost.ai/authorize\n    tokenUrl: https://mcp.agnost.ai/token\n    registrationUrl: https://mcp.agnost.ai/register\n    pkce: S256\nscopes:\n- scope: agnost\n  description: >-\n    Grants an OAuth-authenticated MCP client read access to the signed-in user's\n    Agnost dashboard data (errors, intents, conversations, SOPs, sentiments) for\n    the organization they are logged\
  \ into.\n  flows: [authorizationCode]\n  sources: [https://mcp.agnost.ai/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agnost-ai/refs/heads/main/scopes/agnost-ai-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- AI Agents
- Agent Analytics
- Observability
- OpenTelemetry
- Model Context Protocol
- Conversational AI
- Monitoring
- Developer Tools
- Analytics
token_urls:
- https://mcp.agnost.ai/token
---
