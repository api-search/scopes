---
api_specs:
- filename: creativefabrica-generations-api-openapi.yml
  format: yaml
  label: Creative Fabrica Generations API
  slug: creativefabrica-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-generations-api-openapi.yml
- filename: creativefabrica-models-api-openapi.yml
  format: yaml
  label: Creative Fabrica Models API
  slug: creativefabrica-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-models-api-openapi.yml
- filename: creativefabrica-presets-api-openapi.yml
  format: yaml
  label: Creative Fabrica Presets API
  slug: creativefabrica-presets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-presets-api-openapi.yml
- filename: creativefabrica-voices-api-openapi.yml
  format: yaml
  label: Creative Fabrica Voices API
  slug: creativefabrica-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-voices-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.idea.ai/mcp/docs
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Creativefabrica Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Creative Fabrica publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Creative Fabrica API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Creative Fabrica
provider_slug: creativefabrica
schemes: []
scope_count: 4
scope_names:
- openid
- email
- mcp:read
- mcp:generate
scopes:
- description: Standard OpenID Connect scope. Advertised on the protected-resource metadata; obtained alongside `email` when the user signs in.
  flows: []
  scope: openid
- description: Returns the signed-in idea.ai account's email to the client.
  flows: []
  scope: email
- description: Read-only access to the idea.ai MCP tool list and read tools (browse models, get model, get preset, check generation status and cost).
  flows: []
  scope: mcp:read
- description: Access to the generating MCP tools (start a generation, edit an asset). Generations spend coins from the authorised idea.ai account.
  flows: []
  scope: mcp:generate
slug: creativefabrica-scopes
source_filename: creativefabrica-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n  - https://mcp.idea.ai/.well-known/oauth-protected-resource\n  - https://oauth.creativefabrica.com/.well-known/oauth-authorization-server\n  - https://www.idea.ai/mcp/docs\ndocs: https://www.idea.ai/mcp/docs\napplies_to: https://mcp.idea.ai/mcp\nscheme: oauth2.1\nauthorization_server: https://oauth.creativefabrica.com\nscopes:\n  - name: openid\n    description: >-\n      Standard OpenID Connect scope. Advertised on the protected-resource\n      metadata; obtained alongside `email` when the user signs in.\n  - name: email\n    description: >-\n      Returns the signed-in idea.ai account's email to the client.\n  - name: mcp:read\n    description: >-\n      Read-only access to the idea.ai MCP tool list and read tools (browse\n      models, get model, get preset, check generation status and cost).\n  - name: mcp:generate\n    description: >-\n      Access to the generating MCP tools (start a generation, edit an\n      asset).\
  \ Generations spend coins from the authorised idea.ai account.\nnotes: >-\n  Scopes apply to the idea.ai MCP server at https://mcp.idea.ai/mcp. The\n  idea.ai GenAI REST API (https://api.idea.ai/genai/v1/...) uses a static\n  bearer `sk-...` key and declares no OAuth scopes in its OpenAPI\n  (securitySchemes.bearerAuth is of type http/bearer). See\n  authentication/creativefabrica-authentication.yml.\n"
source_yaml_url: https://artifacts.apis.io/creativefabrica/scopes/creativefabrica-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Creative Marketplace
- Digital Assets
- Fonts
- Graphics
- Print on Demand
- Embroidery
- Design Tools
- Subscription Service
- Amsterdam
token_bound: false
token_urls: []
---
