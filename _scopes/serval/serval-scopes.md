---
api_specs:
- filename: serval-auth-openapi.yml
  format: yaml
  label: Serval Public API
  slug: serval-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serval/refs/heads/main/openapi/serval-auth-openapi.yml
authorization_urls:
- https://public.api.serval.com/oauth/authorize
description: ''
docs: https://docs.serval.com/sections/documentation/end-user/mcp-quickstart
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Serval Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Serval publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Serval API on a user''s behalf.


  Tokens are issued from https://public.api.serval.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Serval
provider_slug: serval
schemes:
- flows:
  - authorizationUrl: https://public.api.serval.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://public.api.serval.com/oauth/token
  name: OAuth2
  source: well-known/serval-oauth-authorization-server.json
scope_count: 1
scope_names:
- serval:user
scopes:
- description: 'Act on behalf of an authenticated Serval user through the OAuth authorization server (the scope requested by the hosted MCP server / delegated agent clients). This is the only scope advertised in the RFC 8414 authorization-server metadata (scopes_supported: ["serval:user"]).'
  flows:
  - authorizationCode
  scope: serval:user
slug: serval-scopes
source_filename: serval-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://public.api.serval.com/.well-known/oauth-authorization-server\ndocs: https://docs.serval.com/sections/documentation/end-user/mcp-quickstart\nschemes:\n  - name: OAuth2\n    source: well-known/serval-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://public.api.serval.com/oauth/authorize\n        tokenUrl: https://public.api.serval.com/oauth/token\n        pkce: S256\nscopes:\n  - scope: serval:user\n    description: >\n      Act on behalf of an authenticated Serval user through the OAuth authorization server\n      (the scope requested by the hosted MCP server / delegated agent clients). This is the\n      only scope advertised in the RFC 8414 authorization-server metadata\n      (scopes_supported: [\"serval:user\"]).\n    flows: [authorizationCode]\n    sources: [well-known/serval-oauth-authorization-server.json]\nnotes: >\n  Serval's public REST API (/v2/*)\
  \ does not use OAuth scopes — it uses a Basic\n  client_id:client_secret -> Bearer token exchange (see authentication/). The scope\n  surface here belongs to the separate OAuth 2.0 authorization server used by the MCP\n  server and interactive agent clients. Per-team API access is scoped by the admin at\n  integration setup time rather than via OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serval/refs/heads/main/scopes/serval-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- IT Service Management
- ITSM
- Help Desk
- Workflow Automation
- AI Agents
- Access Management
- Employee Support
- Ticketing
token_urls:
- https://public.api.serval.com/oauth/token
---
