---
authorization_urls:
- https://home.quakerhoughton.com/oauth/authorize
description: Quaker Houghton's only public OAuth surface is the authorization server advertised on home.quakerhoughton.com for its remote MCP server. It declares a single coarse scope, `mcp`. There is no scope or permission reference anywhere on the site, and no other Quaker Houghton host publishes RFC 8414 or OIDC discovery metadata. The Events Calendar REST APIs on the same host have no OAuth surface at all — their reads are anonymous and their writes declare HTTP Basic (WordPress Application Passwords).
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Quaker Houghton Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Quaker Houghton publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Quaker Houghton API on a user''s behalf.


  Tokens are issued from https://home.quakerhoughton.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Quaker Houghton
provider_slug: quaker-houghton
schemes:
- flows:
  - authorizationUrl: https://home.quakerhoughton.com/oauth/authorize
    client_authentication: none (public client)
    code_challenge_methods:
    - S256
    dynamic_client_registration: 'No RFC 7591 registration_endpoint. The server advertises client_id_metadata_document_supported: true, so clients identify themselves with a client-ID metadata document URL rather than pre-registering.'
    flow: authorizationCode
    pkce: required
    refresh_tokens: true
    revocationUrl: https://home.quakerhoughton.com/oauth/revoke
    tokenUrl: https://home.quakerhoughton.com/oauth/token
  issuer: https://home.quakerhoughton.com
  name: QuakerHoughtonMCPOAuth
  source: https://home.quakerhoughton.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the MCP server at https://home.quakerhoughton.com/wp-json/mcp/mcp-oauth-server. Coarse, single-scope model — the authorization server advertises no finer-grained read/write split.
  flows:
  - authorizationCode
  scope: mcp
slug: quaker-houghton-scopes
source_filename: quaker-houghton-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: https://home.quakerhoughton.com/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Quaker Houghton's only public OAuth surface is the authorization server advertised on\n  home.quakerhoughton.com for its remote MCP server. It declares a single coarse scope, `mcp`.\n  There is no scope or permission reference anywhere on the site, and no other Quaker Houghton\n  host publishes RFC 8414 or OIDC discovery metadata. The Events Calendar REST APIs on the same\n  host have no OAuth surface at all — their reads are anonymous and their writes declare HTTP\n  Basic (WordPress Application Passwords).\nschemes:\n- name: QuakerHoughtonMCPOAuth\n  type: oauth2\n  source: https://home.quakerhoughton.com/.well-known/oauth-authorization-server\n  issuer: https://home.quakerhoughton.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://home.quakerhoughton.com/oauth/authorize\n    tokenUrl: https://home.quakerhoughton.com/oauth/token\n\
  \    revocationUrl: https://home.quakerhoughton.com/oauth/revoke\n    pkce: required\n    code_challenge_methods: [S256]\n    refresh_tokens: true\n    client_authentication: none (public client)\n    dynamic_client_registration: >-\n      No RFC 7591 registration_endpoint. The server advertises\n      client_id_metadata_document_supported: true, so clients identify themselves with a\n      client-ID metadata document URL rather than pre-registering.\nscopes:\n- scope: mcp\n  description: >-\n    Access the MCP server at https://home.quakerhoughton.com/wp-json/mcp/mcp-oauth-server.\n    Coarse, single-scope model — the authorization server advertises no finer-grained\n    read/write split.\n  flows: [authorizationCode]\n  sources: [https://home.quakerhoughton.com/.well-known/oauth-authorization-server]\n  protected_resource: https://home.quakerhoughton.com/wp-json/mcp/mcp-oauth-server\nnot_applicable:\n- surface: Events Calendar REST APIs (tribe/events/v1, tec/v1)\n  reason: No oauth2\
  \ securityScheme; reads are anonymous, writes declare HTTP Basic.\nx-evidence:\n  fetched: '2026-09-17'\n  probes:\n  - url: https://home.quakerhoughton.com/.well-known/oauth-authorization-server/\n    status: 200\n  - url: https://home.quakerhoughton.com/.well-known/oauth-protected-resource/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quaker-houghton/refs/heads/main/scopes/quaker-houghton-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Industrial Fluids
- Chemicals
- Manufacturing
- Metalworking
- Lubricants
- Event
- MCP
token_urls:
- https://home.quakerhoughton.com/oauth/token
---
