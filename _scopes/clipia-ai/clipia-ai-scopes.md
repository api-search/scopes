---
api_specs:
- filename: clipia-ai-account-api-openapi.yml
  format: yaml
  label: Clipia.ai Account API
  slug: clipia-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-account-api-openapi.yml
- filename: clipia-ai-llm-api-openapi.yml
  format: yaml
  label: Clipia.ai LLM API
  slug: clipia-ai-llm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-llm-api-openapi.yml
- filename: clipia-ai-models-api-openapi.yml
  format: yaml
  label: Clipia.ai Models API
  slug: clipia-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-models-api-openapi.yml
- filename: clipia-ai-queue-api-openapi.yml
  format: yaml
  label: Clipia.ai Queue API
  slug: clipia-ai-queue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-queue-api-openapi.yml
authorization_urls: []
description: ''
docs: https://clipia.ai/en/docs/getting-started/authentication#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Clipia.ai Scopes
name_suffix: OAuth Scopes
note: These are API-key permissions, not OAuth scopes. Every key is created with both; they cannot be chosen at key creation. A request without the required permission returns 403 insufficient_scope.
overview: 'Clipia.ai publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clipia.ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clipia.ai
provider_slug: clipia-ai
schemes: []
scope_count: 2
scope_names:
- generate
- read
scopes:
- description: creating generations (POST /v1/models/{model}) and AI Gateway LLM chat (POST /v1/chat/completions)
  flows: []
  scope: generate
- description: reserved; it doesn't unlock anything extra today
  flows: []
  scope: read
slug: clipia-ai-scopes
source_filename: clipia-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clipia.ai/en/docs/getting-started/authentication#scopes\ndocs: https://clipia.ai/en/docs/getting-started/authentication#scopes\nnote: These are API-key permissions, not OAuth scopes. Every key is created with both; they cannot be chosen at key creation. A request without the required permission returns 403 insufficient_scope.\nscopes:\n- name: generate\n  description: creating generations (POST /v1/models/{model}) and AI Gateway LLM chat (POST /v1/chat/completions)\n  operations: [submitGeneration, createChatCompletion]\n- name: read\n  description: reserved; it doesn't unlock anything extra today\n"
source_yaml_url: https://artifacts.apis.io/clipia-ai/scopes/clipia-ai-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Artificial Intelligence
- Video Generation
- Image Generation
- Generative AI
- MCP
token_bound: false
token_urls: []
---
