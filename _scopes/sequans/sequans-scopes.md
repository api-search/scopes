---
authorization_urls:
- https://sequans.com/oauth/authorize
description: Sequans' only OAuth surface is the authorization server the WordPress MCP Adapter advertises on sequans.com for its remote MCP server. It declares a single coarse scope, `mcp`. Sequans publishes no scope or permission reference and no OpenID Connect discovery document.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Sequans Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sequans publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sequans API on a user''s behalf.


  Tokens are issued from https://sequans.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sequans
provider_slug: sequans
schemes:
- flows:
  - authorizationUrl: https://sequans.com/oauth/authorize
    client_authentication: none (public client)
    code_challenge_methods:
    - S256
    dynamic_client_registration: No RFC 7591 registration_endpoint is advertised; client_id_metadata_document_supported is true, so clients identify themselves with a client-ID metadata document URL.
    flow: authorizationCode
    pkce: required
    refresh_tokens: true
    revocationUrl: https://sequans.com/oauth/revoke
    tokenUrl: https://sequans.com/oauth/token
  issuer: https://sequans.com
  name: SequansMCPOAuth
  source: https://sequans.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the Sequans website MCP server at https://sequans.com/wp-json/mcp/mcp-oauth-server. Single-scope model; no finer read/write split is advertised.
  flows:
  - authorizationCode
  scope: mcp
slug: sequans-scopes
source_filename: sequans-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: https://sequans.com/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Sequans' only OAuth surface is the authorization server the WordPress MCP Adapter advertises on\n  sequans.com for its remote MCP server. It declares a single coarse scope, `mcp`. Sequans publishes\n  no scope or permission reference and no OpenID Connect discovery document.\nschemes:\n- name: SequansMCPOAuth\n  type: oauth2\n  source: https://sequans.com/.well-known/oauth-authorization-server\n  issuer: https://sequans.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sequans.com/oauth/authorize\n    tokenUrl: https://sequans.com/oauth/token\n    revocationUrl: https://sequans.com/oauth/revoke\n    pkce: required\n    code_challenge_methods: [S256]\n    refresh_tokens: true\n    client_authentication: none (public client)\n    dynamic_client_registration: >-\n      No RFC 7591 registration_endpoint is advertised;\
  \ client_id_metadata_document_supported is\n      true, so clients identify themselves with a client-ID metadata document URL.\nscopes:\n- scope: mcp\n  description: >-\n    Access the Sequans website MCP server at https://sequans.com/wp-json/mcp/mcp-oauth-server.\n    Single-scope model; no finer read/write split is advertised.\n  flows: [authorizationCode]\n  sources: [https://sequans.com/.well-known/oauth-authorization-server, https://sequans.com/.well-known/oauth-protected-resource]\n  protected_resource: https://sequans.com/wp-json/mcp/mcp-oauth-server\nx-evidence:\n  fetched: '2026-09-16'\n  probes:\n  - url: https://sequans.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://sequans.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://sequans.com/.well-known/openid-configuration\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequans/refs/heads/main/scopes/sequans-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Semiconductors
- Cellular IoT
- 5G
- LTE-M
- NB-IoT
- IoT Modules
- Hardware
- Telecommunications
- France
token_urls:
- https://sequans.com/oauth/token
---
