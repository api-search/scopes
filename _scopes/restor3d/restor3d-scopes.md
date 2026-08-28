---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Restor3D Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'restor3d uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: restor3d
provider_slug: restor3d
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: restor3d-scopes
source_filename: restor3d-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  scopes_supported in https://www.restor3d.com/.well-known/oauth-authorization-server (HTTP 200)\n  and https://www.restor3d.com/.well-known/oauth-protected-resource (HTTP 200), fetched\n  2026-08-26. No scope reference page exists to enrich from - restor3d publishes no developer\n  documentation.\napi: restor3d Website Content API (WordPress REST + MCP)\ndocs: null\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The single scope the authorization server advertises. It gates the Model Context Protocol\n    resource https://www.restor3d.com/wp-json/mcp/mcp-oauth-server. The metadata documents publish\n    no finer-grained scopes and no per-tool or per-content-type scoping; what a granted `mcp` token\n    is actually permitted to do cannot be determined without an authenticated session, and is not\n    asserted here.\n  resource: https://www.restor3d.com/wp-json/mcp/mcp-oauth-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restor3d/refs/heads/main/scopes/restor3d-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Medical Devices
- Health
- Orthopedics
- 3D Printing
- Additive Manufacturing
- Implants
- Surgery
- Artificial Intelligence
- Manufacturing
- Company
token_urls: []
---
