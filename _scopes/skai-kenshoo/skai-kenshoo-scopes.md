---
api_specs:
- filename: skai-kenshoo-api-openapi.yml
  format: yaml
  label: Skai (Kenshoo) API
  slug: skai-kenshoo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skai-kenshoo/refs/heads/main/openapi/skai-kenshoo-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Skai Kenshoo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Skai (Kenshoo) uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Skai (Kenshoo)
provider_slug: skai-kenshoo
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: skai-kenshoo-scopes
source_filename: skai-kenshoo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://login.kenshoo.com/.well-known/oauth-authorization-server,\n  https://mcp.kenshoo.com/.well-known/oauth-protected-resource,\n  https://skai.io/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Skai publishes no scopes/permissions reference page. Every scope below was read from live\n  RFC 8414 / RFC 9728 discovery metadata, not from prose documentation. The REST API has no\n  scope surface at all — it uses a bespoke refresh-token exchange and derives permission from\n  the Skai user's platform role.\napplies_to: MCP servers only\nauthorization_servers:\n- issuer: https://login.kenshoo.com\n  used_by: https://mcp.kenshoo.com (Reporting MCP, Operations MCP)\n  scopes:\n  - name: openid\n    description: >-\n      Standard OIDC scope requesting an ID token. Advertised, though no OIDC discovery\n      document is published on this issuer.\n    source: authorization-server metadata\n  - name: profile\n\
  \    description: Standard OIDC scope for basic profile claims about the authenticating Skai user.\n    source: authorization-server + protected-resource metadata\n  - name: email\n    description: Standard OIDC scope for the authenticating Skai user's email address.\n    source: authorization-server + protected-resource metadata\n  - name: offline_access\n    description: >-\n      Requests a refresh token so an MCP client can maintain a long-lived session without\n      re-prompting the user.\n    source: authorization-server + protected-resource metadata\n- issuer: https://skai.io\n  used_by: https://skai.io/wp-json/mcp/* (WordPress MCP adapter on the marketing site)\n  scopes:\n  - name: mcp\n    description: >-\n      Single coarse scope gating the WordPress MCP adapter surface on the skai.io marketing\n      site. Unrelated to the Skai platform.\n    source: authorization-server metadata\nfindings:\n- >-\n  No resource-level or action-level scopes exist. Nothing in the published\
  \ metadata\n  distinguishes read from write, so an agent granted access to the Operations MCP — which\n  changes bids, budgets and campaign statuses — carries the same four scopes as one granted\n  read-only reporting access. Least-privilege delegation is not expressible through scopes;\n  Skai separates read and write by ENDPOINT (reports-mcp vs operations-mcp) rather than by\n  scope.\n- >-\n  Authorization is enforced by the Skai platform role of the underlying user (Standard or\n  higher) and by ks/agency context, not by OAuth scope.\nscope_count: 5\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skai-kenshoo/refs/heads/main/scopes/skai-kenshoo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Commerce
- Advertising
- Marketing
- Retail Media
- Paid Search
- Paid Social
- Marketing Analytics
- Advertising Technology
- Campaign Management
- Commerce Media
- Reporting
- MCP
- Agent Native
- Omnichannel
token_urls: []
---
