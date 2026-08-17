---
api_specs:
- filename: parallel-chat-api-beta-api-openapi.yml
  format: yaml
  label: Parallel Chat API (Beta) API
  slug: parallel-chat-api-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-chat-api-beta-api-openapi.yml
- filename: parallel-extract-api-openapi.yml
  format: yaml
  label: Parallel Extract API
  slug: parallel-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-extract-api-openapi.yml
- filename: parallel-findall-api-openapi.yml
  format: yaml
  label: Parallel FindAll API
  slug: parallel-findall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-findall-api-openapi.yml
- filename: parallel-monitor-api-openapi.yml
  format: yaml
  label: Parallel Monitor API
  slug: parallel-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-monitor-api-openapi.yml
- filename: parallel-search-api-openapi.yml
  format: yaml
  label: Parallel Search API
  slug: parallel-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-search-api-openapi.yml
- filename: parallel-tasks-api-openapi.yml
  format: yaml
  label: Parallel Tasks API
  slug: parallel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-tasks-api-openapi.yml
- filename: parallel-responses-api-openapi.yml
  format: yaml
  label: Parallel Responses API
  slug: parallel-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-responses-api-openapi.yml
- filename: parallel-memory-api-openapi.yml
  format: yaml
  label: Parallel Memory API
  slug: parallel-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-memory-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.parallel.ai/integrations/mcp/task-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Parallel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Parallel uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Parallel
provider_slug: parallel
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: parallel-scopes
source_filename: parallel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://platform.parallel.ai/.well-known/oauth-authorization-server\nalso:\n- https://task-mcp.parallel.ai/.well-known/oauth-protected-resource\n- https://task-mcp.parallel.ai/.well-known/oauth-authorization-server\n- https://api.parallel.ai/.well-known/agent-card.json\nnotes: >-\n  The Parallel REST API itself is API-key only (x-api-key) and declares no oauth2\n  securityScheme in the OpenAPI, so derive-oauth-scopes.py finds nothing there.\n  OAuth 2.0 exists on the AGENT surfaces: the Task MCP server and the A2A Deep\n  Research agent both delegate to an authorization server at\n  platform.parallel.ai, whose published metadata declares a single scope. The\n  OAuth exchange yields a Parallel API key used as a bearer token.\nauthorization_server:\n  issuer: https://platform.parallel.ai\n  metadata_url: https://platform.parallel.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  authorization_endpoint: https://platform.parallel.ai/getKeys/authorize\n\
  \  token_endpoint: https://platform.parallel.ai/getKeys/token\n  registration_endpoint: https://platform.parallel.ai/getKeys/register\n  device_authorization_endpoint: https://platform.parallel.ai/getKeys/device/code\n  grant_types_supported:\n  - authorization_code\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types_supported: [code]\n  token_endpoint_auth_methods_supported: [none]\n  code_challenge_methods_supported: [S256]\n  dynamic_client_registration: true\n  pkce_required: true\nprotected_resources:\n- resource: https://task-mcp.parallel.ai\n  metadata_url: https://task-mcp.parallel.ai/.well-known/oauth-protected-resource\n  http_status: 200\n  authorization_servers: [https://platform.parallel.ai]\n  bearer_methods_supported: [header, body]\n  resource_documentation: https://task-mcp.parallel.ai\n- resource: https://api.parallel.ai/a2a\n  declared_in: a2a/parallel-agent-card.json (securitySchemes.parallel_oauth)\n  http_status: 401\n  note: A2A Deep Research agent;\
  \ same authorize/token endpoints.\nscopes:\n- name: key:read\n  description: >-\n    Use a Parallel API key to access the agent. Declared in the authorization\n    server metadata, the Task MCP protected-resource metadata, and the A2A agent\n    card's oauth2 authorizationCode flow.\n  surfaces:\n  - https://task-mcp.parallel.ai/mcp\n  - https://api.parallel.ai/a2a\nscope_count: 1\nnot_applicable:\n  rest_api: >-\n    https://api.parallel.ai REST endpoints use apiKey (header x-api-key) with no\n    scoping; there is no per-scope authorization on the REST surface.\n  probe_misses:\n  - {url: 'https://api.parallel.ai/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://search.parallel.ai/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://search.parallel.ai/.well-known/oauth-protected-resource', status: 404}\ndocs: https://docs.parallel.ai/integrations/mcp/task-mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/scopes/parallel-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Ai
- Web Search
- Agents
- Deep Research
- Web Extraction
- Data Enrichment
- Web Monitoring
- LLM Tools
token_urls: []
---
