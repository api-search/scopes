---
authorization_urls: []
description: ''
docs: https://api-docs.tgl.ai/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Reflexivity Scopes
name_suffix: OAuth Scopes
note: 'Read verbatim from Reflexivity''s own RFC 8414 Authorization Server Metadata document, which is served anonymously and enumerates scopes_supported. This is NOT derived from an OpenAPI spec — Reflexivity publishes no public OpenAPI, and the Theneo-hosted API reference is password-protected. Every scope below is the exact string the authorization server advertises. Descriptions are left empty rather than invented: the AS metadata carries no scope descriptions and the scope reference page is behind the documentation password. The naming is the finding — all 23 published scopes are namespaced `mcp:`, meaning Reflexivity''s authorization surface is organised around Model Context Protocol services rather than around REST resources.'
overview: 'Reflexivity uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Reflexivity
provider_slug: reflexivity
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: reflexivity-scopes
source_filename: reflexivity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://identity.reflexivity.com/.well-known/oauth-authorization-server\ndocs: https://api-docs.tgl.ai/\nnote: >-\n  Read verbatim from Reflexivity's own RFC 8414 Authorization Server Metadata document, which is served\n  anonymously and enumerates scopes_supported. This is NOT derived from an OpenAPI spec — Reflexivity\n  publishes no public OpenAPI, and the Theneo-hosted API reference is password-protected. Every scope\n  below is the exact string the authorization server advertises. Descriptions are left empty rather than\n  invented: the AS metadata carries no scope descriptions and the scope reference page is behind the\n  documentation password. The naming is the finding — all 23 published scopes are namespaced `mcp:`, meaning\n  Reflexivity's authorization surface is organised around Model Context Protocol services rather than\n  around REST resources.\nauthorization_server: https://identity.reflexivity.com\nauthorization_endpoint:\
  \ https://identity.reflexivity.com/oauth/authorize\ntoken_endpoint: https://identity.reflexivity.com/oauth/token\nregistration_endpoint: https://identity.reflexivity.com/oauth/register\ngrant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\ncode_challenge_methods_supported:\n  - S256\n  - plain\nscope_count: 23\nscopes:\n  - name: 'mcp:*'\n    description: ''\n    note: wildcard — grants every MCP service scope\n  - name: 'mcp:alfred-integrations'\n    description: ''\n    note: >-\n      \"Alfred\" is Reflexivity's in-product assistant; the terminal SPA calls an `alfred/v1` API path\n  - name: 'mcp:attribution-insights'\n    description: ''\n  - name: 'mcp:earnings'\n    description: ''\n  - name: 'mcp:earnings-insights'\n    description: ''\n  - name: 'mcp:entity-performance'\n    description: ''\n  - name: 'mcp:entity-screener'\n    description: ''\n  - name: 'mcp:file-processor'\n    description: ''\n  - name: 'mcp:financial-events'\n    description:\
  \ ''\n  - name: 'mcp:financial-statements'\n    description: ''\n  - name: 'mcp:insights'\n    description: ''\n  - name: 'mcp:kg-insights'\n    description: ''\n    note: knowledge-graph insights — matches the published Knowledge Graph capability page\n  - name: 'mcp:lseg-datastream-search'\n    description: ''\n    note: LSEG Datastream is named as a licensed data source on reflexivity.com\n  - name: 'mcp:news'\n    description: ''\n  - name: 'mcp:ontology'\n    description: ''\n  - name: 'mcp:price-history'\n    description: ''\n  - name: 'mcp:quant'\n    description: ''\n  - name: 'mcp:scenario-orchestrator'\n    description: ''\n    note: matches the published Scenario Analysis capability page\n  - name: 'mcp:search'\n    description: ''\n  - name: 'mcp:theme'\n    description: ''\n  - name: 'mcp:theme:v3'\n    description: ''\n    note: the only versioned scope in the set — v3 of the theme service\n  - name: 'mcp:watchlist'\n    description: ''\n  - name: 'mcp:web-search'\n    description:\
  \ ''\nx-evidence:\n  fetched: '2026-08-26'\n  url: https://identity.reflexivity.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reflexivity/refs/heads/main/scopes/reflexivity-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Financial-Services
- Investment Analysis
- Market Data
- Artificial Intelligence
- Machine-Learning
- Fintech
- Research
- Knowledge Graph
- Agents
token_urls: []
---
