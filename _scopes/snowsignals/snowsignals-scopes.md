---
api_specs:
- filename: snowsignals-daas-openapi.json
  format: json
  label: SnowSignals API
  slug: snowsignals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowsignals/refs/heads/main/openapi/snowsignals-daas-openapi.json
- filename: snowsignals-x402-openapi.json
  format: json
  label: SnowSignals x402 Gateway
  slug: snowsignals-x402-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowsignals/refs/heads/main/openapi/snowsignals-x402-openapi.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Snowsignals Scopes
name_suffix: OAuth Scopes
note: The REST OpenAPI declares only apiKey schemes (url / nonce methods), so OAuth scopes are not in the spec — the OAuth surface belongs to the MCP endpoint. One scope exists. Public client with PKCE S256, dynamic client registration open at /v1/oauth/register, token endpoint auth method `none`.
overview: 'SnowSignals publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the SnowSignals API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SnowSignals
provider_slug: snowsignals
schemes: []
scope_count: 1
scope_names:
- daas:read
scopes:
- description: 'Read access to the metered/account MCP tools: get_phase, compose_phases (metered) and get_notifications, get_balance, get_usage, deposit_poll (free but account-bound). The two discovery tools (list_phase_meta, phase_resolution_stats) need no scope and no account.'
  flows: []
  scope: daas:read
slug: snowsignals-scopes
source_filename: snowsignals-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: >-\n  https://snowsignals.io/.well-known/oauth-authorization-server (RFC 8414, fetched 2026-09-10) and\n  https://snowsignals.io/.well-known/oauth-protected-resource (RFC 9728); per-tool auth requirements\n  read from the live MCP tools/list (mcp/snowsignals-mcp-tools-list.json).\nnote: >-\n  The REST OpenAPI declares only apiKey schemes (url / nonce methods), so OAuth scopes are not in the\n  spec — the OAuth surface belongs to the MCP endpoint. One scope exists. Public client with PKCE\n  S256, dynamic client registration open at /v1/oauth/register, token endpoint auth method `none`.\nauthorization_server: https://snowsignals.io\nauthorization_endpoint: https://snowsignals.io/oauth/authorize\ntoken_endpoint: https://snowsignals.io/v1/oauth/token\nregistration_endpoint: https://snowsignals.io/v1/oauth/register\nprotected_resource: https://snowsignals.io/mcp\nscopes:\n- scope: daas:read\n  description: >-\n    Read access to\
  \ the metered/account MCP tools: get_phase, compose_phases (metered) and\n    get_notifications, get_balance, get_usage, deposit_poll (free but account-bound). The two\n    discovery tools (list_phase_meta, phase_resolution_stats) need no scope and no account.\n  operations:\n  - get_phase\n  - compose_phases\n  - get_notifications\n  - get_balance\n  - get_usage\n  - deposit_poll\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snowsignals/refs/heads/main/scopes/snowsignals-scopes.yml
summary_line: 1 scope
tags:
- crypto
- market-data
- bitcoin
- analytics
- market-phase
- regime
- trendvane
- daas
- mcp
- agent-native
- financial-data
- x402
token_urls: []
---
