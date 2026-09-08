---
authorization_urls: []
description: 'The only OAuth scope Amphenol publishes anywhere is the single scope "mcp", declared in the RFC 8414 authorization server metadata document served by Amphenol Automotive and repeated in its RFC 9728 protected resource metadata. There is no scope reference page, no permissions matrix, and no finer-grained scope: the whole Model Context Protocol resource sits behind one coarse grant.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Amphenol Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Amphenol uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Amphenol
provider_slug: amphenol
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: amphenol-scopes
source_filename: amphenol-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://amphenol-automotive.com/.well-known/oauth-authorization-server\nprovider: Amphenol\nproviderId: amphenol\ndescription: >-\n  The only OAuth scope Amphenol publishes anywhere is the single scope \"mcp\", declared in the\n  RFC 8414 authorization server metadata document served by Amphenol Automotive and repeated in\n  its RFC 9728 protected resource metadata. There is no scope reference page, no permissions\n  matrix, and no finer-grained scope: the whole Model Context Protocol resource sits behind one\n  coarse grant.\nauthorization_server: https://amphenol-automotive.com\nresource: https://amphenol-automotive.com/wp-json/mcp/mcp-oauth-server\nscope_count: 1\nscopes:\n  - name: mcp\n    description: >-\n      Grants access to the Amphenol Automotive Model Context Protocol resource. The provider\n      publishes no description of what the scope permits; the name is taken verbatim from the\n      scopes_supported array\
  \ in the metadata document. What it actually authorises could not be\n      determined without an authenticated tools/list call.\n    source: /.well-known/oauth-authorization-server\n    granularity: coarse\ndocs: null\ndocs_note: No scopes or permissions reference page exists to enrich these definitions.\nx-evidence:\n  - url: https://amphenol-automotive.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://amphenol-automotive.com/.well-known/oauth-protected-resource\n    status: 200\nchecked: '2026-09-02'\nmaintainers:\n  - FN: API Evangelist\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amphenol/refs/heads/main/scopes/amphenol-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Electronic Connectors
- Interconnect Systems
- Fiber Optics
- Sensors
- Aerospace
- Automotive
- Defense
- Manufacturing
- Fortune 500
token_urls: []
---
