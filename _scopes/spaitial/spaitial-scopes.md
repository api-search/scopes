---
api_specs:
- filename: spaitial-developer-api-openapi.json
  format: json
  label: SpAItial Developer API
  slug: spaitial-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaitial/refs/heads/main/openapi/spaitial-developer-api-openapi.json
authorization_urls: []
description: SpAItial API keys carry an explicit scope set enforced server-side; calls outside the granted scopes return 403 FORBIDDEN. Scopes are attached to the bearer API key (not obtained via an OAuth 2.0 authorization-code flow), and the same scopes apply to the hosted MCP server. This is the documented scope-to-endpoint mapping, captured verbatim.
docs: https://docs.spaitial.ai/api/llm-skills
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Spaitial Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SpAItial uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SpAItial
provider_slug: spaitial
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: spaitial-scopes
source_filename: spaitial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.spaitial.ai/api/llm-skills (required-scopes-per-endpoint table), https://docs.spaitial.ai/api/authentication\ndocs: https://docs.spaitial.ai/api/llm-skills\ndescription: >-\n  SpAItial API keys carry an explicit scope set enforced server-side; calls\n  outside the granted scopes return 403 FORBIDDEN. Scopes are attached to the\n  bearer API key (not obtained via an OAuth 2.0 authorization-code flow), and\n  the same scopes apply to the hosted MCP server. This is the documented\n  scope-to-endpoint mapping, captured verbatim.\nscheme: api-key-scopes\nscopes:\n  - name: worlds:create\n    description: Create world-generation jobs and edit panoramas.\n    endpoints:\n      - POST /v1/worlds\n      - POST /v1/panoramas/edit\n  - name: worlds:read\n    description: Read worlds, statuses, results, exports, download artifacts, list panoramas, and list models.\n    endpoints:\n      - GET /v1/worlds/requests\n      - GET\
  \ /v1/worlds/requests/:id\n      - GET /v1/worlds/requests/:id/status\n      - GET /v1/worlds/requests/:id/splat\n      - GET /v1/worlds/requests/:id/panorama\n      - GET /v1/worlds/requests/:id/exports\n      - GET /v1/worlds/requests/:id/exports/:type\n      - GET /v1/panoramas\n      - GET /v1/panoramas/:id\n      - GET /v1/panoramas/:id/download\n      - GET /v1/models\n  - name: worlds:write\n    description: Mutate existing worlds — update title/visibility, cancel jobs, start exports.\n    endpoints:\n      - PATCH /v1/worlds/requests/:id\n      - POST /v1/worlds/requests/:id/cancel\n      - POST /v1/worlds/requests/:id/exports/:type\n  - name: files:create\n    description: Upload input image files for later use in world generation.\n    endpoints:\n      - POST /v1/files\n  - name: files:read\n    description: List files uploaded by this API key.\n    endpoints:\n      - GET /v1/files\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaitial/refs/heads/main/scopes/spaitial-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Spatial AI
- World Models
- 3D
- Gaussian Splatting
- Generative AI
- Developer API
- MCP
token_urls: []
---
