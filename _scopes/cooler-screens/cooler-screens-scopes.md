---
authorization_urls: []
description: The complete published scope surface for CoolerX, read from the RFC 8414 authorization server metadata and confirmed by the RFC 9728 protected resource metadata. Both documents declare exactly one scope. There is no scopes or permissions reference page on any CoolerX host to enrich this from.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cooler Screens Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CoolerX uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoolerX
provider_slug: cooler-screens
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cooler-screens-scopes
source_filename: cooler-screens-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://coolerx.com/.well-known/oauth-authorization-server\nname: CoolerX OAuth scopes\ndescription: >-\n  The complete published scope surface for CoolerX, read from the RFC 8414 authorization\n  server metadata and confirmed by the RFC 9728 protected resource metadata. Both\n  documents declare exactly one scope. There is no scopes or permissions reference page\n  on any CoolerX host to enrich this from.\ndocs: null\ndocs_note: >-\n  No permissions/scopes documentation published. CoolerX has no developer portal; probed\n  https://coolerx.com/developers/ (404) and /docs (404) on 2026-08-12.\nauthorization_server: https://coolerx.com\nscopes:\n- name: mcp\n  description: >-\n    Access to the CoolerX WordPress MCP server at\n    https://coolerx.com/wp-json/mcp/mcp-oauth-server. The single scope the authorization\n    server advertises and the single scope the protected resource requires. Its\n    granularity is undocumented —\
  \ the underlying WordPress Abilities API\n    (/wp-json/wp-abilities/v1/abilities) returned 401, so which abilities the scope\n    actually unlocks could not be read.\n  source: well-known/cooler-screens-oauth-authorization-server.json\n  resources:\n  - https://coolerx.com/wp-json/mcp/mcp-oauth-server\nscope_count: 1\ngranularity: coarse\ngranularity_note: >-\n  A single all-or-nothing scope gates the entire MCP tool surface. There is no read/write\n  split and no per-ability scoping, so a consenting client cannot be granted less than\n  everything the server exposes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooler-screens/refs/heads/main/scopes/cooler-screens-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Retail
- Retail Media
- Advertising
- Digital Signage
- In-Store Media
- Merchandising
- Artificial Intelligence
- Internet of Things
token_urls: []
---
