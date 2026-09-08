---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Veradermics Scopes
name_suffix: OAuth Scopes
note: Not derived from an OpenAPI — this provider publishes none — and not searched from a docs scopes reference, because no developer documentation exists. The single scope below is read verbatim from the scopes_supported array in the RFC 8414 metadata the WordPress MCP Adapter serves on the corporate host, and is corroborated by the scopes_supported array in the RFC 9728 protected-resource metadata.
overview: 'Veradermics uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Veradermics
provider_slug: veradermics
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: veradermics-scopes
source_filename: veradermics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://www.veradermics.com/.well-known/oauth-authorization-server\nnote: >-\n  Not derived from an OpenAPI — this provider publishes none — and not searched from a\n  docs scopes reference, because no developer documentation exists. The single scope\n  below is read verbatim from the scopes_supported array in the RFC 8414 metadata the\n  WordPress MCP Adapter serves on the corporate host, and is corroborated by the\n  scopes_supported array in the RFC 9728 protected-resource metadata.\nauthorization_server: https://www.veradermics.com\nscopes:\n- name: mcp\n  description: >-\n    Grants a client access to the MCP server at\n    https://www.veradermics.com/wp-json/mcp/mcp-oauth-server. The authorization server\n    advertises no finer-grained scopes; what the scope actually authorizes depends on\n    the WordPress abilities exposed to the authenticated account, which could not be\n    enumerated anonymously.\n  source: scopes_supported\n\
  \  applies_to: https://www.veradermics.com/wp-json/mcp/mcp-oauth-server\nscope_count: 1\nx-evidence:\n  fetched: '2026-09-02'\n  probes:\n  - url: https://www.veradermics.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://www.veradermics.com/.well-known/oauth-protected-resource\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veradermics/refs/heads/main/scopes/veradermics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Healthcare
- Dermatology
- Clinical Trials
- Drug Development
token_urls: []
---
