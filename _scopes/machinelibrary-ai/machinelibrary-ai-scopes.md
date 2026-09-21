---
api_specs:
- filename: machinelibrary-ai-openapi.yml
  format: yaml
  label: Machine Library API
  slug: machine-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-openapi.yml
authorization_urls: []
description: ''
docs: https://api.machinelibrary.ai/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Machinelibrary Ai Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no oauth2 securityScheme (derive-oauth-scopes.py correctly found nothing); OAuth 2.1 access tokens are accepted by the REST API through the bearer_auth http scheme ("Send the same API key, or an OAuth 2.0 access token, as a Bearer token") and by the MCP server. The scope vocabulary therefore comes from the RFC 8414 / RFC 9728 metadata and auth.md, all provider-published and fetched live on 2026-09-19.
overview: 'Space Frontiers uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Space Frontiers
provider_slug: machinelibrary-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: machinelibrary-ai-scopes
source_filename: machinelibrary-ai-scopes.yml
source_heading: OAuth Scopes
source_url: https://mcp.machinelibrary.ai/.well-known/oauth-protected-resource (scopes_supported [search])
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.spacefrontiers.org/.well-known/oauth-authorization-server\ndocs: https://api.machinelibrary.ai/auth.md\nsources:\n- https://mcp.machinelibrary.ai/.well-known/oauth-protected-resource (scopes_supported [search])\n- https://machinelibrary.ai/.well-known/oauth-protected-resource (scopes_supported [search])\n- https://api.machinelibrary.ai/auth.md (\"Scope and policies\")\n- https://machinelibrary.ai/llms.txt (\"OAuth scopes (search)\")\nnote: >-\n  The OpenAPI declares no oauth2 securityScheme (derive-oauth-scopes.py correctly found nothing); OAuth 2.1 access\n  tokens are accepted by the REST API through the bearer_auth http scheme (\"Send the same API key, or an OAuth 2.0\n  access token, as a Bearer token\") and by the MCP server. The scope vocabulary therefore comes from the RFC 8414 /\n  RFC 9728 metadata and auth.md, all provider-published and fetched live on 2026-09-19.\nauthorization_server: https://api.spacefrontiers.org\n\
  resources:\n- https://mcp.machinelibrary.ai\n- https://mcp.spacefrontiers.org\n- https://machinelibrary.ai\n- https://spacefrontiers.org\nscope_count: 1\nscopes:\n- name: search\n  description: Search the corpus and retrieve research documents using the user's account credits.\n  source: https://api.machinelibrary.ai/auth.md (\"Scope and policies\")\n  grants: [authorization_code, refresh_token, 'urn:workos:agent-auth:grant-type:claim', 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  mcp_tools: [spacefrontiers_search_documents, spacefrontiers_search_social, spacefrontiers_fetch_document, spacefrontiers_search_in_document]\n  note: The only scope offered; auth.md instructs clients to \"request only search\". Payment tools/endpoints are not covered by a distinct scope in the published metadata.\ngrant_types_supported:\n- authorization_code\n- refresh_token\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- urn:workos:agent-auth:grant-type:claim\npkce: S256\ndynamic_client_registration:\
  \ https://api.spacefrontiers.org/v2/oauth/register\ntoken_endpoint_auth_methods_supported: [none]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/scopes/machinelibrary-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Research
- Scholarly Search
- Full-Text Search
- Retrieval
- RAG
- Patents
- Documents
- OCR
- Document Recognition
- MCP
- A2A
- agent-native
- AI Agents
- Data
- Search
token_urls: []
---
