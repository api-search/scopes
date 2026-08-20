---
authorization_urls: []
description: The complete OAuth scope surface Cardiosense advertises. It is one scope. Both the RFC 8414 authorization server metadata and the RFC 9728 protected resource metadata declare the identical single-entry list, and there is no scope reference page anywhere on the site to enrich it from.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cardiosense Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cardiosense uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cardiosense
provider_slug: cardiosense
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cardiosense-scopes
source_filename: cardiosense-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://cardiosense.com/.well-known/oauth-authorization-server\ndescription: >-\n  The complete OAuth scope surface Cardiosense advertises. It is one scope.\n  Both the RFC 8414 authorization server metadata and the RFC 9728 protected\n  resource metadata declare the identical single-entry list, and there is no\n  scope reference page anywhere on the site to enrich it from.\ndocs: null\ndocs_note: >-\n  No scopes/permissions reference page is published. SEARCHed the site,\n  llms.txt, and llms-full.txt — none of them mention scopes, tokens, or the\n  MCP endpoint at all.\n\nscopes:\n  - name: mcp\n    description: >-\n      Access to the Cardiosense Model Context Protocol server at\n      /wp-json/mcp/mcp-oauth-server. The scope name is all that is published;\n      Cardiosense documents no semantics for it — no read/write split, no\n      resource qualification, and no statement of what an `mcp`-scoped token\n      is permitted\
  \ to do.\n    granularity: coarse\n    read_write: undocumented\n    source: /.well-known/oauth-authorization-server + /.well-known/oauth-protected-resource\n\ncoverage:\n  scopes_declared: 1\n  scopes_documented: 0\n  note: >-\n    A single coarse scope means an agent client cannot request least privilege:\n    the only grant available is all-or-nothing access to the MCP server.\n\nobservations:\n  - Both discovery documents agree, so this is not a metadata drift case.\n  - No incremental authorization, no scope-per-tool mapping, no consent-screen copy is published.\n  - Because tools/list is itself gated (HTTP 401), it is not possible to check what the `mcp` scope actually unlocks without credentials.\n\nx-evidence:\n  fetched: '2026-08-09'\n  probes:\n    - url: https://cardiosense.com/.well-known/oauth-authorization-server\n      status: 200\n    - url: https://cardiosense.com/.well-known/oauth-protected-resource\n      status: 200\n    - url: https://cardiosense.com/wp-json/mcp/mcp-oauth-server\n\
  \      status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiosense/refs/heads/main/scopes/cardiosense-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health
- Digital Health
- Medical Devices
- Cardiology
- Heart Failure
- Remote Patient Monitoring
- Wearables
- Artificial Intelligence
- Machine-Learning
- MCP
token_urls: []
---
