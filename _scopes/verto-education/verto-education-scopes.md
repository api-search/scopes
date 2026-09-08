---
authorization_urls: []
description: The complete scope surface Verto Education's authorization server advertises. Both discovery documents agree and both list exactly one scope. There is no published scopes or permissions reference page to enrich this from - the metadata document is the only source, and it is the authoritative one.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Verto Education Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Verto Education uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Verto Education
provider_slug: verto-education
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: verto-education-scopes
source_filename: verto-education-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://vertoeducation.org/.well-known/oauth-authorization-server\nname: Verto Education OAuth Scopes\ndescription: >-\n  The complete scope surface Verto Education's authorization server advertises. Both\n  discovery documents agree and both list exactly one scope. There is no published\n  scopes or permissions reference page to enrich this from - the metadata document is\n  the only source, and it is the authoritative one.\nauthorization_server: https://vertoeducation.org\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Grants access to the Model Context Protocol endpoint at\n    https://vertoeducation.org/wp-json/mcp/mcp-oauth-server. The server declares no\n    finer-grained read/write split - a token either carries `mcp` or it reaches nothing.\n  resource: https://vertoeducation.org/wp-json/mcp/mcp-oauth-server\n  source: scopes_supported in RFC 8414 metadata and RFC 9728 protected-resource metadata\n  documented_by_provider:\
  \ false\ndocs: null\ndocs_note: >-\n  No human-readable scopes/permissions reference is published. Searched the site and\n  its llms.txt page inventory; the developer surface is entirely undocumented in prose.\ngranularity_note: >-\n  A single coarse scope over a whole MCP tool surface means a consenting user cannot\n  grant an agent partial access. What `mcp` actually authorises cannot be established\n  anonymously because tools/list is itself gated (HTTP 401).\nx-evidence:\n- url: https://vertoeducation.org/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://vertoeducation.org/.well-known/oauth-protected-resource\n  http_status: 200\nchecked: '2026-09-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verto-education/refs/heads/main/scopes/verto-education-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Education
- Higher Education
- Study Abroad
- College Admissions
- Students
- Travel
- Model Context Protocol
- OAuth
- Agents
token_urls: []
---
