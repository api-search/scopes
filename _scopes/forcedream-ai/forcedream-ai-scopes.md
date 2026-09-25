---
api_specs:
- filename: forcedream-ai-openapi.yml
  format: yaml
  label: ForceDream API
  slug: forcedream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forcedream-ai/refs/heads/main/openapi/forcedream-ai-openapi.yml
authorization_urls: []
description: 'ForceDream''s OAuth scope surface is small and lives in machine-readable discovery documents rather than a scopes reference page (none exists): two scopes in the RFC 8414 / RFC 9728 metadata for the MCP resource, and one scope declared on the A2A agent card. The published OpenAPI declares only bearerAuth, so derive-oauth-scopes.py produced nothing; this file is authored from the discovery documents.'
docs: https://forcedream.ai/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Forcedream Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ForceDream uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ForceDream
provider_slug: forcedream-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: forcedream-ai-scopes
source_filename: forcedream-ai-scopes.yml
source_heading: OAuth Scopes
source_url: well-known/forcedream-ai-oauth-authorization-server.json (scopes_supported)
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.forcedream.ai/.well-known/oauth-authorization-server\nsources:\n  - well-known/forcedream-ai-oauth-authorization-server.json (scopes_supported)\n  - well-known/forcedream-ai-oauth-protected-resource.json (scopes_supported)\n  - a2a/forcedream-ai-agent-card.json (securitySchemes.oauth2.flows.authorizationCode.scopes, security[])\n  - https://github.com/forcedreamai/forcedream-mcp/blob/main/README.md\ndocs: https://forcedream.ai/mcp\ndescription: >-\n  ForceDream's OAuth scope surface is small and lives in machine-readable discovery documents rather than a\n  scopes reference page (none exists): two scopes in the RFC 8414 / RFC 9728 metadata for the MCP resource,\n  and one scope declared on the A2A agent card. The published OpenAPI declares only bearerAuth, so\n  derive-oauth-scopes.py produced nothing; this file is authored from the discovery documents.\nissuer: https://api.forcedream.ai\nresource: https://api.forcedream.ai/v1/mcp\n\
  authorization_endpoint: https://api.forcedream.ai/v1/oauth/authorize\ntoken_endpoint: https://api.forcedream.ai/v1/oauth/token\nregistration_endpoint: https://api.forcedream.ai/v1/oauth/register\ngrant_types: [authorization_code, refresh_token]\npkce: S256\nscope_count: 3\nscopes:\n  - id: 'mcp:invoke'\n    description: Invoke MCP tools that spend balance (forcedream_invoke_agent, forcedream_execute_plan, the named-agent tools).\n    declared_in: [oauth-authorization-server.scopes_supported, oauth-protected-resource.scopes_supported]\n    resource: https://api.forcedream.ai/v1/mcp\n  - id: 'mcp:tools'\n    description: Access the MCP tool surface.\n    declared_in: [oauth-authorization-server.scopes_supported, oauth-protected-resource.scopes_supported]\n    resource: https://api.forcedream.ai/v1/mcp\n  - id: agent.execute\n    description: Discover, price and execute ForceDream agents, and retrieve the signed record of what ran.\n    declared_in: ['a2a agent card securitySchemes.oauth2',\
  \ 'card security[] requires it']\n    resource: https://api.forcedream.ai/v1/a2a/execute\nnotes:\n  - The provider's own descriptions exist only for agent.execute (on the card); the two mcp:* descriptions above are inferred from the tool auth table in the MCP README and are marked as such by their brevity.\n  - Scopes are not documented on any REST route; REST authorisation is by key type (fd_live_ vs sk_fd_), see authentication/forcedream-ai-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forcedream-ai/refs/heads/main/scopes/forcedream-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI Agents
- Agent Marketplace
- MCP
- A2A
- Cryptographic Proofs
- AI Inference Routing
- Agentic Payments
- Agentic Commerce
- Agent-Native
- United Kingdom
token_urls: []
---
