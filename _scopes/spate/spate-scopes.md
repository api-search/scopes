---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Spate Scopes
name_suffix: OAuth Scopes
note: Spate's authorization server advertises exactly one scope. There is no published scope/permissions reference page on spate.nyc or the help center, and no OpenAPI oauth2 securityScheme to derive a richer set from — so this is the complete, real scope surface as the provider advertises it, not a partial harvest.
overview: 'Spate uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spate
provider_slug: spate
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: spate-scopes
source_filename: spate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.spate.nyc/.well-known/oauth-authorization-server\nnote: >-\n  Spate's authorization server advertises exactly one scope. There is no\n  published scope/permissions reference page on spate.nyc or the help center,\n  and no OpenAPI oauth2 securityScheme to derive a richer set from — so this\n  is the complete, real scope surface as the provider advertises it, not a\n  partial harvest.\n\nauthorization_server: https://api.spate.nyc/mcp\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The single coarse scope advertised for the Spate MCP endpoint. It is not\n    described anywhere in Spate's public documentation; the name is taken\n    verbatim from `scopes_supported` in both the RFC 8414\n    authorization-server metadata and the RFC 9728 protected-resource\n    metadata.\n  source: scopes_supported\n  granularity: coarse\n  covers:\n  - top_trends\n  - time_series\n  - top_related_trends\n  - find_category\n\
  \nfindings:\n- >-\n  There is no read/write split and no per-tool scope. A token minted for the\n  Spate MCP server carries the whole trend-data surface, so an agent cannot\n  be granted least privilege against it.\n- >-\n  All four tools are read-only data retrieval, so the blast radius of the\n  single scope is bounded — but that is a property of the current tool set,\n  not a guarantee expressed in the authorization model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spate/refs/heads/main/scopes/spate-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Enterprise Saas
- Market Intelligence
- Trend Forecasting
- Consumer Insights
- Social Listening
- Analytics
- Beauty
- MCP
- AI Agents
- Trend Data
- Consumer Packaged Goods
token_urls: []
---
