---
authorization_urls:
- https://cloud9.gg/oauth/authorize
description: Cloud9's only OAuth surface is the authorization server advertised on cloud9.gg for its remote MCP server. It declares a single coarse scope, `mcp`. Cloud9 publishes no developer program, no scope or permission reference, and no OpenID Connect discovery document on any host (/.well-known/openid-configuration returns 404). The anonymous WordPress REST API has no OAuth surface at all — reads need no credential and writes use WordPress application passwords.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cloud9 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cloud9 publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cloud9 API on a user''s behalf.


  Tokens are issued from https://cloud9.gg/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cloud9
provider_slug: cloud9
schemes:
- flows:
  - authorizationUrl: https://cloud9.gg/oauth/authorize
    client_authentication: none (public client)
    code_challenge_methods:
    - S256
    dynamic_client_registration: 'No RFC 7591 registration_endpoint is advertised. The server sets client_id_metadata_document_supported: true, so clients identify themselves with a client-ID metadata document URL rather than pre-registering.'
    flow: authorizationCode
    pkce: required
    refresh_tokens: true
    revocationUrl: https://cloud9.gg/oauth/revoke
    tokenUrl: https://cloud9.gg/oauth/token
  issuer: https://cloud9.gg
  name: Cloud9MCPOAuth
  source: https://cloud9.gg/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the Cloud9 MCP server at https://cloud9.gg/wp-json/mcp/mcp-oauth-server. Coarse, single-scope model — the authorization server advertises no finer-grained read/write split, so a token that can read content can also invoke any write ability the adapter registered.
  flows:
  - authorizationCode
  scope: mcp
slug: cloud9-scopes
source_filename: cloud9-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://cloud9.gg/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Cloud9's only OAuth surface is the authorization server advertised on cloud9.gg for its remote\n  MCP server. It declares a single coarse scope, `mcp`. Cloud9 publishes no developer program, no\n  scope or permission reference, and no OpenID Connect discovery document on any host\n  (/.well-known/openid-configuration returns 404). The anonymous WordPress REST API has no OAuth\n  surface at all — reads need no credential and writes use WordPress application passwords.\nschemes:\n- name: Cloud9MCPOAuth\n  type: oauth2\n  source: https://cloud9.gg/.well-known/oauth-authorization-server\n  issuer: https://cloud9.gg\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloud9.gg/oauth/authorize\n    tokenUrl: https://cloud9.gg/oauth/token\n    revocationUrl: https://cloud9.gg/oauth/revoke\n    pkce: required\n    code_challenge_methods:\
  \ [S256]\n    refresh_tokens: true\n    client_authentication: none (public client)\n    dynamic_client_registration: >-\n      No RFC 7591 registration_endpoint is advertised. The server sets\n      client_id_metadata_document_supported: true, so clients identify themselves with a\n      client-ID metadata document URL rather than pre-registering.\nscopes:\n- scope: mcp\n  description: >-\n    Access the Cloud9 MCP server at https://cloud9.gg/wp-json/mcp/mcp-oauth-server. Coarse,\n    single-scope model — the authorization server advertises no finer-grained read/write split,\n    so a token that can read content can also invoke any write ability the adapter registered.\n  flows: [authorizationCode]\n  sources: [https://cloud9.gg/.well-known/oauth-authorization-server]\n  protected_resource: https://cloud9.gg/wp-json/mcp/mcp-oauth-server\nnot_applicable:\n- surface: Cloud9 WordPress REST API (wp/v2)\n  reason: >-\n    No OAuth. Anonymous reads require no credential; writes are authenticated\
  \ with WordPress\n    application passwords issued at /wp-admin/authorize-application.php. There is no scope\n    surface to record — WordPress capabilities/roles do the authorization.\n- surface: Cloud9 Store JSON endpoints (Shopify)\n  reason: Anonymous platform endpoints. No authorization surface is exposed publicly.\nx-evidence:\n  fetched: '2026-08-09'\n  probes:\n  - url: https://cloud9.gg/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://cloud9.gg/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://cloud9.gg/.well-known/openid-configuration\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud9/refs/heads/main/scopes/cloud9-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Esports
- Gaming
- Entertainment
- Media
- Sports
- Content
- WordPress
- Community
- Merchandise
token_urls:
- https://cloud9.gg/oauth/token
---
