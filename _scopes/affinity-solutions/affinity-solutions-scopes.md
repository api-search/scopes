---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Affinity Solutions Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Affinity Solutions uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Affinity Solutions
provider_slug: affinity-solutions
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: affinity-solutions-scopes
source_filename: affinity-solutions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://www.affinity.solutions/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  The provider publishes no scopes or permissions reference page; these scopes are read from the\n  authorization-server and protected-resource metadata documents themselves.\nauthorization_server: https://www.affinity.solutions\nscopes:\n- name: mcp\n  description: >-\n    The single scope the authorization server advertises (scopes_supported) and the single scope the\n    protected-resource document attaches to the MCP endpoint. The provider publishes no per-tool or\n    per-resource scope breakdown; a finer-grained model, if one exists, is only visible after an\n    authenticated tools/list, which returns 401 anonymously.\n  resource: https://www.affinity.solutions/wp-json/mcp/mcp-oauth-server\n  source: both scopes_supported in the RFC 8414 document and scopes_supported in the RFC 9728 document\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinity-solutions/refs/heads/main/scopes/affinity-solutions-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Data
- Analytics
- Consumer Purchase Data
- Transaction Data
- Marketing
- Advertising
- Measurements
- Financial-Services
- Retail
- MCP
token_urls: []
---
