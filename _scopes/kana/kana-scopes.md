---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Kana Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kana uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kana
provider_slug: kana
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: kana-scopes
source_filename: kana-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://apps.kana.ai/.well-known/oauth-authorization-server\ndocs: null\nissuer: https://apps.kana.ai\nauthorization_url: https://apps.kana.ai/oauth/authorize\ntoken_url: https://apps.kana.ai/oauth/token\nscope_count: 4\nscopes:\n- name: mcp:read\n  description: >-\n    Read-level access to Kana's MCP surface. Verbatim from scopes_supported in the\n    authorization-server metadata; Kana publishes no scope-reference page, so no\n    per-scope description is available beyond the scope string itself.\n- name: mcp:write\n  description: >-\n    Write-level access to Kana's MCP surface. Verbatim from scopes_supported; no\n    published scope reference.\n- name: kana:read\n  description: >-\n    Read-level access to the Kana platform API. Verbatim from scopes_supported; no\n    published scope reference.\n- name: kana:write\n  description: >-\n    Write-level access to the Kana platform API. Verbatim from scopes_supported; no\n   \
  \ published scope reference.\nnotes: >-\n  These four strings are exactly what the provider advertises in scopes_supported.\n  The mcp:* / kana:* split is the only structure Kana publishes — it separates the\n  MCP agent surface from the platform surface. Nothing here is inferred or expanded:\n  Kana has no public scopes/permissions documentation page to enrich from, and every\n  other path on apps.kana.ai (including /.well-known/oauth-protected-resource, which\n  would name the resource each scope guards) returns 401.\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://apps.kana.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kana/refs/heads/main/scopes/kana-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Artificial Intelligence
- Agentic AI
- Marketing Technology
- Audience Intelligence
- Customer Data Platform
- AI Search Optimization
- Growth
token_urls: []
---
