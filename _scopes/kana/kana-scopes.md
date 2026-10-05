---
authorization_urls:
- https://apps.kana.ai/oauth/authorize
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Kana Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kana publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kana API on a user''s behalf.


  Tokens are issued from https://apps.kana.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kana
provider_slug: kana
schemes: []
scope_count: 4
scope_names:
- mcp:read
- mcp:write
- kana:read
- kana:write
scopes:
- description: Read-level access to Kana's MCP surface. Verbatim from scopes_supported in the authorization-server metadata; Kana publishes no scope-reference page, so no per-scope description is available beyond the scope string itself.
  flows: []
  scope: mcp:read
- description: Write-level access to Kana's MCP surface. Verbatim from scopes_supported; no published scope reference.
  flows: []
  scope: mcp:write
- description: Read-level access to the Kana platform API. Verbatim from scopes_supported; no published scope reference.
  flows: []
  scope: kana:read
- description: Write-level access to the Kana platform API. Verbatim from scopes_supported; no published scope reference.
  flows: []
  scope: kana:write
slug: kana-scopes
source_filename: kana-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://apps.kana.ai/.well-known/oauth-authorization-server\ndocs: null\nissuer: https://apps.kana.ai\nauthorization_url: https://apps.kana.ai/oauth/authorize\ntoken_url: https://apps.kana.ai/oauth/token\nscope_count: 4\nscopes:\n- name: mcp:read\n  description: >-\n    Read-level access to Kana's MCP surface. Verbatim from scopes_supported in the\n    authorization-server metadata; Kana publishes no scope-reference page, so no\n    per-scope description is available beyond the scope string itself.\n- name: mcp:write\n  description: >-\n    Write-level access to Kana's MCP surface. Verbatim from scopes_supported; no\n    published scope reference.\n- name: kana:read\n  description: >-\n    Read-level access to the Kana platform API. Verbatim from scopes_supported; no\n    published scope reference.\n- name: kana:write\n  description: >-\n    Write-level access to the Kana platform API. Verbatim from scopes_supported; no\n   \
  \ published scope reference.\nnotes: >-\n  These four strings are exactly what the provider advertises in scopes_supported.\n  The mcp:* / kana:* split is the only structure Kana publishes — it separates the\n  MCP agent surface from the platform surface. Nothing here is inferred or expanded:\n  Kana has no public scopes/permissions documentation page to enrich from, and every\n  other path on apps.kana.ai (including /.well-known/oauth-protected-resource, which\n  would name the resource each scope guards) returns 401.\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://apps.kana.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kana/refs/heads/main/scopes/kana-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Marketing
- Artificial Intelligence
- AI Agents
- Marketing Technology
- Audience Intelligence
- Customer Data Platform
- AI Search Optimization
- Growth
token_bound: false
token_urls:
- https://apps.kana.ai/oauth/token
---
