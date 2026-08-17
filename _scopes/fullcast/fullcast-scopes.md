---
api_specs:
- filename: fullcast-assistant-openapi-original.json
  format: json
  label: Fullcast Assistant API
  slug: fullcast-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcast/refs/heads/main/openapi/fullcast-assistant-openapi-original.json
authorization_urls:
- https://assistant.fullcast.io/oauth/authorize
- https://app.fullcast.io/mcp/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Fullcast Scopes
name_suffix: OAuth Scopes
note: Fullcast's OpenAPI declares no oauth2 security scheme, so the mechanical derive pass found nothing. The scopes below were read directly from live RFC 8414 / RFC 9728 metadata on the MCP hosts, which is where Fullcast's real OAuth surface is described. No human-readable scopes reference page is published; descriptions below are the standard meaning of each registered scope, marked as such.
overview: 'Fullcast publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fullcast API on a user''s behalf.


  Tokens are issued from https://assistant.fullcast.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fullcast
provider_slug: fullcast
schemes:
- dynamic_client_registration: https://assistant.fullcast.io/oauth/register
  flows:
  - authorizationUrl: https://assistant.fullcast.io/oauth/authorize
    flow: authorizationCode
    pkce:
    - plain
    - S256
    tokenUrl: https://assistant.fullcast.io/oauth/token
    token_endpoint_auth_methods:
    - client_secret_post
    - none
    userinfoUrl: https://assistant.fullcast.io/oauth/userinfo
  issuer: https://assistant.fullcast.io
  name: Fullcast Assistant OAuth 2.1
  source: well-known/fullcast-assistant-oauth-authorization-server.json
- dynamic_client_registration: https://app.fullcast.io/mcp/register
  flows:
  - authorizationUrl: https://app.fullcast.io/mcp/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://app.fullcast.io/mcp/token
    token_endpoint_auth_methods:
    - client_secret_post
    - none
  issuer: https://app.fullcast.io/mcp
  name: Fullcast MCP OAuth 2.1
  note: this issuer advertises no scopes_supported in its metadata
  source: well-known/fullcast-app-mcp-oauth-authorization-server.json
scope_count: 7
scope_names:
- openid
- email
- profile
- offline_access
- mcp:tools
- mcp:resources
- mcp:prompts
scopes:
- description: OpenID Connect subject identifier (standard scope meaning; not provider-documented)
  flows:
  - authorizationCode
  scope: openid
- description: User email address (standard scope meaning; not provider-documented)
  flows:
  - authorizationCode
  scope: email
- description: Basic user profile claims (standard scope meaning; not provider-documented)
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token for long-lived agent sessions
  flows:
  - authorizationCode
  scope: offline_access
- description: Call MCP tools on the Fullcast Assistant MCP server
  flows:
  - authorizationCode
  scope: mcp:tools
- description: Read MCP resources (the fullcast://resource/* guidance documents)
  flows:
  - authorizationCode
  scope: mcp:resources
- description: Read MCP prompts exposed by the server
  flows:
  - authorizationCode
  scope: mcp:prompts
slug: fullcast-scopes
source_filename: fullcast-scopes.yml
source_heading: OAuth Scopes
source_url: https://assistant.fullcast.io/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://assistant.fullcast.io/.well-known/oauth-authorization-server\nsources:\n- https://assistant.fullcast.io/.well-known/oauth-authorization-server\n- https://assistant.fullcast.io/.well-known/oauth-protected-resource\n- https://app.fullcast.io/mcp/.well-known/oauth-authorization-server\nnote: >-\n  Fullcast's OpenAPI declares no oauth2 security scheme, so the mechanical derive pass found\n  nothing. The scopes below were read directly from live RFC 8414 / RFC 9728 metadata on the\n  MCP hosts, which is where Fullcast's real OAuth surface is described. No human-readable\n  scopes reference page is published; descriptions below are the standard meaning of each\n  registered scope, marked as such.\nschemes:\n- name: Fullcast Assistant OAuth 2.1\n  issuer: https://assistant.fullcast.io\n  source: well-known/fullcast-assistant-oauth-authorization-server.json\n  dynamic_client_registration: https://assistant.fullcast.io/oauth/register\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://assistant.fullcast.io/oauth/authorize\n    tokenUrl: https://assistant.fullcast.io/oauth/token\n    userinfoUrl: https://assistant.fullcast.io/oauth/userinfo\n    pkce: [plain, S256]\n    token_endpoint_auth_methods: [client_secret_post, none]\n- name: Fullcast MCP OAuth 2.1\n  issuer: https://app.fullcast.io/mcp\n  source: well-known/fullcast-app-mcp-oauth-authorization-server.json\n  dynamic_client_registration: https://app.fullcast.io/mcp/register\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.fullcast.io/mcp/authorize\n    tokenUrl: https://app.fullcast.io/mcp/token\n    pkce: [S256]\n    token_endpoint_auth_methods: [client_secret_post, none]\n  note: this issuer advertises no scopes_supported in its metadata\nscopes:\n- scope: openid\n  description: OpenID Connect subject identifier (standard scope meaning; not provider-documented)\n  flows: [authorizationCode]\n  sources: [https://assistant.fullcast.io/.well-known/oauth-authorization-server]\n\
  - scope: email\n  description: User email address (standard scope meaning; not provider-documented)\n  flows: [authorizationCode]\n  sources: [https://assistant.fullcast.io/.well-known/oauth-authorization-server]\n- scope: profile\n  description: Basic user profile claims (standard scope meaning; not provider-documented)\n  flows: [authorizationCode]\n  sources: [https://assistant.fullcast.io/.well-known/oauth-authorization-server]\n- scope: offline_access\n  description: Issue a refresh token for long-lived agent sessions\n  flows: [authorizationCode]\n  sources: [https://assistant.fullcast.io/.well-known/oauth-authorization-server]\n- scope: 'mcp:tools'\n  description: Call MCP tools on the Fullcast Assistant MCP server\n  flows: [authorizationCode]\n  sources: [https://assistant.fullcast.io/.well-known/oauth-protected-resource]\n- scope: 'mcp:resources'\n  description: Read MCP resources (the fullcast://resource/* guidance documents)\n  flows: [authorizationCode]\n  sources: [https://assistant.fullcast.io/.well-known/oauth-protected-resource]\n\
  - scope: 'mcp:prompts'\n  description: Read MCP prompts exposed by the server\n  flows: [authorizationCode]\n  sources: [https://assistant.fullcast.io/.well-known/oauth-protected-resource]\ngaps:\n- No scopes reference page is published for developers.\n- >-\n  Scopes are surface-level (mcp:tools covers all 17 verified tools), not capability-scoped.\n  There is no read-only scope, so an agent granted mcp:tools can call move_account and\n  end_coverage with the same token it uses to call get_account.\n- The app.fullcast.io/mcp issuer publishes no scopes_supported at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullcast/refs/heads/main/scopes/fullcast-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Enterprise
- Revenue Operations
- Sales Planning
- Territory Management
- Go-to-Market
- Incentive Compensation
- Forecasting
- Lead Routing
- MCP
- AI Agents
- Model Context Protocol
- Sales Compensation
token_urls:
- https://assistant.fullcast.io/oauth/token
- https://app.fullcast.io/mcp/token
---
