---
api_specs:
- filename: newtqnia-news-api-openapi.yml
  format: yaml
  label: NewTqnia | Technology News, AI and Innovation News API
  slug: newtqnia-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newtqnia/refs/heads/main/openapi/newtqnia-news-api-openapi.yml
authorization_urls: []
description: ''
docs: https://newtqnia.com/en/connect
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Newtqnia Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found no oauth2 securitySchemes because the published OpenAPI declares none - the REST contract is keyless. The OAuth surface belongs to the MCP server and its scopes were read directly from the live RFC 8414 / RFC 9728 discovery documents, not inferred.
overview: 'NewTqnia | Technology News, AI and Innovation uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NewTqnia | Technology News, AI and Innovation
provider_slug: newtqnia
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: newtqnia-scopes
source_filename: newtqnia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://newtqnia.com/.well-known/oauth-authorization-server (HTTP 200) and https://newtqnia.com/.well-known/oauth-protected-resource (HTTP 200)\ndocs: https://newtqnia.com/en/connect\nnote: >-\n  derive-oauth-scopes.py found no oauth2 securitySchemes because the published OpenAPI\n  declares none - the REST contract is keyless. The OAuth surface belongs to the MCP\n  server and its scopes were read directly from the live RFC 8414 / RFC 9728 discovery\n  documents, not inferred.\n\nauthorization_server: https://newtqnia.com\nprotected_resource: https://newtqnia.com/mcp\nflows:\n  authorization_code:\n    authorization_url: https://newtqnia.com/oauth/authorize\n    token_url: https://newtqnia.com/oauth/token\n    refresh_supported: true\n    pkce_required_methods: [S256]\n\nscopes:\n- name: mcp:read\n  description: >-\n    Read-only access to published NewTqnia content over MCP - recent news, a single\n    article, a story timeline,\
  \ glossary terminology and explainers, each as title,\n    summary and canonical URL. This is what a signed-in reader's assistant receives.\n  source: oauth-authorization-server scopes_supported\n  maps_to_tools: [server_status, get_recent_news, get_news_by_id, get_timeline_by_id, search_terminology, search_explainers]\n- name: mcp:write\n  description: >-\n    Write access backing the editor/administrator content-drafting workflow the provider\n    documents in llms.txt. No write tool is exposed in the anonymous tools/list result -\n    all six live tools are annotated readOnlyHint:true - so the write surface this scope\n    protects is visible only to an authorized editor session.\n  source: oauth-authorization-server scopes_supported\n  maps_to_tools: []\n\nscope_count: 2\nbearer_methods_supported: [header]\ngaps:\n- >-\n  Scopes are coarse: one read and one write for the entire MCP surface, with no per-tool\n  or per-content-type granularity. An agent that only needs the glossary must\
  \ be granted\n  the same scope as one reading every article.\n- >-\n  There is no published scopes/permissions reference page on the site; the scope names\n  exist only in the discovery document.\n- >-\n  The two scopes are not referenced anywhere in the OpenAPI contract, so the REST and MCP\n  authorization models are documented in entirely separate places.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newtqnia/refs/heads/main/scopes/newtqnia-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- News API
- News
- Technology
- Artificial Intelligence
- Cybersecurity
- Developer Tools
- Cloud Computing
- Media
- Publishing
- Bilingual
token_urls: []
---
