---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Quizizz Scopes
name_suffix: OAuth Scopes
note: A single all-or-nothing scope is the finding. An agent authorising against Wayground's MCP server cannot request less than everything the scope covers, and cannot tell from any published source what "everything" is.
overview: 'Wayground uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wayground
provider_slug: quizizz
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: quizizz-scopes
source_filename: quizizz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  scopes_supported in https://wayground.com/.well-known/oauth-authorization-server and\n  https://wayground.com/.well-known/oauth-protected-resource (both HTTP 200, 2026-08-26).\ndocs: null\ndocs_note: >-\n  Wayground publishes no scopes or permissions reference page. Searched wayground.com,\n  help.wayground.com and support.wayground.com; nothing documents the OAuth surface at all.\nscope_count: 1\nscopes:\n- name: full_access\n  description: >-\n    Verbatim from the provider's own metadata. Wayground does not state what it grants; from\n    the protected-resource document it is the scope required to call\n    https://wayground.com/_quizizzmcp/main/mcp.\n  resource: https://wayground.com/_quizizzmcp/main/mcp\n  granularity: coarse\nnote: >-\n  A single all-or-nothing scope is the finding. An agent authorising against Wayground's MCP\n  server cannot request less than everything the scope covers, and cannot tell from any\n\
  \  published source what \"everything\" is.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quizizz/refs/heads/main/scopes/quizizz-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Education
- EdTech
- K-12
- Learning
- Assessment
- Artificial Intelligence
- Model Context Protocol
- LTI
- Rostering
- Single Sign On
token_urls: []
---
