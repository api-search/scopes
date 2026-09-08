---
authorization_urls: []
description: The complete scope surface Apollo Global Management advertises. It is the standard OpenID Connect set plus offline_access — no Apollo-specific business scopes are published. Apollo has no scopes or permissions reference page; a documentation search across www.apollo.com (4,784 sitemap URLs, no /api or /developer path segment anywhere) found none, so nothing could be added beyond what the discovery documents declare.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Apollo Global Management Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Apollo Global Management uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apollo Global Management
provider_slug: apollo-global-management
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: apollo-global-management-scopes
source_filename: apollo-global-management-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://api.apollo.com/.well-known/oauth-authorization-server (scopes_supported) and\n  https://api.apollo.com/.well-known/oauth-protected-resource/mcp (scopes_supported),\n  both HTTP 200, fetched 2026-09-04.\ndescription: >-\n  The complete scope surface Apollo Global Management advertises. It is the standard\n  OpenID Connect set plus offline_access — no Apollo-specific business scopes are\n  published. Apollo has no scopes or permissions reference page; a documentation search\n  across www.apollo.com (4,784 sitemap URLs, no /api or /developer path segment anywhere)\n  found none, so nothing could be added beyond what the discovery documents declare.\ndocs: null\ndocs_note: No scopes/permissions reference page is published by Apollo.\nauthorization_server: https://api.apollo.com\nscopes:\n  - name: openid\n    description: >-\n      Standard OpenID Connect scope requesting an ID token. Advertised by both the\n      authorization\
  \ server and the MCP protected resource.\n    standard: openid-connect-core\n    resources:\n      - https://api.apollo.com/mcp\n  - name: profile\n    description: >-\n      Standard OpenID Connect scope for basic profile claims. Advertised by both the\n      authorization server and the MCP protected resource.\n    standard: openid-connect-core\n    resources:\n      - https://api.apollo.com/mcp\n  - name: email\n    description: >-\n      Standard OpenID Connect scope for the email and email_verified claims. Advertised by\n      both the authorization server and the MCP protected resource.\n    standard: openid-connect-core\n    resources:\n      - https://api.apollo.com/mcp\n  - name: offline_access\n    description: >-\n      Standard scope requesting a refresh token. Advertised by the authorization server\n      only; the MCP protected-resource document does not list it.\n    standard: openid-connect-core\n    resources: []\nscope_count: 4\ngaps:\n  - >-\n    No resource-specific\
  \ or business-domain scopes are advertised. Whatever the MCP server\n    lets an authorized agent read or write is not expressed in the scope surface, so an\n    integrator cannot reason about least privilege from public documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-global-management/refs/heads/main/scopes/apollo-global-management-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Alternative Investments
- Asset Management
- Credit
- Finance
- Investment Management
- Private Equity
- Real Assets
token_urls: []
---
