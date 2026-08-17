---
api_specs:
- filename: rocketreach-account-api-openapi.yml
  format: yaml
  label: RocketReach Account API
  slug: rocketreach-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-account-api-openapi.yml
- filename: rocketreach-company-data-api-api-openapi.yml
  format: yaml
  label: RocketReach Company Data API API
  slug: rocketreach-company-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-company-data-api-api-openapi.yml
- filename: rocketreach-people-data-api-api-openapi.yml
  format: yaml
  label: RocketReach People Data API API
  slug: rocketreach-people-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-people-data-api-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.rocketreach.co/reference/mcp-auth
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Rocketreach Scopes
name_suffix: OAuth Scopes
note: The RocketReach REST API is API-key authenticated and has no scope surface. OAuth exists solely for the RocketReach MCP server, and the scope list below is read verbatim from the provider's own RFC 8414 authorization-server metadata (scopes_supported), corroborated by the published Authentication page. It is a single coarse scope — there is no per-tool or read/write separation.
overview: 'RocketReach uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RocketReach
provider_slug: rocketreach
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rocketreach-scopes
source_filename: rocketreach-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://rocketreach.co/.well-known/oauth-authorization-server\ndocs: https://docs.rocketreach.co/reference/mcp-auth\nnote: >-\n  The RocketReach REST API is API-key authenticated and has no scope surface. OAuth exists solely for the\n  RocketReach MCP server, and the scope list below is read verbatim from the provider's own RFC 8414\n  authorization-server metadata (scopes_supported), corroborated by the published Authentication page. It is\n  a single coarse scope — there is no per-tool or read/write separation.\nauthorization_server: https://rocketreach.co\nprotected_resource: https://mcp.rocketreach.co\noauth_version: '2.1'\nflows:\n- type: authorization_code\n  pkce: S256\n  authorization_endpoint: https://rocketreach.co/mcp-oauth/authorize\n  token_endpoint: https://rocketreach.co/mcp-oauth/token\n- type: refresh_token\n  token_endpoint: https://rocketreach.co/mcp-oauth/token\ndynamic_client_registration:\n  supported: true\n\
  \  rfc: RFC 7591\n  endpoint: https://rocketreach.co/mcp-oauth/register\n  open: true\n  note: No pre-approval required. Redirect URIs are bound at registration; non-localhost redirects must be https.\ntoken_endpoint_auth_methods_supported:\n- none\nresponse_types_supported:\n- code\ngrant_types_supported:\n- authorization_code\n- refresh_token\ncode_challenge_methods_supported:\n- S256\nscopes:\n- name: rocketreach:read\n  description: >-\n    Grants access to all RocketReach MCP tools — person and company search, person and company lookup, and\n    account. Authorizing this single scope authorizes the whole tool set, including the three\n    credit-consuming lookup tools.\n  default: true\n  note: >-\n    An empty scope parameter on the authorize request defaults to rocketreach:read. Requesting any other\n    scope returns HTTP 400 invalid_scope.\nscope_count: 1\ngranularity: coarse\ngap: >-\n  There is no way for a user to authorize read-only search (free) without also authorizing the\n\
  \  credit-consuming lookup tools. A finer split — for example rocketreach:search versus rocketreach:enrich —\n  would let an agent be granted a spend-free capability. Worth raising with the provider.\nrevocation:\n  endpoint: https://rocketreach.co/mcp-oauth/revoke\n  note: Revoking a refresh token invalidates every access token issued from it.\nx-evidence:\n- url: https://rocketreach.co/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://mcp.rocketreach.co/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/scopes/rocketreach-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- B2B
- Contact Data
- Email Lookup
- Phone Lookup
- Sales Intelligence
- Lead Generation
- People Search
- Company Search
- Data Enrichment
- Prospecting
- Recruiting
- Webhooks
token_urls: []
---
