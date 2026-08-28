---
authorization_urls: []
description: ''
docs: https://moz.com/api/docs/guides/mcp-servers
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Moz Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Moz uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Moz
provider_slug: moz
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: moz-scopes
source_filename: moz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://api.moz.com/.well-known/oauth-protected-resource/mcp/v1/data\ndocs: https://moz.com/api/docs/guides/mcp-servers\nsummary: >-\n  Moz declares a single OAuth scope, \"mcp\", in both the authorization-server metadata and each MCP\n  endpoint's protected-resource metadata. There is no per-resource or per-method scope vocabulary;\n  authorization granularity comes from the subscription attached to the account, not from scopes.\nauthorization_server: https://api.moz.com\napplies_to:\n- https://api.moz.com/mcp/v1/data\n- https://api.moz.com/mcp/v1/local\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Access to the Moz MCP surface for the authenticated account. Declared in\n    scopes_supported on both /.well-known/oauth-authorization-server and each\n    /.well-known/oauth-protected-resource/mcp/v1/* document.\n  source: RFC 8414 + RFC 9728 metadata, probed 2026-08-26\nnotes:\n- >-\n  The JSON-RPC API at https://api.moz.com/jsonrpc\
  \ is API-key authenticated and has no scope surface\n  at all - see authentication/moz-authentication.yml.\n- >-\n  Because the beta restricts MCP access to account owners, an MCP token today carries whatever the\n  owner's subscription carries; Moz documents no read-only or per-product scope split.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moz/refs/heads/main/scopes/moz-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- SEO
- Search
- Marketing
- Analytics
- Keywords
- Backlinks
- Local Marketing
- Domain Authority
- Link Index
- JSON-RPC
- MCP
- Company
token_urls: []
---
