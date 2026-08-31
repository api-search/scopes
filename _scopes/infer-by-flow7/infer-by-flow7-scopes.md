---
api_specs:
- filename: infer-by-flow7-catalog-api-openapi.yml
  format: yaml
  label: Infer by Flow7 Catalog API
  slug: infer-by-flow7-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/openapi/infer-by-flow7-catalog-api-openapi.yml
- filename: infer-by-flow7-inference-api-openapi.yml
  format: yaml
  label: Infer by Flow7 Inference API
  slug: infer-by-flow7-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/openapi/infer-by-flow7-inference-api-openapi.yml
- filename: infer-by-flow7-status-api-openapi.yml
  format: yaml
  label: Infer by Flow7 Status API
  slug: infer-by-flow7-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/openapi/infer-by-flow7-status-api-openapi.yml
authorization_urls: []
description: Infer publishes a permission scope on its API keys, but it is NOT OAuth 2.0. There is no authorization server (both /.well-known/oauth-authorization-server and /.well-known/openid-configuration return 404), no token endpoint and no consent flow. The scope is a property attached to a workspace API key at creation time. This file records that honestly rather than leaving a documented permission model unrecorded.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Infer By Flow7 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Infer by Flow7 uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Infer by Flow7
provider_slug: infer-by-flow7
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: infer-by-flow7-scopes
source_filename: infer-by-flow7-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: >-\n  https://infer.flow7.org/openapi-public.json (listModels description) and https://infer.flow7.org/docs\ndescription: >-\n  Infer publishes a permission scope on its API keys, but it is NOT OAuth 2.0. There is no\n  authorization server (both /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration return 404), no token endpoint and no consent flow. The scope is a\n  property attached to a workspace API key at creation time. This file records that honestly rather\n  than leaving a documented permission model unrecorded.\noauth2: false\nauthorization_server: null\nscheme: api-key-permission-scopes\nscope_count: 1\nscopes:\n  - name: inference:write\n    description: >-\n      Required for the authenticated operations. Infer's OpenAPI states on listModels: \"The key must\n      carry the inference:write scope.\" createResponse uses the same bearerAuth scheme.\n    operations:\n      - listModels\n\
  \      - createResponse\n    granted_by: key creation inside a verified workspace\nderived_from:\n  - openapi/infer-by-flow7-public-api-openapi.yml\nnotes:\n  - >-\n    derive-oauth-scopes.py yields nothing for this provider by design — there is no oauth2\n    securityScheme in the contract to derive from.\n  - >-\n    Spend ceilings (per-key daily and monthly microdollar limits) act as a second, orthogonal\n    authorization axis. They are recorded in authentication/ and rate-limits/, not here, because they\n    limit cost rather than capability.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/scopes/infer-by-flow7-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI/ML inference
- LLM API gateway
- Responses-compatible API
- Coding-agent tooling
- Developer Tools
- Usage-based billing
- Prepaid billing
- Agent-native
- Agent Skills
- Model routing
token_urls: []
---
