---
api_specs:
- filename: clay-com-me-api-openapi.yml
  format: yaml
  label: Clay Me API
  slug: clay-com-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/openapi/clay-com-me-api-openapi.yml
- filename: clay-com-routines-api-openapi.yml
  format: yaml
  label: Clay Routines API
  slug: clay-com-routines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/openapi/clay-com-routines-api-openapi.yml
- filename: clay-com-search-api-openapi.yml
  format: yaml
  label: Clay Search API
  slug: clay-com-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/openapi/clay-com-search-api-openapi.yml
- filename: clay-com-tables-api-openapi.yml
  format: yaml
  label: Clay Tables API
  slug: clay-com-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/openapi/clay-com-tables-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.clay.com/concepts/cli-basics
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Clay Com Scopes
name_suffix: OAuth Scopes
note: Clay's OpenAPI declares NO oauth2 security scheme — the Public API is api-key only (`clay-api-key` header), so derive-oauth-scopes.py correctly found nothing in the spec. But Clay does run a real OAuth 2.0 authorization server, published as RFC 8414 metadata at https://api.clay.com/.well-known/oauth-authorization-server, and it is what gates the `clay` CLI and the remote MCP server at https://api.clay.com/v3/mcp. The scope surface below is read verbatim from that metadata document, not inferred.
overview: 'Clay publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clay API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clay
provider_slug: clay-com
schemes: []
scope_count: 1
scope_names:
- mcp
scopes:
- description: The single scope Clay's authorization server advertises. It gates the whole MCP surface — search, routines and tables alike — as one grant.
  flows:
  - authorizationCode
  - deviceCode
  scope: mcp
slug: clay-com-scopes
source_filename: clay-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://api.clay.com/.well-known/oauth-authorization-server\ndocs: https://developers.clay.com/concepts/cli-basics\nnote: >-\n  Clay's OpenAPI declares NO oauth2 security scheme — the Public API is api-key only\n  (`clay-api-key` header), so derive-oauth-scopes.py correctly found nothing in the spec.\n  But Clay does run a real OAuth 2.0 authorization server, published as RFC 8414 metadata\n  at https://api.clay.com/.well-known/oauth-authorization-server, and it is what gates the\n  `clay` CLI and the remote MCP server at https://api.clay.com/v3/mcp. The scope surface\n  below is read verbatim from that metadata document, not inferred.\napplies_to:\n- surface: MCP server\n  url: https://api.clay.com/v3/mcp\n- surface: clay CLI\n  command: clay login\ndoes_not_apply_to:\n- surface: Public API\n  url: https://api.clay.com/public/v0\n  auth: apiKey header clay-api-key\nauthorization_server:\n  issuer: https://api.clay.com\n  authorization_endpoint:\
  \ https://app.clay.com/oauth/authorize\n  token_endpoint: https://api.clay.com/oauth/token\n  device_authorization_endpoint: https://api.clay.com/oauth/device_authorization\n  registration_endpoint: https://api.clay.com/oauth/register\n  revocation_endpoint: https://api.clay.com/oauth/revoke\n  metadata_file: well-known/clay-com-oauth-authorization-server.json\nflows:\n- flow: authorizationCode\n  authorizationUrl: https://app.clay.com/oauth/authorize\n  tokenUrl: https://api.clay.com/oauth/token\n  pkce: [S256]\n- flow: deviceCode\n  grant_type: 'urn:ietf:params:oauth:grant-type:device_code'\n  deviceAuthorizationUrl: https://api.clay.com/oauth/device_authorization\n  note: Used by `clay login --device` on headless machines.\n- flow: refreshToken\n  grant_type: refresh_token\nscopes:\n- scope: mcp\n  description: >-\n    The single scope Clay's authorization server advertises. It gates the whole MCP\n    surface — search, routines and tables alike — as one grant.\n  flows: [authorizationCode,\
  \ deviceCode]\n  sources: [well-known/clay-com-oauth-authorization-server.json]\n  resource: https://api.clay.com/v3/mcp\nscope_count: 1\nprotected_resources:\n- resource: https://api.clay.com/v3/mcp\n  authorization_servers: [https://api.clay.com]\n  scopes_supported: [mcp]\n  metadata: well-known/clay-com-oauth-protected-resource.json\n  discovery: >-\n    Advertised in the WWW-Authenticate header on an unauthenticated POST:\n    Bearer resource_metadata=\"https://api.clay.com/.well-known/oauth-protected-resource/v3/mcp\"\nobservations:\n  granularity: coarse\n  note: >-\n    One scope for the entire agent surface means consent is all-or-nothing: an agent\n    authorized to read a search is equally authorized to run credit-consuming enrichment\n    routines and, on Enterprise, to query customer tables. There is no read-only scope and\n    no per-primitive scope. Worth flagging to the provider.\n  strengths:\n  - RFC 8414 authorization-server metadata published and reachable anonymously\n\
  \  - RFC 9728 protected-resource metadata published, correctly linked from WWW-Authenticate\n  - PKCE S256 supported\n  - dynamic client registration supported (RFC 7591)\n  - device-code grant supported for headless agents\n  - token revocation endpoint published\n  gaps:\n  - no openid-configuration (Clay is an OAuth authorization server, not an OIDC provider)\n  - single coarse scope; no least-privilege option\n  - the Public API sits outside this model entirely, on long-lived api keys with no scoping\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/scopes/clay-com-scopes.yml
summary_line: 1 scope
tags:
- Prospecting
- Go-To-Market
- Sales
- Enrichment
- Automation
- Artificial Intelligence
- Webhook
token_urls: []
---
