---
authorization_urls: []
description: ''
docs: https://github.com/luminarylane/lane-plugin
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Luminarylane App Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Luminary Lane uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Luminary Lane
provider_slug: luminarylane-app
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: luminarylane-app-scopes
source_filename: luminarylane-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://mcp.luminarylane.app/.well-known/oauth-authorization-server\ndocs: https://github.com/luminarylane/lane-plugin\ncorroborating_source: https://mcp.luminarylane.app/.well-known/oauth-protected-resource/mcp\nscope_count: 0\nsummary: >-\n  Luminary Lane publishes no OpenAPI (derive-oauth-scopes.py reports 0 oauth2 providers for this repo),\n  so this file records what the live RFC 8414 / RFC 9728 discovery documents on the MCP host declare.\n  Neither document carries scopes_supported, the provider documents no scope or permission vocabulary\n  anywhere public, and the alternative X-API-Key credential is a per-user key with no scoping surface.\n  An OAuth client therefore requests a token with no scope parameter and receives whatever the signed-in\n  user's workspace access allows. The absence is the measurement; no scope names were invented.\nmodel: >-\n  Unscoped OAuth 2.1 authorization-code + PKCE against a first-party\
  \ authorization server co-hosted with\n  the MCP resource. Authorization is workspace/brand-membership based, not scope based.\nauthorization_server:\n  issuer: https://mcp.luminarylane.app/\n  vendor: first-party (Express)\n  metadata_url: https://mcp.luminarylane.app/.well-known/oauth-authorization-server\n  http_status: 200\n  authorization_endpoint: https://mcp.luminarylane.app/authorize\n  token_endpoint: https://mcp.luminarylane.app/token\n  revocation_endpoint: https://mcp.luminarylane.app/revoke\n  registration_endpoint: https://mcp.luminarylane.app/register\n  grant_types_supported:\n    - authorization_code\n    - refresh_token\n  response_types_supported:\n    - code\n  code_challenge_methods_supported:\n    - S256\n  token_endpoint_auth_methods_supported:\n    - client_secret_post\n    - none\n  revocation_endpoint_auth_methods_supported:\n    - client_secret_post\n  scopes_supported: null\n  jwks_uri: null\nprotected_resource:\n  metadata_url: https://mcp.luminarylane.app/.well-known/oauth-protected-resource/mcp\n\
  \  http_status: 200\n  resource: https://mcp.luminarylane.app/mcp\n  resource_name: Luminary Lane MCP Server\n  authorization_servers:\n    - https://mcp.luminarylane.app/\n  scopes_supported: null\n  bearer_methods_supported: null\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luminarylane-app/refs/heads/main/scopes/luminarylane-app-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Marketing Automation
- AI Agents
- Agent-Native
- MCP
- A2A
- Brand Management
- Content Generation
- Campaign Management
- Social Media
- Software-as-a-Service
token_urls: []
---
