---
authorization_urls: []
description: The only OAuth scope Vi Labs publishes is the single coarse `mcp` scope advertised in both its authorization server metadata and its protected resource metadata. There is no scopes or permissions reference page — Vi Labs publishes no developer documentation at all — so this is the complete published scope surface, not a sample of it.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Vi Labs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vi Labs uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vi Labs
provider_slug: vi-labs
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: vi-labs-scopes
source_filename: vi-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://vi.co/.well-known/oauth-authorization-server\nname: Vi Labs OAuth scopes\ndescription: >-\n  The only OAuth scope Vi Labs publishes is the single coarse `mcp` scope\n  advertised in both its authorization server metadata and its protected\n  resource metadata. There is no scopes or permissions reference page — Vi Labs\n  publishes no developer documentation at all — so this is the complete\n  published scope surface, not a sample of it.\nauthorization_server: https://vi.co\ndocs: null\ndocs_note: No published scopes/permissions reference exists on vi.co.\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Access to the Vi Labs Model Context Protocol server at\n    https://vi.co/wp-json/mcp/mcp-oauth-server. The provider publishes no\n    breakdown of what the scope grants; granularity below this scope is not\n    documented.\n  source: scopes_supported in RFC 8414 + RFC 9728 metadata\n  operations: []\nx-evidence:\n\
  \  fetched: '2026-09-02'\n  probes:\n  - url: https://vi.co/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://vi.co/.well-known/oauth-protected-resource\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vi-labs/refs/heads/main/scopes/vi-labs-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Artificial Intelligence
- Health
- Healthcare
- Life Sciences
- Pharmaceuticals
- Patient Engagement
- Enterprise AI
- AI Agents
- Model Context Protocol
- Data
token_urls: []
---
