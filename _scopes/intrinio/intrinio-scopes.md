---
authorization_urls:
- https://intrinio-mcp.intrinio.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Intrinio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Intrinio publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Intrinio API on a user''s behalf.


  Tokens are issued from https://intrinio-mcp.intrinio.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Intrinio
provider_slug: intrinio
schemes:
- dynamic_client_registration: https://intrinio-mcp.intrinio.com/register
  flows:
  - authorizationUrl: https://intrinio-mcp.intrinio.com/authorize
    flow: authorizationCode
    refreshUrl: https://intrinio-mcp.intrinio.com/token
    tokenUrl: https://intrinio-mcp.intrinio.com/token
  name: Intrinio MCP OAuth
  pkce: S256
  revocation: https://intrinio-mcp.intrinio.com/revoke
  source: well-known/intrinio-oauth-authorization-server.json
scope_count: 1
scope_names:
- intrinio
scopes:
- description: Single advertised scope for the Intrinio MCP server (scopes_supported in the RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata). Grants access to the Intrinio data catalog through the MCP surface; effective dataset entitlements are governed by the account's subscription tier, not by finer-grained OAuth scopes.
  flows:
  - authorizationCode
  scope: intrinio
slug: intrinio-scopes
source_filename: intrinio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://intrinio-mcp.intrinio.com/.well-known/oauth-authorization-server\nschemes:\n  - name: Intrinio MCP OAuth\n    source: well-known/intrinio-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://intrinio-mcp.intrinio.com/authorize\n        tokenUrl: https://intrinio-mcp.intrinio.com/token\n        refreshUrl: https://intrinio-mcp.intrinio.com/token\n    pkce: S256\n    dynamic_client_registration: https://intrinio-mcp.intrinio.com/register\n    revocation: https://intrinio-mcp.intrinio.com/revoke\nscopes:\n  - scope: intrinio\n    description: >-\n      Single advertised scope for the Intrinio MCP server (scopes_supported in the RFC 8414\n      authorization-server metadata and RFC 9728 protected-resource metadata). Grants access\n      to the Intrinio data catalog through the MCP surface; effective dataset entitlements\n      are governed by the account's subscription\
  \ tier, not by finer-grained OAuth scopes.\n    flows: [authorizationCode]\n    sources: [well-known/intrinio-oauth-authorization-server.json]\nnotes: >-\n  The core REST API (api-v2.intrinio.com) is API-key authenticated and exposes no OAuth\n  scope surface; this scope model applies to the hosted MCP server only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intrinio/refs/heads/main/scopes/intrinio-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Finance
- Financial Data
- Market Data
- Stocks
- Options
- Fundamentals
- ETFs
- Real-Time Data
token_urls:
- https://intrinio-mcp.intrinio.com/token
---
