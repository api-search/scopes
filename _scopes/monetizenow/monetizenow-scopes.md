---
api_specs:
- filename: monetizenow-openapi.json
  format: json
  label: MonetizeNow API
  slug: monetizenow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetizenow/refs/heads/main/openapi/monetizenow-openapi.json
authorization_urls:
- https://mcp.monetizeplatform.com/oauth/authorize
description: 'MonetizeNow runs one OAuth 2.x authorization server — the one protecting its hosted MCP server at mcp.monetizeplatform.com. Its RFC 8414 and RFC 9728 discovery documents are public and were read directly. Both declare `scopes_supported: []`. That is the finding: the authorization server exists, supports dynamic client registration and PKCE S256, and publishes NO scope vocabulary at all, so a client cannot request least privilege and a resource owner cannot see what an agent is being granted. The REST API (api.monetizeplatform.com) is not OAuth-protected at all — it uses a single tenant-wide x-api-key with no scoping, so it contributes no scopes either.'
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Monetizenow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MonetizeNow uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://mcp.monetizeplatform.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MonetizeNow
provider_slug: monetizenow
schemes:
- dynamic_client_registration: https://mcp.monetizeplatform.com/oauth/register
  flows:
  - authorizationUrl: https://mcp.monetizeplatform.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    scopes: {}
    tokenUrl: https://mcp.monetizeplatform.com/oauth/token
    token_endpoint_auth_methods:
    - none
  issuer: https://mcp.monetizeplatform.com
  name: MonetizeNow MCP OAuth
  protects: https://mcp.monetizeplatform.com/mcp
  refresh: true
  source: https://mcp.monetizeplatform.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 0
scope_names: []
scopes: []
slug: monetizenow-scopes
source_filename: monetizenow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.monetizeplatform.com/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  MonetizeNow runs one OAuth 2.x authorization server — the one protecting its\n  hosted MCP server at mcp.monetizeplatform.com. Its RFC 8414 and RFC 9728\n  discovery documents are public and were read directly. Both declare\n  `scopes_supported: []`. That is the finding: the authorization server exists,\n  supports dynamic client registration and PKCE S256, and publishes NO scope\n  vocabulary at all, so a client cannot request least privilege and a resource\n  owner cannot see what an agent is being granted. The REST API\n  (api.monetizeplatform.com) is not OAuth-protected at all — it uses a single\n  tenant-wide x-api-key with no scoping, so it contributes no scopes either.\nschemes:\n- name: MonetizeNow MCP OAuth\n  type: oauth2\n  source: https://mcp.monetizeplatform.com/.well-known/oauth-authorization-server\n  issuer:\
  \ https://mcp.monetizeplatform.com\n  protects: https://mcp.monetizeplatform.com/mcp\n  dynamic_client_registration: https://mcp.monetizeplatform.com/oauth/register\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.monetizeplatform.com/oauth/authorize\n    tokenUrl: https://mcp.monetizeplatform.com/oauth/token\n    pkce: S256\n    token_endpoint_auth_methods: [none]\n    scopes: {}\n  refresh: true\nscope_count: 0\nscopes: []\nnon_oauth_surfaces:\n- name: MonetizeNow REST API\n  base_url: https://api.monetizeplatform.com\n  auth: apiKey (x-api-key header)\n  scoped: false\n  note: >-\n    One tenant-generated key authenticates all MonetizeNow REST APIs. No scopes,\n    no per-resource permissions, no read-only key type is documented. See\n    authentication/monetizenow-authentication.yml.\nevidence:\n- {url: 'https://mcp.monetizeplatform.com/.well-known/oauth-authorization-server', status: 200, fetched: '2026-08-13'}\n- {url: 'https://mcp.monetizeplatform.com/.well-known/oauth-protected-resource',\
  \ status: 200, fetched: '2026-08-13'}\nnotes:\n- >-\n  No scopes/permissions reference page exists in the MonetizeNow documentation;\n  the MCP server is not documented publicly at all.\n- >-\n  RECOMMENDATION TO THE PROVIDER: publish a scope vocabulary (at minimum\n  read/write splits per domain — quotes, contracts, billing, usage) in\n  scopes_supported. An empty scopes_supported on an agent-facing MCP server means\n  every authorized agent gets whatever the token carries, unbounded.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monetizenow/refs/heads/main/scopes/monetizenow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Monetization
- Billing
- Subscription
- Usage-Based Pricing
- Quote-to-Cash
- CPQ
- Payments
- Invoicing
- Revenue
- Software-as-a-Service
- Fintech
token_urls:
- https://mcp.monetizeplatform.com/oauth/token
---
