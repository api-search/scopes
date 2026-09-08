---
api_specs:
- filename: eden-ai-audio-features-openapi.json
  format: json
  label: Eden AI Audio API
  slug: eden-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-audio-features-openapi.json
- filename: eden-ai-image-features-openapi.json
  format: json
  label: Eden AI Image API
  slug: eden-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-image-features-openapi.json
- filename: eden-ai-ocr-features-openapi.json
  format: json
  label: Eden AI OCR API
  slug: eden-ai-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-ocr-features-openapi.json
- filename: eden-ai-text-features-openapi.json
  format: json
  label: Eden AI Text API
  slug: eden-ai-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-text-features-openapi.json
- filename: eden-ai-translation-features-openapi.json
  format: json
  label: Eden AI Translation API
  slug: eden-ai-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-translation-features-openapi.json
- filename: eden-ai-v3-openapi.json
  format: json
  label: Eden AI API V3
  slug: eden-ai-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-v3-openapi.json
- filename: eden-ai-video-features-openapi.json
  format: json
  label: Eden AI Video API
  slug: eden-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-video-features-openapi.json
- filename: eden-ai-llm-features-openapi.json
  format: json
  label: Eden AI LLM API (v2)
  slug: eden-ai-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-llm-features-openapi.json
- filename: eden-ai-multimodal-features-openapi.json
  format: json
  label: Eden AI Multimodal API
  slug: eden-ai-multimodal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-multimodal-features-openapi.json
- filename: eden-ai-user-management-openapi.json
  format: json
  label: Eden AI User Management API
  slug: eden-ai-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-user-management-openapi.json
- filename: eden-ai-cost-monitoring-openapi.json
  format: json
  label: Eden AI Cost Monitoring API
  slug: eden-ai-cost-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-cost-monitoring-openapi.json
- filename: eden-ai-organization-management-openapi.json
  format: json
  label: Eden AI Organization Management API
  slug: eden-ai-organization-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-organization-management-openapi.json
authorization_urls: []
description: ''
docs: https://www.edenai.co/docs/v3/organization/management-api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Eden Ai Scopes
name_suffix: OAuth Scopes
note: These are NOT OAuth 2.0 scopes — Eden AI publishes no oauth2 securityScheme and serves no authorization-server metadata. They are explicit scopes carried by a management key (mgmt-eden-...) and checked per management endpoint, documented by Eden AI in the Management API reference and repeated in the operation descriptions of openapi/_original/eden-ai-organization-management-openapi.json. Recorded here because the scope surface is real and machine-relevant even though the grant mechanism is key issuance rather than an authorization flow.
overview: 'Eden AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Eden AI
provider_slug: eden-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: eden-ai-scopes
source_filename: eden-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://www.edenai.co/docs/v3/organization/management-api\ndocs: https://www.edenai.co/docs/v3/organization/management-api\nmodel: api-key-scopes\noauth2: false\nnote: >-\n  These are NOT OAuth 2.0 scopes — Eden AI publishes no oauth2 securityScheme and serves no\n  authorization-server metadata. They are explicit scopes carried by a management key\n  (mgmt-eden-...) and checked per management endpoint, documented by Eden AI in the Management API\n  reference and repeated in the operation descriptions of\n  openapi/_original/eden-ai-organization-management-openapi.json. Recorded here because the scope\n  surface is real and machine-relevant even though the grant mechanism is key issuance rather than\n  an authorization flow.\nscopes:\n  - name: manage:mint\n    description: >-\n      Mint and revoke management (worker) keys. Held by an ISSUER key, which can do nothing else —\n      it cannot read, write, or call inference,\
  \ and it can never mint another issuer key.\n    operations:\n      - {method: POST, path: /v3/manage/auth-keys, operationId: manage_auth_keys_create}\n      - {method: GET, path: /v3/manage/auth-keys, operationId: manage_auth_keys_retrieve}\n      - {method: DELETE, path: '/v3/manage/auth-keys/{key_id}', operationId: manage_auth_keys_destroy}\n  - name: manage:read\n    description: Read the organization — inference keys, members, IdP-synced groups, usage, and key introspection. Org-scoped.\n    operations:\n      - {method: GET, path: /v3/manage/keys, operationId: manage_keys_list}\n      - {method: GET, path: '/v3/manage/keys/{key_id}', operationId: manage_keys_retrieve}\n      - {method: GET, path: '/v3/manage/keys/{key_id}/usage', operationId: manage_keys_usage_retrieve}\n      - {method: GET, path: /v3/manage/members, operationId: manage_members_list}\n      - {method: GET, path: /v3/manage/groups, operationId: manage_groups_list}\n      - {method: GET, path: '/v3/manage/groups/{external_group_id}',\
  \ operationId: manage_groups_retrieve}\n      - {method: GET, path: /v3/manage/usage, operationId: manage_usage_retrieve}\n  - name: manage:write\n    description: >-\n      Mint, update, rotate and revoke inference keys (sk-eden-...) and set member RBAC roles.\n      This is the scope that can create a credential which spends money.\n    operations:\n      - {method: POST, path: /v3/manage/keys, operationId: manage_keys_create}\n      - {method: PATCH, path: '/v3/manage/keys/{key_id}', operationId: manage_keys_partial_update}\n      - {method: DELETE, path: '/v3/manage/keys/{key_id}', operationId: manage_keys_destroy}\n      - {method: POST, path: '/v3/manage/keys/{key_id}/rotate', operationId: manage_keys_rotate_create}\n      - {method: PATCH, path: '/v3/manage/members/{email}/role', operationId: manage_members_role_partial_update}\n  - name: (none)\n    description: >-\n      GET /v3/manage/whoami requires only a valid management key with no scope at all — enough to\n      prove the\
  \ auth path end to end without granting any read.\n    operations:\n      - {method: GET, path: /v3/manage/whoami, operationId: manage_whoami_retrieve}\ninference_surface:\n  scoped: false\n  note: >-\n    The inference surface (v3 chat/completions, universal-ai, embeddings, images, audio, upload) has\n    NO scope model. An inference key is all-or-nothing on inference; spend is bounded by per-key\n    budget (balance / balance_reset_period / balance_reset_amount), expiry, and guardrails rather\n    than by scopes.\n  docs: https://www.edenai.co/docs/v3/organization/guardrails\nscope_count: 4\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/scopes/eden-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- AI Gateway
- LLM
- Machine Learning
- OCR
- Translation
- Speech
- Computer Vision
- Model Context Protocol
- Emotion Detection
token_urls: []
---
