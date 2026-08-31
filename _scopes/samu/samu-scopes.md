---
api_specs:
- filename: samu-meetings-api-openapi.yml
  format: yaml
  label: Samu Meetings API
  slug: samu-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/openapi/samu-meetings-api-openapi.yml
- filename: samu-threads-api-openapi.yml
  format: yaml
  label: Samu Threads API
  slug: samu-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/openapi/samu-threads-api-openapi.yml
- filename: samu-usuarios-api-openapi.yml
  format: yaml
  label: Samu Usuarios API
  slug: samu-usuarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/openapi/samu-usuarios-api-openapi.yml
authorization_urls:
- https://api.samu.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Samu Scopes
name_suffix: OAuth Scopes
note: Samu's OpenAPI declares only an apiKey scheme and has no oauth2 flows, so derive-oauth-scopes.py found nothing. The OAuth surface is real but lives entirely in the MCP authorization server metadata on api.samu.ai, which is served anonymously and is captured verbatim in well-known/. Samu publishes no human-readable scope reference page.
overview: 'Samu publishes 1 OAuth 2.0 scope via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Samu API on a user''s behalf.


  Tokens are issued from https://api.samu.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Samu
provider_slug: samu
schemes:
- code_challenge_methods:
  - S256
  dynamic_client_registration: https://api.samu.ai/oauth/register
  flows:
  - authorizationUrl: https://api.samu.ai/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://api.samu.ai/oauth/revoke
    tokenUrl: https://api.samu.ai/oauth/token
  - flow: refreshToken
    tokenUrl: https://api.samu.ai/oauth/token
  issuer: https://api.samu.ai
  name: MCP OAuth 2.1
  protected_resource: https://api.samu.ai/mcp
  source: well-known/samu-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - none
scope_count: 1
scope_names:
- mcp:read
scopes:
- description: The only scope advertised in scopes_supported. Read access for MCP clients to the Samu MCP server. Samu publishes no per-scope description; this is the scope string verbatim from the authorization-server metadata.
  flows:
  - authorizationCode
  scope: mcp:read
slug: samu-scopes
source_filename: samu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.samu.ai/.well-known/oauth-authorization-server\nnote: >-\n  Samu's OpenAPI declares only an apiKey scheme and has no oauth2 flows, so\n  derive-oauth-scopes.py found nothing. The OAuth surface is real but lives\n  entirely in the MCP authorization server metadata on api.samu.ai, which is\n  served anonymously and is captured verbatim in well-known/. Samu publishes no\n  human-readable scope reference page.\nschemes:\n- name: MCP OAuth 2.1\n  source: well-known/samu-oauth-authorization-server.json\n  issuer: https://api.samu.ai\n  protected_resource: https://api.samu.ai/mcp\n  dynamic_client_registration: https://api.samu.ai/oauth/register\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.samu.ai/oauth/authorize\n    tokenUrl: https://api.samu.ai/oauth/token\n    revocationUrl: https://api.samu.ai/oauth/revoke\n  - flow:\
  \ refreshToken\n    tokenUrl: https://api.samu.ai/oauth/token\nscopes:\n- scope: mcp:read\n  description: >-\n    The only scope advertised in scopes_supported. Read access for MCP clients to\n    the Samu MCP server. Samu publishes no per-scope description; this is the\n    scope string verbatim from the authorization-server metadata.\n  flows: [authorizationCode]\n  sources: [well-known/samu-oauth-authorization-server.json]\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://api.samu.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/scopes/samu-scopes.yml
summary_line: 1 scope · authorizationCode/refreshToken
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Intelligence
- Conversation Intelligence
- CRM
- Call Recording
- Analytics
- Latin America
- Transcription
- WhatsApp
- MCP
- Agent Native
token_urls:
- https://api.samu.ai/oauth/token
---
