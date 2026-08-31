---
api_specs:
- filename: samaya-ai-organizations-api-openapi.yml
  format: yaml
  label: Samaya AI Organizations API
  slug: samaya-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-organizations-api-openapi.yml
- filename: samaya-ai-teams-api-openapi.yml
  format: yaml
  label: Samaya AI Teams API
  slug: samaya-ai-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-teams-api-openapi.yml
- filename: samaya-ai-users-api-openapi.yml
  format: yaml
  label: Samaya AI Users API
  slug: samaya-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-users-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Samaya Ai Scopes
name_suffix: OAuth Scopes
note: 'Samaya''s MCP authorization server publishes RFC 9728 protected-resource metadata with an EMPTY scopes_supported array, and the RFC 8414 authorization-server document declares no scopes_supported key at all. This is a measured absence, not an unchecked field: the server runs OAuth 2.1 with dynamic client registration and PKCE S256 but exposes no granular permission vocabulary, so an agent connecting to it cannot request or be granted least privilege at the protocol level. The published REST OpenAPI declares no oauth2 securityScheme (it uses a WorkOS bearer token), so it contributes no scopes either.'
overview: 'Samaya AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Samaya AI
provider_slug: samaya-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: samaya-ai-scopes
source_filename: samaya-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://mcp.samaya.ai/.well-known/oauth-protected-resource/mcp\nscope_count: 0\nscopes: []\nnote: >-\n  Samaya's MCP authorization server publishes RFC 9728 protected-resource metadata with an EMPTY\n  scopes_supported array, and the RFC 8414 authorization-server document declares no scopes_supported\n  key at all. This is a measured absence, not an unchecked field: the server runs OAuth 2.1 with\n  dynamic client registration and PKCE S256 but exposes no granular permission vocabulary, so an\n  agent connecting to it cannot request or be granted least privilege at the protocol level. The\n  published REST OpenAPI declares no oauth2 securityScheme (it uses a WorkOS bearer token), so it\n  contributes no scopes either.\nauthorization_server:\n  issuer: https://mcp.samaya.ai/\n  authorization_endpoint: https://mcp.samaya.ai/authorize\n  token_endpoint: https://mcp.samaya.ai/token\n  registration_endpoint: https://mcp.samaya.ai/register\n\
  \  revocation_endpoint: https://mcp.samaya.ai/revoke\n  code_challenge_methods_supported:\n  - S256\ndocs: null\nevidence:\n- url: https://mcp.samaya.ai/.well-known/oauth-protected-resource/mcp\n  status: 200\n  scopes_supported: []\n- url: https://mcp.samaya.ai/.well-known/oauth-authorization-server\n  status: 200\n  scopes_supported: absent\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/scopes/samaya-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- artificial-intelligence
- Financial-Services
- investment-research
- AI Agents
- MCP
- agent-native
- capital-markets
- enterprise-search
- retrieval
- graphql
token_urls: []
---
