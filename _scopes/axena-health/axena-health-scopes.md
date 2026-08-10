---
authorization_urls: []
description: One scope, and it is the whole surface. The OAuth Authorization Server Metadata document on levacares.com declares a single supported scope, `mcp`, which the Protected Resource Metadata document binds to the WordPress MCP Adapter endpoint. There is no scope reference page to search — Axena Health publishes no developer documentation — so nothing beyond what the discovery documents themselves assert is recorded here.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Axena Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Axena Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Axena Health
provider_slug: axena-health
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: axena-health-scopes
source_filename: axena-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://levacares.com/.well-known/oauth-authorization-server\nname: Axena Health — OAuth scopes\ndescription: >-\n  One scope, and it is the whole surface. The OAuth Authorization Server\n  Metadata document on levacares.com declares a single supported scope, `mcp`,\n  which the Protected Resource Metadata document binds to the WordPress MCP\n  Adapter endpoint. There is no scope reference page to search — Axena Health\n  publishes no developer documentation — so nothing beyond what the discovery\n  documents themselves assert is recorded here.\ndocs: null\nauthorization_server: https://levacares.com\nresource: https://levacares.com/wp-json/mcp/mcp-oauth-server\n\nscopes:\n- name: mcp\n  description: >-\n    Granted access to the WordPress MCP Adapter endpoint at\n    https://levacares.com/wp-json/mcp/mcp-oauth-server. The adapter does not\n    subdivide this scope; it is coarse-grained and covers whatever abilities the\n   \
  \ site has registered under the wp-abilities/v1 namespace. Those abilities\n    could not be enumerated anonymously (tools/list returns 401), so the real\n    consequence of granting this scope is not publicly knowable.\n  source: scopes_supported\n  granularity: coarse\n\nx-gap: >-\n  A single coarse scope over an unenumerable tool set is the pattern this\n  catalog flags: a consenting user cannot see what they are consenting to. The\n  fix is the provider's — register named abilities and publish the tool\n  manifest, or narrow the scope.\n\nx-evidence:\n  probed: '2026-08-06'\n  results:\n  - url: https://levacares.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://levacares.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://levacares.com/wp-json/mcp/mcp-oauth-server\n    http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axena-health/refs/heads/main/scopes/axena-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health
- Digital Health
- Medical Devices
- Women's Health
- Digital Therapeutics
- Pelvic Health
- Medical Software
- Telehealth
token_urls: []
---
