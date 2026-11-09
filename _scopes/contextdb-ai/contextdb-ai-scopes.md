---
api_specs:
- filename: contextdb-ai-decisions-api-openapi.yml
  format: yaml
  label: ContextDB Decisions API
  slug: contextdb-ai-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-decisions-api-openapi.yml
- filename: contextdb-ai-mcp-api-openapi.yml
  format: yaml
  label: ContextDB MCP API
  slug: contextdb-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-mcp-api-openapi.yml
- filename: contextdb-ai-memory-api-openapi.yml
  format: yaml
  label: ContextDB Memory API
  slug: contextdb-ai-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-memory-api-openapi.yml
- filename: contextdb-ai-meta-api-openapi.yml
  format: yaml
  label: ContextDB Meta API
  slug: contextdb-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-meta-api-openapi.yml
- filename: contextdb-ai-oauth-api-openapi.yml
  format: yaml
  label: ContextDB OAuth API
  slug: contextdb-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextdb-ai/openapi/contextdb-ai-oauth-api-openapi.yml
authorization_urls:
- https://app.contextdb.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Contextdb Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ContextDB publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ContextDB API on a user''s behalf.


  Tokens are issued from https://api.contextdb.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ContextDB
provider_slug: contextdb-ai
schemes:
- description: User-bound marketplace connector grant (`cmo_…`).
  flows:
  - authorizationUrl: https://app.contextdb.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.contextdb.ai/oauth/token
  name: McpOAuth
  source: openapi/contextdb-ai-openapi.yaml
scope_count: 3
scope_names:
- memory:read
- memory:write
- offline_access
scopes:
- description: Recall memory and evaluate evidence before actions
  flows:
  - authorizationCode
  scope: memory:read
- description: Remember, confirm, and forget memory
  flows:
  - authorizationCode
  scope: memory:write
- description: Rotate a refresh token for continued access
  flows:
  - authorizationCode
  scope: offline_access
slug: contextdb-ai-scopes
source_filename: contextdb-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/contextdb-ai-openapi.yaml\nschemes:\n- name: McpOAuth\n  source: openapi/contextdb-ai-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.contextdb.ai/oauth/authorize\n    tokenUrl: https://api.contextdb.ai/oauth/token\n  description: User-bound marketplace connector grant (`cmo_…`).\nscopes:\n- scope: memory:read\n  description: Recall memory and evaluate evidence before actions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/contextdb-ai-openapi.yaml\n- scope: memory:write\n  description: Remember, confirm, and forget memory\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/contextdb-ai-openapi.yaml\n- scope: offline_access\n  description: Rotate a refresh token for continued access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/contextdb-ai-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/contextdb-ai/scopes/contextdb-ai-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Artificial Intelligence
- Memory
- Customer Data
- Agent Platform
- Context
token_bound: false
token_urls:
- https://api.contextdb.ai/oauth/token
---
