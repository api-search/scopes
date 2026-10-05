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
overview: 'Wayground publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wayground API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wayground
provider_slug: quizizz
schemes: []
scope_count: 1
scope_names:
- full_access
scopes:
- description: Verbatim from the provider's own metadata. Wayground does not state what it grants; from the protected-resource document it is the scope required to call https://wayground.com/_quizizzmcp/main/mcp.
  flows: []
  scope: full_access
slug: quizizz-scopes
source_filename: quizizz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  scopes_supported in https://wayground.com/.well-known/oauth-authorization-server and\n  https://wayground.com/.well-known/oauth-protected-resource (both HTTP 200, 2026-08-26).\ndocs: null\ndocs_note: >-\n  Wayground publishes no scopes or permissions reference page. Searched wayground.com,\n  help.wayground.com and support.wayground.com; nothing documents the OAuth surface at all.\nscope_count: 1\nscopes:\n- name: full_access\n  description: >-\n    Verbatim from the provider's own metadata. Wayground does not state what it grants; from\n    the protected-resource document it is the scope required to call\n    https://wayground.com/_quizizzmcp/main/mcp.\n  resource: https://wayground.com/_quizizzmcp/main/mcp\n  granularity: coarse\nnote: >-\n  A single all-or-nothing scope is the finding. An agent authorising against Wayground's MCP\n  server cannot request less than everything the scope covers, and cannot tell from any\n\
  \  published source what \"everything\" is.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quizizz/refs/heads/main/scopes/quizizz-scopes.yml
summary_line: 1 scope
tags:
- Company
- Education
- EdTech
- K-12
- Learning
- Assessment
- Artificial Intelligence
- MCP
- LTI
- Rostering
- SSO
token_bound: false
token_urls: []
---
