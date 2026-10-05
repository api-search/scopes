---
api_specs:
- filename: machinelibrary-ai-documents-api-openapi.yml
  format: yaml
  label: Space Frontiers Documents API
  slug: machinelibrary-ai-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-documents-api-openapi.yml
- filename: machinelibrary-ai-payments-api-openapi.yml
  format: yaml
  label: Space Frontiers Payments API
  slug: machinelibrary-ai-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-payments-api-openapi.yml
- filename: machinelibrary-ai-raw-document-downloads-api-openapi.yml
  format: yaml
  label: Space Frontiers Raw document downloads API
  slug: machinelibrary-ai-raw-document-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-raw-document-downloads-api-openapi.yml
- filename: machinelibrary-ai-recognition-api-openapi.yml
  format: yaml
  label: Space Frontiers Recognition API
  slug: machinelibrary-ai-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-recognition-api-openapi.yml
- filename: machinelibrary-ai-search-api-openapi.yml
  format: yaml
  label: Space Frontiers Search API
  slug: machinelibrary-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-search-api-openapi.yml
- filename: machinelibrary-ai-conversations-api-openapi.yml
  format: yaml
  label: Space Frontiers Conversations API
  slug: machinelibrary-ai-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-conversations-api-openapi.yml
authorization_urls: []
description: ''
docs: https://api.machinelibrary.ai/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Machinelibrary Ai Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no oauth2 securityScheme (derive-oauth-scopes.py correctly found nothing); OAuth 2.1 access tokens are accepted by the REST API through the bearer_auth http scheme ("Send the same API key, or an OAuth 2.0 access token, as a Bearer token") and by the MCP server. The scope vocabulary therefore comes from the RFC 8414 / RFC 9728 metadata and auth.md, all provider-published and fetched live on 2026-09-19 and re-verified 2026-10-03, when the issuer had moved from https://api.spacefrontiers.org to https://api.machinelibrary.ai.
overview: 'Space Frontiers publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Space Frontiers API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Space Frontiers
provider_slug: machinelibrary-ai
schemes: []
scope_count: 1
scope_names:
- search
scopes:
- description: Search the corpus and retrieve research documents using the user's account credits.
  flows: []
  scope: search
slug: machinelibrary-ai-scopes
source_filename: machinelibrary-ai-scopes.yml
source_heading: OAuth Scopes
source_url: https://mcp.machinelibrary.ai/.well-known/oauth-protected-resource (scopes_supported [search])
source_yaml: "generated: '2026-10-03'\nmethod: searched\nsource: https://api.machinelibrary.ai/.well-known/oauth-authorization-server\ndocs: https://api.machinelibrary.ai/auth.md\nsources:\n- https://mcp.machinelibrary.ai/.well-known/oauth-protected-resource (scopes_supported [search])\n- https://machinelibrary.ai/.well-known/oauth-protected-resource (scopes_supported [search])\n- https://api.machinelibrary.ai/auth.md (\"Scope and policies\")\n- https://machinelibrary.ai/llms.txt (\"scope `search`\")\n- https://machinelibrary.ai/docs/api/operations (\"OAuth uses the search scope ... mandatory S256 PKCE\"; re-read 2026-10-03)\n- https://api.spacefrontiers.org/.well-known/oauth-authorization-server (legacy host; names issuer https://api.machinelibrary.ai on 2026-10-03)\nnote: >-\n  The OpenAPI declares no oauth2 securityScheme (derive-oauth-scopes.py correctly found nothing); OAuth 2.1 access\n  tokens are accepted by the REST API through the bearer_auth http scheme (\"Send the same API key,\
  \ or an OAuth 2.0\n  access token, as a Bearer token\") and by the MCP server. The scope vocabulary therefore comes from the RFC 8414 /\n  RFC 9728 metadata and auth.md, all provider-published and fetched live on 2026-09-19 and re-verified 2026-10-03,\n  when the issuer had moved from https://api.spacefrontiers.org to https://api.machinelibrary.ai.\nauthorization_server: https://api.machinelibrary.ai\nresources:\n- https://mcp.machinelibrary.ai\n- https://mcp.spacefrontiers.org\n- https://machinelibrary.ai\n- https://spacefrontiers.org\nscope_count: 1\nscopes:\n- name: search\n  description: Search the corpus and retrieve research documents using the user's account credits.\n  source: https://api.machinelibrary.ai/auth.md (\"Scope and policies\")\n  grants: [authorization_code, refresh_token, 'urn:workos:agent-auth:grant-type:claim', 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  mcp_tools: [machinelibrary_search_documents, machinelibrary_search_social, machinelibrary_fetch_document,\
  \ machinelibrary_search_in_document, machinelibrary_research, machinelibrary_search_feedback, machinelibrary_comment_on_document, machinelibrary_vote_on_comment, machinelibrary_top_up_balance]\n  mcp_tools_note: The MCP server's only scope covers all nine machinelibrary_* tools (legacy spacefrontiers_* aliases accepted). Per docs/api/operations (2026-10-03), approval lets the application search and retrieve using account credits, and publish AI-labeled comments and votes on the user's behalf.\n  note: The only scope offered; auth.md instructs clients to \"request only search\". Payment tools/endpoints are not covered by a distinct scope in the published metadata.\ngrant_types_supported:\n- authorization_code\n- refresh_token\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- urn:workos:agent-auth:grant-type:claim\npkce: S256\ndynamic_client_registration: https://api.machinelibrary.ai/v2/oauth/register\nclient_id_prefix: ml_oauth_ (new client IDs, docs/api/operations)\ntoken_endpoint_auth_methods_supported:\
  \ [none]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/scopes/machinelibrary-ai-scopes.yml
summary_line: 1 scope
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
- Agent-Native
- AI Agents
- Data
- Search
token_bound: false
token_urls: []
---
