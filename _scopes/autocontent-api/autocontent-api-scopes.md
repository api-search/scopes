---
api_specs:
- filename: autocontent-api-content-api-openapi.yml
  format: yaml
  label: AutoContent API Content API
  slug: autocontent-api-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-content-api-openapi.yml
- filename: autocontent-api-dedicated-account-api-openapi.yml
  format: yaml
  label: AutoContent API Dedicated Account API
  slug: autocontent-api-dedicated-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-dedicated-account-api-openapi.yml
- filename: autocontent-api-podcast-api-openapi.yml
  format: yaml
  label: AutoContent API Podcast API
  slug: autocontent-api-podcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-podcast-api-openapi.yml
- filename: autocontent-api-share-api-openapi.yml
  format: yaml
  label: AutoContent API Share API
  slug: autocontent-api-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-share-api-openapi.yml
- filename: autocontent-api-video-api-openapi.yml
  format: yaml
  label: AutoContent API Video API
  slug: autocontent-api-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-video-api-openapi.yml
- filename: autocontent-api-platform-v1-openapi.json
  format: json
  label: AutoContent Platform API v1
  slug: platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-platform-v1-openapi.json
- filename: autocontent-api-legacy-content-openapi.json
  format: json
  label: AutoContent legacy Content API
  slug: legacy-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/openapi/autocontent-api-legacy-content-openapi.json
authorization_urls: []
description: Eight OAuth scopes across two products. The Platform API declares a required scope on every one of its 55 operations via x-required-scopes, so the mapping below is read from the contract rather than inferred. Two legacy scopes cover the older MCP resource.
docs: https://autocontentapi.com/developers/api
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Autocontent Api Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AutoContent API uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AutoContent API
provider_slug: autocontent-api
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: autocontent-api-scopes
source_filename: autocontent-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  scopes_supported in https://auth.autocontentapi.com/.well-known/oauth-authorization-server\n  (fetched 2026-09-04, saved at well-known/autocontent-api-auth-oauth-authorization-server.json),\n  cross-checked against x-required-scopes on every operation in\n  openapi/autocontent-api-platform-v1-openapi.json and the scope table at\n  https://autocontentapi.com/developers/api.\ndocs: https://autocontentapi.com/developers/api\ndescription: >-\n  Eight OAuth scopes across two products. The Platform API declares a required scope on every one\n  of its 55 operations via x-required-scopes, so the mapping below is read from the contract rather\n  than inferred. Two legacy scopes cover the older MCP resource.\nauthorization_server: https://auth.autocontentapi.com\ngrant_types:\n- authorization_code\n- refresh_token\npkce: S256\ndynamic_client_registration: https://auth.autocontentapi.com/reg\nscopes:\n- name: platform.read\n  product:\
  \ Platform API v1\n  description: >-\n    Read Projects, Collections, Sources, Assets, Generations, Content Loops, Content Loop Runs and\n    the account record, plus the Asset Type / Model / Voice / Avatar discovery endpoints.\n  operations: 21\n  examples:\n  - listProjects\n  - getProject\n  - listSources\n  - getSource\n  - listAssetTypes\n  - listModels\n  - listVoices\n  - listAvatars\n  - listGenerations\n  - getGeneration\n  - listAssets\n  - getAsset\n  - listContentLoops\n  - getContentLoop\n  - listContentLoopRuns\n  - getContentLoopRun\n  - getAccount\n- name: platform.write\n  product: Platform API v1\n  description: >-\n    Create and mutate Projects, Collections, Sources, logos, Asset feedback, Content Loop Run\n    feedback and webhook destinations.\n  examples:\n  - createProject\n  - updateProject\n  - archiveProject\n  - replaceProjectLogo\n  - removeProjectLogo\n  - refreshProject\n  - createCollection\n  - updateCollection\n  - deleteCollection\n  - createSource\n\
  \  - removeSource\n  - refreshSource\n  - recordAssetFeedback\n  - recordContentLoopRunFeedback\n  - createWebhook\n  - listWebhooks\n  - deleteWebhook\n- name: platform.generate\n  product: Platform API v1\n  description: >-\n    Spend money. Preview and create Generations and full-Asset edits, cancel Generations, run\n    Content Loops, and create or revoke custom Voices and Avatars.\n  spends: true\n  examples:\n  - previewGeneration\n  - createGeneration\n  - previewGenerationEdit\n  - createGenerationEdit\n  - cancelGeneration\n  - runContentLoop\n  - createVoice\n  - revokeVoice\n  - createAvatar\n  - revokeAvatar\n  note: >-\n    Content Loop create/update/archive require BOTH platform.write and platform.generate, because\n    a Loop is a standing authorization to spend.\n- name: platform.billing.read\n  product: Platform API v1\n  description: Read authoritative usage and prepaid service balance.\n  examples:\n  - getBillingUsage\n- name: platform.billing.write\n  product: Platform\
  \ API v1\n  description: >-\n    Create a prepaid Checkout session to add USD service balance. The docs call this the OAuth-only\n    prepayment endpoint.\n  examples:\n  - createPrepaymentSession\n  note: >-\n    NOT requested by the Platform MCP — the MCP WWW-Authenticate challenge asks only for\n    platform.read, platform.write, platform.generate and platform.billing.read, so an MCP client\n    cannot move money into the account.\n- name: platform.keys.write\n  product: Platform API v1\n  description: Mint, list and revoke scoped Platform API keys.\n  examples:\n  - createApiKey\n  - listApiKeys\n  - revokeApiKey\n  note: >-\n    Credential minting. Also outside the Platform MCP's requested scope set. listApiKeys requires\n    the write scope, so there is no read-only view of an account's keys.\n- name: content.create\n  product: Legacy AutoContent MCP\n  description: Create content through the legacy AutoContent MCP resource.\n  resource: https://mcp.autocontentapi.com/mcp\n- name:\
  \ content.status\n  product: Legacy AutoContent MCP\n  description: Read the status of legacy content requests.\n  resource: https://mcp.autocontentapi.com/mcp\nmcp_scope_sets:\n- endpoint: https://mcp.autocontentapi.com/v1\n  scopes: [platform.read, platform.write, platform.generate, platform.billing.read]\n  evidence: WWW-Authenticate header on an anonymous POST, 2026-09-04.\n- endpoint: https://mcp.autocontentapi.com/mcp\n  scopes: [content.create, content.status]\n  evidence: https://mcp.autocontentapi.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/scopes/autocontent-api-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Audio
- Content Generation
- Podcasts
- Video
- Generative AI
- Text-to-Speech
- Automation
token_urls: []
---
