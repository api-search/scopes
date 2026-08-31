---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sdui Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sdui uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sdui
provider_slug: sdui
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: sdui-scopes
source_filename: sdui-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://sdui.de/.well-known/oauth-authorization-server\napi: Sdui Website MCP Server\nauthorization_server: https://sdui.de\ndocs: null\ndocs_note: Sdui publishes no OAuth scope reference page; the scope set below is read from the served RFC 8414 metadata only.\nflows:\n- type: authorization_code\n  authorization_endpoint: https://sdui.de/oauth/authorize\n  token_endpoint: https://sdui.de/oauth/token\n  revocation_endpoint: https://sdui.de/oauth/revoke\n  pkce: true\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  refresh_token_supported: true\nscopes:\n- name: mcp\n  description: >-\n    The single scope advertised by both the authorization-server metadata (scopes_supported) and the\n    protected-resource metadata for https://sdui.de/wp-json/mcp/mcp-oauth-server. Sdui publishes no\n    description of what it grants; it is recorded verbatim as the only declared scope.\n  source: /.well-known/oauth-authorization-server\
  \ + /.well-known/oauth-protected-resource\nscope_count: 1\nnotes:\n- token_endpoint_auth_methods_supported is [\"none\"], i.e. public clients with PKCE.\n- client_id_metadata_document_supported is true.\n- The Sdui Platform API at api.sdui.app does NOT use OAuth — it answers WWW-Authenticate Bearer with no discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sdui/refs/heads/main/scopes/sdui-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Education
- EdTech
- Schools
- Communications
- Messaging
- Timetabling
- Grade Management
- Germany
- GDPR
token_urls: []
---
