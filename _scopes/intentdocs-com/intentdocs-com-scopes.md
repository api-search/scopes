---
api_specs:
- filename: intentdocs-com-cli-api-openapi.yml
  format: yaml
  label: intentdocs-com CLI API
  slug: intentdocs-com-cli-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-cli-api-openapi.yml
- filename: intentdocs-com-mcp-api-openapi.yml
  format: yaml
  label: intentdocs-com MCP API
  slug: intentdocs-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-mcp-api-openapi.yml
- filename: intentdocs-com-oauth-api-openapi.yml
  format: yaml
  label: intentdocs-com OAuth API
  slug: intentdocs-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-oauth-api-openapi.yml
- filename: intentdocs-com-sync-api-openapi.yml
  format: yaml
  label: intentdocs-com Sync API
  slug: intentdocs-com-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-sync-api-openapi.yml
authorization_urls:
- https://intentdocs.com/api/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Intentdocs Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'intentdocs-com publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the intentdocs-com API on a user''s behalf.


  Tokens are issued from https://intentdocs.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: intentdocs-com
provider_slug: intentdocs-com
schemes:
- description: OAuth 2.1 bearer token. Obtain via /api/oauth/authorize → /api/oauth/token flow, or use intent_cli_* tokens from /api/cli/auth.
  flows:
  - authorizationUrl: https://intentdocs.com/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://intentdocs.com/api/oauth/token
  name: bearerAuth
  source: openapi/intentdocs-com-openapi.json
scope_count: 6
scope_names:
- read:maps
- read:projects
- read:specs
- write:maps
- write:projects
- write:specs
scopes:
- description: Read story map data, stories, and criteria
  flows:
  - authorizationCode
  scope: read:maps
- description: Read project metadata and story maps
  flows:
  - authorizationCode
  scope: read:projects
- description: Read generated specifications and build orders
  flows:
  - authorizationCode
  scope: read:specs
- description: Modify stories, log decisions, and report progress
  flows:
  - authorizationCode
  scope: write:maps
- description: Create and modify projects
  flows:
  - authorizationCode
  scope: write:projects
- description: Generate and update specifications
  flows:
  - authorizationCode
  scope: write:specs
slug: intentdocs-com-scopes
source_filename: intentdocs-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/intentdocs-com-openapi.json\nschemes:\n- name: bearerAuth\n  source: openapi/intentdocs-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://intentdocs.com/api/oauth/authorize\n    tokenUrl: https://intentdocs.com/api/oauth/token\n  description: OAuth 2.1 bearer token. Obtain via /api/oauth/authorize → /api/oauth/token flow,\n    or use intent_cli_* tokens from /api/cli/auth.\nscopes:\n- scope: read:maps\n  description: Read story map data, stories, and criteria\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/intentdocs-com-openapi.json\n- scope: read:projects\n  description: Read project metadata and story maps\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/intentdocs-com-openapi.json\n- scope: read:specs\n  description: Read generated specifications and build orders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/intentdocs-com-openapi.json\n- scope:\
  \ write:maps\n  description: Modify stories, log decisions, and report progress\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/intentdocs-com-openapi.json\n- scope: write:projects\n  description: Create and modify projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/intentdocs-com-openapi.json\n- scope: write:specs\n  description: Generate and update specifications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/intentdocs-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/intentdocs-com/scopes/intentdocs-com-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Spec-Driven
- Platform
- Automation
- Low-Code
token_bound: false
token_urls:
- https://intentdocs.com/api/oauth/token
---
