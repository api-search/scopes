---
api_specs:
- filename: viewmax-studio-account-api-openapi.yml
  format: yaml
  label: ViewMax Studio Account API
  slug: viewmax-studio-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-account-api-openapi.yml
- filename: viewmax-studio-advanced-api-openapi.yml
  format: yaml
  label: ViewMax Studio Advanced API
  slug: viewmax-studio-advanced-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-advanced-api-openapi.yml
- filename: viewmax-studio-catalog-api-openapi.yml
  format: yaml
  label: ViewMax Studio Catalog API
  slug: viewmax-studio-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-catalog-api-openapi.yml
- filename: viewmax-studio-generation-api-openapi.yml
  format: yaml
  label: ViewMax Studio Generation API
  slug: viewmax-studio-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-generation-api-openapi.yml
- filename: viewmax-studio-tasks-api-openapi.yml
  format: yaml
  label: ViewMax Studio Tasks API
  slug: viewmax-studio-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viewmax-studio/openapi/viewmax-studio-tasks-api-openapi.yml
authorization_urls:
- https://viewmax.studio/api/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Viewmax Studio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ViewMax Studio publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ViewMax Studio API on a user''s behalf.


  Tokens are issued from https://viewmax.studio/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ViewMax Studio
provider_slug: viewmax-studio
schemes:
- description: 'OAuth 2.0 for the ViewMax MCP server (`/api/mcp`) only. REST endpoints accept API keys, not OAuth tokens. Discovery: `/.well-known/oauth-protected-resource/api/mcp` and `/.well-known/oauth-authorization-server/api/auth`.'
  flows:
  - authorizationUrl: https://viewmax.studio/api/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://viewmax.studio/api/auth/oauth2/token
  name: oauth2
  source: openapi/viewmax-studio-openapi.json
scope_count: 4
scope_names:
- credits:read
- models:read
- tasks:read
- tasks:write
scopes:
- description: Read the remaining credit balance for the authenticated account.
  flows:
  - authorizationCode
  scope: credits:read
- description: Read the public model and voice catalogs without creating generation tasks.
  flows:
  - authorizationCode
  scope: models:read
- description: Read generation task status and output URLs for the authenticated account.
  flows:
  - authorizationCode
  scope: tasks:read
- description: Create credit-consuming video, image, music, speech, and sound-effect tasks.
  flows:
  - authorizationCode
  scope: tasks:write
slug: viewmax-studio-scopes
source_filename: viewmax-studio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/viewmax-studio-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/viewmax-studio-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://viewmax.studio/api/auth/oauth2/authorize\n    tokenUrl: https://viewmax.studio/api/auth/oauth2/token\n  description: 'OAuth 2.0 for the ViewMax MCP server (`/api/mcp`) only. REST endpoints accept\n    API keys, not OAuth tokens. Discovery: `/.well-known/oauth-protected-resource/api/mcp` and\n    `/.well-known/oauth-authorization-server/api/auth`.'\nscopes:\n- scope: credits:read\n  description: Read the remaining credit balance for the authenticated account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/viewmax-studio-openapi.json\n- scope: models:read\n  description: Read the public model and voice catalogs without creating generation tasks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/viewmax-studio-openapi.json\n- scope:\
  \ tasks:read\n  description: Read generation task status and output URLs for the authenticated account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/viewmax-studio-openapi.json\n- scope: tasks:write\n  description: Create credit-consuming video, image, music, speech, and sound-effect tasks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/viewmax-studio-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/viewmax-studio/scopes/viewmax-studio-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Video
- Generation
- Marketing
token_bound: false
token_urls:
- https://viewmax.studio/api/auth/oauth2/token
---
