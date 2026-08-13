---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Valid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Valid uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Valid
provider_slug: valid
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: valid-scopes
source_filename: valid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  scopes_supported in https://mcp.valid.co/.well-known/oauth-authorization-server\n  and https://mcp.valid.co/.well-known/oauth-protected-resource (both HTTP 200,\n  fetched 2026-08-12).\ndocs: null\ndocs_note: >-\n  Valid publishes no scopes or permissions reference page. These three scopes are\n  taken verbatim from the server's own metadata; the descriptions below are the\n  standard OpenID Connect meanings of those scope names, not provider text.\napi: Valid Chat With Your Ads MCP Server\nauthorization_server: https://mcp.valid.co\nscope_count: 3\nscopes:\n- name: openid\n  description: Request an OpenID Connect subject identifier for the authenticated user.\n  standard: OpenID Connect Core 1.0\n  provider_described: false\n- name: email\n  description: Access the authenticated user's email address.\n  standard: OpenID Connect Core 1.0\n  provider_described: false\n- name: profile\n  description: Access basic profile\
  \ claims for the authenticated user.\n  standard: OpenID Connect Core 1.0\n  provider_described: false\nnotes: >-\n  All three advertised scopes are identity scopes. Valid publishes NO resource\n  scopes — nothing like ads:read, spend:read, campaigns:write — even though the\n  server's stated purpose is querying an advertising account. Authorization to the\n  underlying ad data is therefore not expressed in the OAuth scope layer at all; it\n  is presumably bound to the client account behind the token. For an agent surface\n  this matters: a consenting user cannot grant an agent read-only access to spend\n  data, because no scope exists to describe that. Recording the gap is the finding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valid/refs/heads/main/scopes/valid-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- Marketing
- Artificial Intelligence
- Creative
- Media Buying
- Influencers
- MCP
- Agents
- Performance Marketing
token_urls: []
---
