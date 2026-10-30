---
api_specs:
- filename: hasmcp-providers-api-openapi.yml
  format: yaml
  label: HasMCP Providers API
  slug: hasmcp-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/openapi/hasmcp-providers-api-openapi.yml
- filename: hasmcp-servers-api-openapi.yml
  format: yaml
  label: HasMCP Servers API
  slug: hasmcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/openapi/hasmcp-servers-api-openapi.yml
- filename: hasmcp-variables-api-openapi.yml
  format: yaml
  label: HasMCP Variables API
  slug: hasmcp-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/openapi/hasmcp-variables-api-openapi.yml
authorization_urls:
- https://accounts.hasmcp.com/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hasmcp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HasMCP publishes 17 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HasMCP API on a user''s behalf.


  Tokens are issued from https://accounts.hasmcp.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HasMCP
provider_slug: hasmcp
schemes:
- flows:
  - authorizationUrl: https://accounts.hasmcp.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.hasmcp.com/oauth2/token
  name: oauth2
  source: openapi/hasmcp-openapi.yaml
scope_count: 17
scope_names:
- gitconnection:delete
- gitconnection:list
- provider:create
- provider:delete
- provider:list
- provider:read
- provider:update
- server:create
- server:create_token
- server:delete
- server:list
- server:read
- server:update
- variable:create
- variable:delete
- variable:list
- variable:update
scopes:
- description: Delete Git connection
  flows:
  - authorizationCode
  scope: gitconnection:delete
- description: List Git connections
  flows:
  - authorizationCode
  scope: gitconnection:list
- description: Create provider
  flows:
  - authorizationCode
  scope: provider:create
- description: Delete provider
  flows:
  - authorizationCode
  scope: provider:delete
- description: List providers
  flows:
  - authorizationCode
  scope: provider:list
- description: Get provider
  flows:
  - authorizationCode
  scope: provider:read
- description: Update provider
  flows:
  - authorizationCode
  scope: provider:update
- description: Create MCP server
  flows:
  - authorizationCode
  scope: server:create
- description: Create MCP server token
  flows:
  - authorizationCode
  scope: server:create_token
- description: Delete MCP server
  flows:
  - authorizationCode
  scope: server:delete
- description: List MCP servers
  flows:
  - authorizationCode
  scope: server:list
- description: Get MCP server
  flows:
  - authorizationCode
  scope: server:read
- description: Update MCP server
  flows:
  - authorizationCode
  scope: server:update
- description: Create variable
  flows:
  - authorizationCode
  scope: variable:create
- description: Delete variable
  flows:
  - authorizationCode
  scope: variable:delete
- description: List variables
  flows:
  - authorizationCode
  scope: variable:list
- description: Update variable
  flows:
  - authorizationCode
  scope: variable:update
slug: hasmcp-scopes
source_filename: hasmcp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/hasmcp-openapi.yaml\nschemes:\n- name: oauth2\n  source: openapi/hasmcp-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.hasmcp.com/oauth2/auth\n    tokenUrl: https://accounts.hasmcp.com/oauth2/token\nscopes:\n- scope: gitconnection:delete\n  description: Delete Git connection\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: gitconnection:list\n  description: List Git connections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: provider:create\n  description: Create provider\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: provider:delete\n  description: Delete provider\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: provider:list\n  description: List providers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n\
  - scope: provider:read\n  description: Get provider\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: provider:update\n  description: Update provider\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: server:create\n  description: Create MCP server\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: server:create_token\n  description: Create MCP server token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: server:delete\n  description: Delete MCP server\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: server:list\n  description: List MCP servers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: server:read\n  description: Get MCP server\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: server:update\n  description: Update MCP\
  \ server\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: variable:create\n  description: Create variable\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: variable:delete\n  description: Delete variable\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: variable:list\n  description: List variables\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- scope: variable:update\n  description: Update variable\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hasmcp-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/scopes/hasmcp-scopes.yml
summary_line: 17 scopes · authorizationCode
tags:
- Company
- No-Code
- Low-Code
- MCP
- API Gateway
token_bound: false
token_urls:
- https://accounts.hasmcp.com/oauth2/token
---
