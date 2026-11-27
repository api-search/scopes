---
api_specs:
- filename: api-stock-com-account-management-api-openapi.yml
  format: yaml
  label: API Stock Account Management API
  slug: api-stock-com-account-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-account-management-api-openapi.yml
- filename: api-stock-com-agent-api-openapi.yml
  format: yaml
  label: API Stock Agent API
  slug: api-stock-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-agent-api-openapi.yml
- filename: api-stock-com-catalog-api-openapi.yml
  format: yaml
  label: API Stock Catalog API
  slug: api-stock-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-catalog-api-openapi.yml
- filename: api-stock-com-costs-api-openapi.yml
  format: yaml
  label: API Stock Costs API
  slug: api-stock-com-costs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-costs-api-openapi.yml
- filename: api-stock-com-generations-api-openapi.yml
  format: yaml
  label: API Stock Generations API
  slug: api-stock-com-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-generations-api-openapi.yml
- filename: api-stock-com-llm-api-openapi.yml
  format: yaml
  label: API Stock LLM API
  slug: api-stock-com-llm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-llm-api-openapi.yml
- filename: api-stock-com-task-management-api-openapi.yml
  format: yaml
  label: API Stock Task Management API
  slug: api-stock-com-task-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-stock-com/openapi/api-stock-com-task-management-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: API Stock Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'API Stock publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the API Stock API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: API Stock
provider_slug: api-stock-com
schemes: []
scope_count: 3
scope_names:
- mcp:read
- mcp:generate
- offline_access
scopes:
- description: Read-only MCP tools.
  flows: []
  scope: mcp:read
- description: MCP tools that create generations (billed against the prepaid balance).
  flows: []
  scope: mcp:generate
- description: Refresh tokens.
  flows: []
  scope: offline_access
slug: api-stock-com-scopes
source_filename: api-stock-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: https://api.api-stock.com/.well-known/oauth-protected-resource\nresource: https://api.api-stock.com/mcp\nauthorization_servers:\n- https://api-stock.com/api/auth\nauthorization_server_metadata: https://api-stock.com/.well-known/oauth-authorization-server\nbearer_methods_supported: [header]\nscopes:\n- name: mcp:read\n  description: Read-only MCP tools.\n- name: mcp:generate\n  description: MCP tools that create generations (billed against the prepaid balance).\n- name: offline_access\n  description: Refresh tokens.\n"
source_yaml_url: https://artifacts.apis.io/api-stock-com/scopes/api-stock-com-scopes.yml
summary_line: 3 scopes
tags:
- Artificial Intelligence
- Machine Learning
- LLM
- Platform
token_bound: false
token_urls: []
---
