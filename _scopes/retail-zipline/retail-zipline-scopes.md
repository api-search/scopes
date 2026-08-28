---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Retail Zipline Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Retail Zipline uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Retail Zipline
provider_slug: retail-zipline
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: retail-zipline-scopes
source_filename: retail-zipline-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://getzipline.com/.well-known/oauth-authorization-server\nsummary: >-\n  Zipline's authorization server advertises exactly one OAuth scope. There is no\n  published scope or permissions reference page — this list is read directly from\n  the RFC 8414 metadata document and the RFC 9728 protected-resource document,\n  which agree.\nauthorization_server: https://getzipline.com\ndocs: null\ndocs_note: No public scopes/permissions reference page exists on any Zipline host.\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Grants an MCP client access to the Zipline MCP server at\n    https://getzipline.com/wp-json/mcp/mcp-oauth-server. The provider publishes\n    no finer-grained breakdown of what the scope authorizes; it is a single\n    coarse scope covering the whole resource.\n  source: scopes_supported in both the authorization-server and protected-resource metadata\nx-evidence:\n- url: https://getzipline.com/.well-known/oauth-authorization-server\n\
  \  http_status: 200\n  fetched: '2026-08-26'\n- url: https://getzipline.com/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retail-zipline/refs/heads/main/scopes/retail-zipline-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Retail
- Retail Operations
- Task Management
- Employee Communications
- Store Operations
- Workforce
- Knowledge Base
- SaaS
- MCP
- Company
token_urls: []
---
