---
api_specs:
- filename: aimlapi-api-key-management-api-openapi.yml
  format: yaml
  label: AIMLAPI API Key Management API
  slug: aimlapi-api-key-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-api-key-management-api-openapi.yml
- filename: aimlapi-assistants-api-openapi.yml
  format: yaml
  label: AIMLAPI Assistants API
  slug: aimlapi-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-assistants-api-openapi.yml
- filename: aimlapi-chat-api-openapi.yml
  format: yaml
  label: AIMLAPI Chat API
  slug: aimlapi-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-chat-api-openapi.yml
- filename: aimlapi-images-api-openapi.yml
  format: yaml
  label: AIMLAPI Images API
  slug: aimlapi-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-images-api-openapi.yml
- filename: aimlapi-models-api-openapi.yml
  format: yaml
  label: AIMLAPI Models API
  slug: aimlapi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-models-api-openapi.yml
- filename: aimlapi-threads-api-openapi.yml
  format: yaml
  label: AIMLAPI Threads API
  slug: aimlapi-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-threads-api-openapi.yml
- filename: aimlapi-threads-messages-api-openapi.yml
  format: yaml
  label: AIMLAPI Threads > Messages API
  slug: aimlapi-threads-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-threads-messages-api-openapi.yml
- filename: aimlapi-threads-runs-api-openapi.yml
  format: yaml
  label: AIMLAPI Threads > Runs API
  slug: aimlapi-threads-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-threads-runs-api-openapi.yml
- filename: aimlapi-voice-api-openapi.yml
  format: yaml
  label: AIMLAPI Voice API
  slug: aimlapi-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-voice-api-openapi.yml
- filename: aimlapi-wip-completions-api-openapi.yml
  format: yaml
  label: AIMLAPI [WIP] Completions API
  slug: aimlapi-wip-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-wip-completions-api-openapi.yml
- filename: aimlapi-inference-openapi.yml
  format: yaml
  label: AIMLAPI Inference API
  slug: aimlapi-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-inference-openapi.yml
authorization_urls: []
description: AIMLAPI has two independent permission vocabularies. OAuth scopes exist only on the MCP authorization server and are coarse — one scope covers every tool call. The finer-grained permission model lives on API keys instead, as a set of model-category scopes attached at key creation. Both are recorded here because an integrator choosing between the REST API and the MCP server is choosing between the two.
docs: https://docs.aimlapi.com/quickstart/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Aimlapi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AIMLAPI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AIMLAPI
provider_slug: aimlapi
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: aimlapi-scopes
source_filename: aimlapi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: AIMLAPI\nproviderId: aimlapi\ngenerated: '2026-08-30'\nmethod: searched\nsource: >-\n  https://auth.aimlapi.com/mcp-oauth/.well-known/oauth-authorization-server\n  (probed 200) and\n  https://docs.aimlapi.com/api-references/service-endpoints/api-key-management\ndocs: https://docs.aimlapi.com/quickstart/mcp\ndescription: >-\n  AIMLAPI has two independent permission vocabularies. OAuth scopes exist only on\n  the MCP authorization server and are coarse — one scope covers every tool call.\n  The finer-grained permission model lives on API keys instead, as a set of\n  model-category scopes attached at key creation. Both are recorded here because\n  an integrator choosing between the REST API and the MCP server is choosing\n  between the two.\noauth:\n  issuer: https://auth.aimlapi.com/mcp-oauth\n  applies_to: https://mcp.aimlapi.com/mcp\n  discovery: https://auth.aimlapi.com/mcp-oauth/.well-known/oauth-authorization-server\n\
  \  scopes:\n  - name: openid\n    description: Standard OpenID Connect scope; returns a subject identifier.\n    standard: true\n  - name: email\n    description: The account's email address.\n    standard: true\n  - name: offline_access\n    description: >-\n      Issues a refresh token so the client can re-authorize without a browser\n      round trip. Required for an agent that runs unattended.\n    standard: true\n  - name: mcp:invoke\n    description: >-\n      Permission to invoke MCP tools on the AIMLAPI server. Calls made under this\n      scope are billed to the account exactly as REST calls are.\n    standard: false\n  granularity: coarse\n  granularity_note: >-\n    ONE scope covers every tool the server exposes — model discovery, inference\n    across every modality, job management and account balance all sit behind\n    mcp:invoke. There is no read-only scope, no spend-free scope, and no way to\n    grant an agent catalogue access without also granting it the ability to spend\n\
  \    money. The API-key scopes below are finer than the OAuth scopes.\napi_key_scopes:\n  applies_to: https://api.aimlapi.com\n  assigned_at: key creation (POST /v1/keys, `scopes` array) or in the dashboard\n  source: https://docs.aimlapi.com/api-references/service-endpoints/api-key-management\n  description: >-\n    \"List of model access scopes assigned to the key. Defines which categories of\n    models can be called using this API key.\" Enumerated in the request and\n    response schemas of the key-management endpoints.\n  scopes:\n  - name: model:chat\n    description: Chat completion models.\n  - name: model:responses\n    description: The Responses-shaped inference surface.\n  - name: model:image\n    description: Image generation and editing models.\n  - name: model:audio\n    description: Audio and music generation models.\n  - name: model:video\n    description: Video generation models.\n  - name: model:embeddings\n    description: Embedding models.\n  - name: model:speech\n\
  \    description: Speech models (text-to-speech and speech-to-text).\n  - name: model:ocr\n    description: OCR models.\n  nullable: true\n  nullable_note: >-\n    The scopes array is declared nullable in both the request and the response\n    schema, so a key created with no scopes is a valid, unrestricted key. Scoping\n    is opt-in.\n  complementary_control:\n    spend_limit:\n      retention:\n      - no_reset\n      - day\n      - week\n      - month\n      threshold: USD\n      note: >-\n        Scopes bound WHAT a key may call; the spend limit bounds HOW MUCH it may\n        cost. Together they are the closest thing AIMLAPI has to an agent\n        sandbox.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/scopes/aimlapi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Machine-Learning
- AI Models
- LLM
- Image-Generation
- Video Generation
- Speech
- Embeddings
- API Gateway
- Developer Tools
token_urls: []
---
