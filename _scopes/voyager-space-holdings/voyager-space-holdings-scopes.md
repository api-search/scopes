---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Voyager Space Holdings Scopes
name_suffix: OAuth Scopes
note: Read verbatim from scopes_supported in the provider's RFC 8414 metadata and confirmed by the RFC 9728 protected-resource document (both HTTP 200, 2026-09-18). The single scope belongs to the WordPress MCP adapter's authorization server; there is no product API, no scopes reference page and no finer-grained permission model published.
overview: 'Voyager Technologies uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Voyager Technologies
provider_slug: voyager-space-holdings
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: voyager-space-holdings-scopes
source_filename: voyager-space-holdings-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://voyagertechnologies.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Read verbatim from scopes_supported in the provider's RFC 8414 metadata and confirmed by the RFC\n  9728 protected-resource document (both HTTP 200, 2026-09-18). The single scope belongs to the\n  WordPress MCP adapter's authorization server; there is no product API, no scopes reference page\n  and no finer-grained permission model published.\nscheme: mcpOAuth2\nflows:\n- authorizationCode\nscope_count: 1\nscopes:\n- name: mcp\n  description: Access the site's Model Context Protocol server (https://voyagertechnologies.com/wp-json/mcp/mcp-oauth-server).\n  resource: https://voyagertechnologies.com/wp-json/mcp/mcp-oauth-server\n  sources:\n  - https://voyagertechnologies.com/.well-known/oauth-authorization-server\n  - https://voyagertechnologies.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyager-space-holdings/refs/heads/main/scopes/voyager-space-holdings-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Space
- Defense
- Aerospace
- Propulsion
- Satellite
- Lunar
- Space Stations
- Public Company
token_urls: []
---
