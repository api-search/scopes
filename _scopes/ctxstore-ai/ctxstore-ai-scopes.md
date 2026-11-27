---
api_specs:
- filename: ctxstore-ai-account-api-openapi.yml
  format: yaml
  label: ctxstore.ai Account API
  slug: ctxstore-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-account-api-openapi.yml
- filename: ctxstore-ai-admin-api-openapi.yml
  format: yaml
  label: ctxstore.ai Admin API
  slug: ctxstore-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-admin-api-openapi.yml
- filename: ctxstore-ai-context-api-openapi.yml
  format: yaml
  label: ctxstore.ai Context API
  slug: ctxstore-ai-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-context-api-openapi.yml
- filename: ctxstore-ai-events-api-openapi.yml
  format: yaml
  label: ctxstore.ai Events API
  slug: ctxstore-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-events-api-openapi.yml
- filename: ctxstore-ai-facts-api-openapi.yml
  format: yaml
  label: ctxstore.ai Facts API
  slug: ctxstore-ai-facts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-facts-api-openapi.yml
- filename: ctxstore-ai-openapi-json-api-openapi.yml
  format: yaml
  label: ctxstore.ai Openapi.json API
  slug: ctxstore-ai-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-openapi-json-api-openapi.yml
- filename: ctxstore-ai-search-api-openapi.yml
  format: yaml
  label: ctxstore.ai Search API
  slug: ctxstore-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-search-api-openapi.yml
- filename: ctxstore-ai-stats-api-openapi.yml
  format: yaml
  label: ctxstore.ai Stats API
  slug: ctxstore-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-stats-api-openapi.yml
- filename: ctxstore-ai-users-api-openapi.yml
  format: yaml
  label: ctxstore.ai Users API
  slug: ctxstore-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctxstore-ai/openapi/ctxstore-ai-users-api-openapi.yml
authorization_urls: []
description: ''
docs: https://ctxstore.ai/llms-full.txt
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: ctxstore.ai Scopes
name_suffix: OAuth Scopes
note: OAuth 2.1 is documented for the MCP server only; the REST OpenAPI declares bearer API keys and no oauth2 scheme. Scope descriptions are not published beyond the names.
overview: 'ctxstore.ai publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ctxstore.ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ctxstore.ai
provider_slug: ctxstore-ai
schemes: []
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Scope named in the docs ("scopes mcp:read mcp:write"); no further description published.
  flows: []
  scope: mcp:read
- description: Scope named in the docs ("scopes mcp:read mcp:write"); no further description published.
  flows: []
  scope: mcp:write
slug: ctxstore-ai-scopes
source_filename: ctxstore-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://ctxstore.ai/llms-full.txt\ndocs: https://ctxstore.ai/llms-full.txt\nnote: OAuth 2.1 is documented for the MCP server only; the REST OpenAPI declares bearer API keys and no oauth2 scheme. Scope descriptions are not published beyond the names.\nscopes:\n- name: mcp:read\n  scheme: OAuth 2.1 (MCP)\n  description: Scope named in the docs (\"scopes mcp:read mcp:write\"); no further description published.\n- name: mcp:write\n  scheme: OAuth 2.1 (MCP)\n  description: Scope named in the docs (\"scopes mcp:read mcp:write\"); no further description published.\n"
source_yaml_url: https://artifacts.apis.io/ctxstore-ai/scopes/ctxstore-ai-scopes.yml
summary_line: 2 scopes
tags:
- Company
- AI Agents
- Memory
- MCP
- Context Management
- Developer Tools
token_bound: false
token_urls: []
---
