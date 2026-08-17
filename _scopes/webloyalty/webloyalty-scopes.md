---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Webloyalty Scopes
name_suffix: OAuth Scopes
note: The authorization server advertises exactly one scope. There is no published scope reference page — Webloyalty has no developer documentation of any kind — so this is the complete, machine-advertised scope surface and nothing more is inferred.
overview: 'Webloyalty uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Webloyalty
provider_slug: webloyalty
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: webloyalty-scopes
source_filename: webloyalty-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://webloyalty.co.uk/.well-known/oauth-authorization-server\nnote: >-\n  The authorization server advertises exactly one scope. There is no published\n  scope reference page — Webloyalty has no developer documentation of any kind —\n  so this is the complete, machine-advertised scope surface and nothing more is\n  inferred.\nissuer: https://webloyalty.co.uk\nauthorization_url: https://webloyalty.co.uk/oauth/authorize\ntoken_url: https://webloyalty.co.uk/oauth/token\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Access the MCP resource at\n    https://webloyalty.co.uk/wp-json/mcp/mcp-oauth-server. Coarse-grained: the\n    server publishes no read/write split and no per-tool scopes.\n  resource: https://webloyalty.co.uk/wp-json/mcp/mcp-oauth-server\n  source: scopes_supported in the RFC 8414 metadata (and repeated in the RFC 9728\n    protected-resource metadata)\ndocs: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webloyalty/refs/heads/main/scopes/webloyalty-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Loyalty
- Rewards
- Ecommerce
- Customer Engagement
- Marketing
- Retail
- Cashback
token_urls: []
---
