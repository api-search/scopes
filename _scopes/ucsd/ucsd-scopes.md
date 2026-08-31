---
api_specs:
- filename: ucsd-chat-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — chat
  slug: tritonai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-chat-api-openapi.yml
- filename: ucsd-completions-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — completions
  slug: tritonai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-completions-api-openapi.yml
- filename: ucsd-embeddings-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — embeddings
  slug: tritonai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-embeddings-api-openapi.yml
- filename: ucsd-models-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — models
  slug: tritonai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-models-api-openapi.yml
- filename: ucsd-images-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — images
  slug: tritonai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-images-api-openapi.yml
- filename: ucsd-audio-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — audio
  slug: tritonai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-audio-api-openapi.yml
- filename: ucsd-scim-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — SCIM 2.0 provisioning
  slug: tritonai-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-scim-api-openapi.yml
- filename: ucsd-objects-api-openapi.yml
  format: yaml
  label: University of California, San Diego Objects API
  slug: ucsd-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-objects-api-openapi.yml
- filename: ucsd-search-api-openapi.yml
  format: yaml
  label: University of California, San Diego Search API
  slug: ucsd-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-search-api-openapi.yml
authorization_urls: []
description: Authorization scopes observable on UC San Diego's institution-operated API surfaces. Both surfaces are credential-gated; the scope names below were read from endpoints that answer anonymously, not from published developer documentation, because UC San Diego does not publish a scope reference outside its Single Sign-On boundary.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ucsd Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of California, San Diego uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of California, San Diego
provider_slug: ucsd
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ucsd-scopes
source_filename: ucsd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  https://api.ucsd.edu/api/am/devportal/v2/settings (200, anonymous) and\n  https://tritonai-api.ucsd.edu/openapi.json (200)\nprovider: University of California, San Diego\nproviderId: ucsd\ndescription: >-\n  Authorization scopes observable on UC San Diego's institution-operated API surfaces. Both\n  surfaces are credential-gated; the scope names below were read from endpoints that answer\n  anonymously, not from published developer documentation, because UC San Diego does not\n  publish a scope reference outside its Single Sign-On boundary.\nsurfaces:\n  - name: UC San Diego API Gateway (WSO2 API Manager 4.1.0)\n    host: api.ucsd.edu\n    x-operator: institution\n    model: OAuth 2.0 / OpenID Connect scopes issued by the gateway's own key manager\n    evidence:\n      url: https://api.ucsd.edu/api/am/devportal/v2/settings\n      status: 200\n    notes: >-\n      The gateway reports IsAnonymousModeEnabled=false, monetizationEnabled=false\
  \ and\n      identityProvider.external=false, which is why the API catalogue itself\n      (/api/am/devportal/v2/apis) answers 401 to an unauthenticated client. The scope names are\n      WSO2 product scopes governing developer-portal actions, not per-API business scopes; the\n      per-API scopes are behind the same 401.\n    scopes:\n      - name: apim:admin\n        description: Administrative access to the developer portal.\n      - name: apim:api_key\n        description: Issue and manage API keys for a subscribed application.\n      - name: apim:app_import_export\n        description: Import and export developer-portal applications.\n      - name: apim:app_manage\n        description: Create, update and delete developer-portal applications.\n      - name: apim:store_settings\n        description: Read developer-portal settings.\n      - name: apim:sub_alert_manage\n        description: Manage subscriber alert configuration.\n      - name: apim:sub_manage\n        description: Manage\
  \ subscriptions to published APIs.\n      - name: apim:subscribe\n        description: Subscribe an application to a published API.\n      - name: openid\n        description: OpenID Connect identity scope.\n  - name: TritonAI Developer API (LiteLLM Gateway)\n    host: tritonai-api.ucsd.edu\n    x-operator: institution\n    model: Bearer token — issued TritonAI API key\n    evidence:\n      url: https://tritonai-api.ucsd.edu/openapi.json\n      status: 200\n    notes: >-\n      The gateway declares no OAuth scope vocabulary. Authorization is a single opaque\n      credential; entitlement is expressed server-side through LiteLLM key, team, budget and\n      access-group objects rather than through scopes on the wire. Access is granted to approved\n      UC San Diego faculty, staff, researchers and campus teams.\n    scopes: []\n  - name: UC San Diego Library Digital Collections JSON API\n    host: library.ucsd.edu\n    x-operator: institution\n    model: none — anonymous read\n    evidence:\n\
  \      url: https://library.ucsd.edu/dc/search.json?q=ocean\n      status: 200\n    notes: >-\n      No authorization layer. Entitlement is enforced server-side by a fixed Solr filter query\n      (discover_access_group_ssim:public OR discover_access_group_ssim:unknown), so restricted\n      and embargoed material is never returned to an anonymous client.\n    scopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/scopes/ucsd-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Public Research University
- UC System
- United States
- California
- Research
- Research Data
- Digital Collections
- Identity Federation
- API Gateway
- Artificial Intelligence
- Research Computing
token_urls: []
---
