---
api_specs:
- filename: lets-enhance-claid-openapi.json
  format: json
  label: Claid API
  slug: claid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lets-enhance/refs/heads/main/openapi/lets-enhance-claid-openapi.json
authorization_urls: []
description: ''
docs: https://docs.claid.ai/authentication
flows:
- password
kind: oauth-scopes
layout: scope
method: searched
name: Lets Enhance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Let''s Enhance publishes 4 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Let''s Enhance API on a user''s behalf.


  Tokens are issued from token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Let's Enhance
provider_slug: lets-enhance
schemes:
- description: 'OAuth 2.0 bearer token (API key) authorization. Send requests over HTTPS with `Authorization: Bearer <YOUR_API_KEY>`; no password is required.'
  flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/lets-enhance-claid-openapi.json
  type: oauth2
scope_count: 4
scope_names:
- image_editing
- image_generation
- video_generation
- storage
scopes:
- description: Image editing operations — synchronous and asynchronous edit pipelines, batch edit, direct upload edit, natural-language AI edit, AI fashion models, and image generation.
  flows: []
  scope: image_editing
- description: AI background scene creation.
  flows: []
  scope: image_generation
- description: Image-to-video generation and job status retrieval.
  flows: []
  scope: video_generation
- description: Storage connector management — list storage types, and create, read, update and delete connected AWS S3, Google Cloud Storage and web folder storages.
  flows: []
  scope: storage
slug: lets-enhance-scopes
source_filename: lets-enhance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lets-enhance-claid-openapi.json\ndocs: https://docs.claid.ai/authentication\nnotes: >-\n  Scope strings are taken verbatim from the `security` requirements of the OpenAPI 3.1 definitions\n  Claid publishes for each endpoint in its API reference. The Claid dashboard presents these to\n  developers as coarser permission groups — Storage, Image editing, or both under Admin — assigned\n  per API key at creation time or later via API keys -> Edit key.\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/lets-enhance-claid-openapi.json\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: token\n  description: >-\n    OAuth 2.0 bearer token (API key) authorization. Send requests over HTTPS with\n    `Authorization: Bearer <YOUR_API_KEY>`; no password is required.\nscopes:\n- scope: image_editing\n  description: >-\n    Image editing operations — synchronous and asynchronous edit pipelines, batch edit, direct\n\
  \    upload edit, natural-language AI edit, AI fashion models, and image generation.\n  dashboard_group: Image editing\n  operations:\n  - POST /v1/image/edit\n  - POST /v1/image/edit/async\n  - GET /v1/image/edit/async/{task_id}\n  - POST /v1/image/edit/batch\n  - GET /v1/image/edit/batch/{task_id}\n  - POST /v1/image/edit/upload\n  - POST /v1/image/ai-edit\n  - GET /v1/image/ai-edit/{ai_edit_id}\n  - POST /v1/image/ai-fashion-models\n  - GET /v1/image/ai-fashion-models/{processing_request_id}\n  - POST /v1/image/generate\n  sources:\n  - openapi/lets-enhance-claid-openapi.json\n- scope: image_generation\n  description: AI background scene creation.\n  dashboard_group: Image editing\n  operations:\n  - POST /v1/scene/create\n  sources:\n  - openapi/lets-enhance-claid-openapi.json\n- scope: video_generation\n  description: Image-to-video generation and job status retrieval.\n  dashboard_group: Image editing\n  operations:\n  - POST /v1/video/generate\n  - GET /v1/video/generate/{animation_id}\n\
  \  sources:\n  - openapi/lets-enhance-claid-openapi.json\n- scope: storage\n  description: >-\n    Storage connector management — list storage types, and create, read, update and delete\n    connected AWS S3, Google Cloud Storage and web folder storages.\n  dashboard_group: Storage\n  operations:\n  - GET /v1/storage/storage-types\n  - GET /v1/storage/storages\n  - POST /v1/storage/storages\n  - GET /v1/storage/storages/{storage_id}\n  - PATCH /v1/storage/storages/{storage_id}\n  - DELETE /v1/storage/storages/{storage_id}\n  sources:\n  - openapi/lets-enhance-claid-openapi.json\ndashboard_permission_groups:\n- name: Storage\n  scopes:\n  - storage\n- name: Image editing\n  scopes:\n  - image_editing\n  - image_generation\n  - video_generation\n- name: Admin\n  description: Both Storage and Image editing permissions.\n  scopes:\n  - storage\n  - image_editing\n  - image_generation\n  - video_generation\nguidance: >-\n  Claid recommends creating API keys with the minimal permission scopes\
  \ necessary for the use case.\n  A request made with a key lacking the required scope returns HTTP 403 \"Not enough permissions\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lets-enhance/refs/heads/main/scopes/lets-enhance-scopes.yml
summary_line: 4 scopes · password
tags:
- Company
- Artificial Intelligence
- Image Processing
- Image Enhancement
- Image Generation
- Computer Vision
- Ecommerce
- Media
- Photography
- Video Generation
token_urls:
- token
---
