---
authorization_urls:
- https://mcp.corvera.ai/authorize
description: ''
docs: https://docs.corvera.ai/quickstart
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Corvera Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Corvera publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Corvera API on a user''s behalf.


  Tokens are issued from https://mcp.corvera.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Corvera
provider_slug: corvera
schemes:
- flows:
  - authorizationUrl: https://mcp.corvera.ai/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://mcp.corvera.ai/register
    tokenUrl: https://mcp.corvera.ai/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: OAuth2
  source: https://mcp.corvera.ai/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- email
- profile
- user:org:read
scopes:
- description: OpenID Connect authentication (subject identity).
  flows:
  - authorizationCode
  scope: openid
- description: Access the authenticated user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Access the authenticated user's basic profile.
  flows:
  - authorizationCode
  scope: profile
- description: Read access to the user's organization / workspace context. Combined with Corvera's per-account integration gating, this determines which dataset tools the connected AI tool can call.
  flows:
  - authorizationCode
  scope: user:org:read
slug: corvera-scopes
source_filename: corvera-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://mcp.corvera.ai/.well-known/oauth-authorization-server\ndocs: https://docs.corvera.ai/quickstart\nschemes:\n  - name: OAuth2\n    source: https://mcp.corvera.ai/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.corvera.ai/authorize\n        tokenUrl: https://mcp.corvera.ai/token\n        registrationUrl: https://mcp.corvera.ai/register\n        pkce: S256\n        grant_types: [authorization_code, refresh_token]\n        token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (subject identity).\n    flows: [authorizationCode]\n    sources: [well-known/corvera-oauth-authorization-server.json]\n  - scope: email\n    description: Access the authenticated user's email address.\n    flows: [authorizationCode]\n    sources: [well-known/corvera-oauth-authorization-server.json]\n\
  \  - scope: profile\n    description: Access the authenticated user's basic profile.\n    flows: [authorizationCode]\n    sources: [well-known/corvera-oauth-authorization-server.json]\n  - scope: user:org:read\n    description: >-\n      Read access to the user's organization / workspace context. Combined with\n      Corvera's per-account integration gating, this determines which dataset\n      tools the connected AI tool can call.\n    flows: [authorizationCode]\n    sources: [well-known/corvera-oauth-authorization-server.json]\nnotes: >-\n  Scopes are advertised via RFC 8414 metadata on the product MCP server.\n  Data-access authorization beyond these OAuth scopes is enforced by Corvera's\n  role-based dataset access controls and per-account integration gating rather\n  than by additional OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corvera/refs/heads/main/scopes/corvera-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- MCP
- Model Context Protocol
- CPG
- Consumer Packaged Goods
- Retail
- Data
- Context Layer
- AI Agents
- Analytics
- Y Combinator
token_urls:
- https://mcp.corvera.ai/token
---
