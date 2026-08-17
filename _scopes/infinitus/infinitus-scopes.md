---
authorization_urls:
- https://www.infinitus.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Infinitus Scopes
name_suffix: OAuth Scopes
note: Not derived from OpenAPI — Infinitus publishes none. These scopes come from the RFC 8414 Authorization Server Metadata document and the RFC 9728 Protected Resource Metadata document that Infinitus serves at www.infinitus.ai. Exactly one scope is advertised, and it governs the MCP server on the WordPress marketing host — not the healthcare product API at api.infinitusai.com, which publishes no scope reference at all.
overview: 'Infinitus publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Infinitus API on a user''s behalf.


  Tokens are issued from https://www.infinitus.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Infinitus
provider_slug: infinitus
schemes:
- flows:
  - authorizationUrl: https://www.infinitus.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://www.infinitus.ai/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://www.infinitus.ai/oauth/token
  issuer: https://www.infinitus.ai
  name: infinitus-wordpress-oauth
  source: https://www.infinitus.ai/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the Model Context Protocol server at https://www.infinitus.ai/wp-json/mcp/mcp-oauth-server. The single scope advertised in both scopes_supported arrays.
  flows:
  - authorizationCode
  scope: mcp
slug: infinitus-scopes
source_filename: infinitus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: https://www.infinitus.ai/.well-known/oauth-authorization-server\nnote: >-\n  Not derived from OpenAPI — Infinitus publishes none. These scopes come from\n  the RFC 8414 Authorization Server Metadata document and the RFC 9728 Protected\n  Resource Metadata document that Infinitus serves at www.infinitus.ai. Exactly\n  one scope is advertised, and it governs the MCP server on the WordPress\n  marketing host — not the healthcare product API at api.infinitusai.com, which\n  publishes no scope reference at all.\n\nschemes:\n- name: infinitus-wordpress-oauth\n  source: https://www.infinitus.ai/.well-known/oauth-authorization-server\n  issuer: https://www.infinitus.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.infinitus.ai/oauth/authorize\n    tokenUrl: https://www.infinitus.ai/oauth/token\n    revocationUrl: https://www.infinitus.ai/oauth/revoke\n    pkce: S256\n    scopes: [mcp]\n\nscopes:\n- scope:\
  \ mcp\n  description: >-\n    Access the Model Context Protocol server at\n    https://www.infinitus.ai/wp-json/mcp/mcp-oauth-server. The single scope\n    advertised in both scopes_supported arrays.\n  flows: [authorizationCode]\n  resource: https://www.infinitus.ai/wp-json/mcp/mcp-oauth-server\n  sources:\n  - https://www.infinitus.ai/.well-known/oauth-authorization-server\n  - https://www.infinitus.ai/.well-known/oauth-protected-resource\n\nsummary:\n  scope_count: 1\n  granularity: coarse\n  note: >-\n    A single all-or-nothing \"mcp\" scope. There is no read/write or per-resource\n    separation, so an agent granted this scope receives whatever the server\n    exposes in full. Recorded as measured.\n\ngaps:\n- gap: product-api-scopes-unpublished\n  detail: >-\n    api.infinitusai.com advertises no OAuth metadata (both\n    /.well-known/oauth-authorization-server and\n    /.well-known/oauth-protected-resource return 404), and no permissions\n    reference page exists in the public\
  \ knowledge base. Portal authorization is\n    described only as role-based (RBAC) with no published role or scope list.\n\nx-evidence:\n- fetched: '2026-08-15'\n  url: https://www.infinitus.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n- fetched: '2026-08-15'\n  url: https://www.infinitus.ai/.well-known/oauth-protected-resource\n  http_status: 200\n  content_type: application/json\n- fetched: '2026-08-15'\n  url: https://api.infinitusai.com/.well-known/oauth-authorization-server\n  http_status: 404\n  kind: negative-probe\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinitus/refs/heads/main/scopes/infinitus-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Ai
- Healthcare
- Voice AI
- Benefit Verification
- Prior Authorization
- HIPAA
token_urls:
- https://www.infinitus.ai/oauth/token
---
