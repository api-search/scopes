---
api_specs:
- filename: globaldatabase-com-mcp-playground-openapi.yml
  format: yaml
  label: Global Database MCP Server
  slug: global-database-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-mcp-playground-openapi.yml
authorization_urls: []
description: ''
docs: https://github.com/global-database/mcp-server#microsoft-copilot-studio
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Globaldatabase Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Global Database uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Global Database
provider_slug: globaldatabase-com
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: globaldatabase-com-scopes
source_filename: globaldatabase-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://mcp.globaldatabase.com/.well-known/oauth-protected-resource + https://mcp.globaldatabase.com/.well-known/oauth-authorization-server + https://github.com/global-database/mcp-server (README, Copilot Studio section)\ndocs: https://github.com/global-database/mcp-server#microsoft-copilot-studio\nscope_count: 0\nsummary: >-\n  The provider runs an OAuth 2.1 authorization server for its MCP endpoint but publishes NO\n  scopes: the RFC 9728 protected-resource document declares `scopes_supported: []` and the\n  RFC 8414 document omits `scopes_supported` entirely. The README states it plainly (\"the\n  server publishes no scopes, and a non-empty one fails the token request\"). Authorization is\n  therefore all-or-nothing at the account level; entitlements (e.g. the AI-query entitlement\n  that returns 403 on POST /v2/ai/query) are enforced per account/module server-side, not via\n  OAuth scope. The consent page (\"You see exactly\
  \ what the assistant can read, and you can\n  revoke it later\" — landing page) is coarse-grained. The REST API uses a static token with no\n  scope concept; per-module permissions surface only through GET /v2/metrics\n  (permission / module / app blocks in the LimitError body).\nscopes: []\naccount_level_entitlements_observed_in_docs:\n- {name: AI-query entitlement, evidence: 'POST /v2/ai/query returns 403 {detail, code} \"No AI-query entitlement on the account\" (docs v2, Regis API errors table).'}\n- {name: module permissions, evidence: 'LimitError body carries access.permission / access.module / access.app and error_guard \"limits.daily\" (docs v2, Errors).'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/scopes/globaldatabase-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Company Data
- KYB
- Compliance
- Business Verification
- Beneficial Ownership
- Financial
- Credit Risk
- Data Enrichment
- Prospecting
- Webhook
- MCP
- AI Agents
- United Kingdom
token_urls: []
---
