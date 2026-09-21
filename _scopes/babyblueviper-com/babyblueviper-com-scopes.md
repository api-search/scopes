---
api_specs:
- filename: babyblueviper-com-openapi.yml
  format: yaml
  label: invinoveritas API
  slug: invinoveritas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babyblueviper-com/refs/heads/main/openapi/babyblueviper-com-openapi.yml
authorization_urls:
- https://api.babyblueviper.com/oauth/authorize
description: ''
docs: https://api.babyblueviper.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Babyblueviper Com Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no oauth2 securityScheme, so derive-oauth-scopes.py found nothing. The provider's OAuth 2.1 surface exists for the MCP resource only and is documented by its RFC 8414 / RFC 9728 metadata, which is the source here. Exactly one scope is published. No human scopes/permissions reference page was found; the metadata is the reference.
overview: 'invinoveritas publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the invinoveritas API on a user''s behalf.


  Tokens are issued from https://api.babyblueviper.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: invinoveritas
provider_slug: babyblueviper-com
schemes:
- flows:
  - authorizationUrl: https://api.babyblueviper.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    refresh_token: true
    registration_endpoint: https://api.babyblueviper.com/oauth/register
    tokenUrl: https://api.babyblueviper.com/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_post
  issuer: https://api.babyblueviper.com
  name: OAuth 2.1 (MCP resource)
  resource: https://api.babyblueviper.com/mcp
  source: https://api.babyblueviper.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access to the invinoveritas MCP server at https://api.babyblueviper.com/mcp (the only scope listed in scopes_supported of both the authorization-server and protected-resource metadata).
  flows:
  - authorizationCode
  scope: mcp
slug: babyblueviper-com-scopes
source_filename: babyblueviper-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.babyblueviper.com/.well-known/oauth-authorization-server\ndocs: https://api.babyblueviper.com/.well-known/oauth-protected-resource\nnote: >-\n  The OpenAPI declares no oauth2 securityScheme, so derive-oauth-scopes.py found nothing. The provider's OAuth\n  2.1 surface exists for the MCP resource only and is documented by its RFC 8414 / RFC 9728 metadata, which is\n  the source here. Exactly one scope is published. No human scopes/permissions reference page was found; the\n  metadata is the reference.\nschemes:\n- name: OAuth 2.1 (MCP resource)\n  source: https://api.babyblueviper.com/.well-known/oauth-authorization-server\n  issuer: https://api.babyblueviper.com\n  resource: https://api.babyblueviper.com/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.babyblueviper.com/oauth/authorize\n    tokenUrl: https://api.babyblueviper.com/oauth/token\n    refresh_token: true\n    code_challenge_methods:\
  \ [S256]\n    registration_endpoint: https://api.babyblueviper.com/oauth/register\n    token_endpoint_auth_methods: [none, client_secret_post]\nscopes:\n- scope: mcp\n  description: Access to the invinoveritas MCP server at https://api.babyblueviper.com/mcp (the only scope listed in scopes_supported of both the authorization-server and protected-resource metadata).\n  flows: [authorizationCode]\n  sources: [https://api.babyblueviper.com/.well-known/oauth-authorization-server, https://api.babyblueviper.com/.well-known/oauth-protected-resource]\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/babyblueviper-com/refs/heads/main/scopes/babyblueviper-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- AI Agents
- Agent Verification
- Agent Governance
- MCP
- A2A
- Bitcoin Lightning
- x402
- Trading
- Cryptographic Proofs
- Agent Marketplace
token_urls:
- https://api.babyblueviper.com/oauth/token
---
