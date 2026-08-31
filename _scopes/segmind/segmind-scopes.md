---
api_specs:
- filename: segmind-inference-api-openapi.yml
  format: yaml
  label: Segmind Inference API
  slug: segmind-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-inference-api-openapi.yml
- filename: segmind-account-api-openapi.yml
  format: yaml
  label: Segmind Account API
  slug: segmind-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-account-api-openapi.yml
- filename: segmind-storage-api-openapi.yml
  format: yaml
  label: Segmind Storage API
  slug: segmind-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-storage-api-openapi.yml
- filename: segmind-fine-tuning-api-openapi.yml
  format: yaml
  label: Segmind Fine-tuning API
  slug: segmind-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-fine-tuning-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.segmind.com/docs/get-started/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Segmind Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Segmind uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Segmind
provider_slug: segmind
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: segmind-scopes
source_filename: segmind-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.segmind.com/docs/get-started/authentication\ndocs: https://docs.segmind.com/docs/get-started/authentication\nstatus: partial\nsummary: >-\n  Segmind has no published OAuth scope reference. Two scope surfaces exist and only one of\n  them belongs to Segmind. This file records exactly what is published and nothing more —\n  the scope names below are the only two that appear anywhere in Segmind's documentation.\nsegmind_scopes:\n  reference_page: null\n  note: >-\n    The only Segmind-issued scope names published anywhere are the two in the API-key\n    creation example on the authentication page. No scope reference page exists, no\n    enumeration of valid values is given, and the console is not documented as exposing\n    scope selection when a key is created. A 403 insufficient_scope error is documented,\n    so scopes are enforced somewhere, but a developer cannot discover the vocabulary.\n  scopes:\n    - name:\
  \ 'read:models'\n      description: >-\n        Appears in the documented POST /api/keys request body example. No definition is\n        published.\n      source: 'https://docs.segmind.com/docs/get-started/authentication#api-key-management'\n    - name: 'write:inference'\n      description: >-\n        Appears in the same example. No definition is published.\n      source: 'https://docs.segmind.com/docs/get-started/authentication#api-key-management'\nidentity_provider_scopes:\n  note: >-\n    These are requested BY Segmind AT the identity provider during social login. They are\n    Google/Microsoft/Discord scopes, not Segmind API scopes, and are recorded here only so\n    they are not mistaken for one.\n  providers:\n    - provider: Google\n      scopes: [email, profile]\n    - provider: Microsoft\n      scopes: ['user.read', profile, email]\n    - provider: Discord\n      scopes: [identify, email, guilds]\noauth21_server:\n  status: announced\n  scopes_published: false\n  note: >-\n \
  \   The June 2026 release notes describe an OAuth 2.1 authorization server granting\n    \"scoped, user-authorized access\" to third-party applications and MCP clients. No scope\n    vocabulary for it is published, and no authorization-server metadata document exists\n    to enumerate scopes_supported. Probed 2026-08-27:\n    platform.segmind.com/.well-known/oauth-authorization-server -> 404.\n  source: https://docs.segmind.com/docs/platform/release-notes/2026-06-21-weekly\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/scopes/segmind-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Machine Learning
- Generative AI
- Inference
- Image Generation
- Video Generation
- Text to Image
- Text to Video
- Serverless
- GPU
- Workflows
- Fine-Tuning
token_urls: []
---
