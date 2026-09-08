---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Vanderhall Motor Works Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vanderhall Motor Works uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vanderhall Motor Works
provider_slug: vanderhall-motor-works
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: vanderhall-motor-works-scopes
source_filename: vanderhall-motor-works-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://portal.vanderhallusa.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Vanderhall publishes no scopes/permissions reference page. The scope list below is taken verbatim\n  from the `scopes_supported` array of the live RFC 8414 authorization-server metadata document and\n  nothing has been added to it. The human-readable description is API Evangelist's, derived from the\n  protected resource the scope guards; Vanderhall states no description of its own.\nauthorization_server: https://portal.vanderhallusa.com\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Grants a client access to the Vanderhall Admin Portal MCP endpoint at\n    https://portal.vanderhallusa.com/mcp. It is the only scope the authorization server advertises,\n    so the MCP surface is all-or-nothing — there is no read/write split, no per-resource scope, and\n    no way for a consumer to request least privilege.\n  protected_resource:\
  \ https://portal.vanderhallusa.com/mcp\n  source: scopes_supported[0]\ngrants:\n- authorization_code\n- refresh_token\npkce_methods:\n- S256\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanderhall-motor-works/refs/heads/main/scopes/vanderhall-motor-works-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Automotive
- Manufacturing
- Electric Vehicles
- Powersports
- Autocycles
- Dealer Network
- Model Context Protocol
- Utah
token_urls: []
---
