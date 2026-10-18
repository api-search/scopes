---
api_specs:
- filename: inflection-chat-api-openapi.yml
  format: yaml
  label: Inflection AI Chat API
  slug: inflection-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-chat-api-openapi.yml
- filename: inflection-discovery-api-openapi.yml
  format: yaml
  label: Inflection AI Discovery API
  slug: inflection-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-discovery-api-openapi.yml
- filename: inflection-embeddings-api-openapi.yml
  format: yaml
  label: Inflection AI Embeddings API
  slug: inflection-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-embeddings-api-openapi.yml
- filename: inflection-external-api-openapi.yml
  format: yaml
  label: Inflection AI External API
  slug: inflection-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-external-api-openapi.yml
- filename: inflection-status-api-openapi.yml
  format: yaml
  label: Inflection AI Status API
  slug: inflection-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-status-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Inflection Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Inflection AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Inflection AI
provider_slug: inflection
schemes:
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/inflection-chat-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/inflection-discovery-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/inflection-embeddings-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/inflection-external-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/inflection-status-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: inflection-scopes
source_filename: inflection-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/inflection-chat-api-openapi.yml, openapi/inflection-discovery-api-openapi.yml,\n  openapi/inflection-embeddings-api-openapi.yml, openapi/inflection-external-api-openapi.yml,\n  openapi/inflection-status-api-openapi.yml\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/inflection-chat-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\n- name: OAuth2PasswordBearer\n  source: openapi/inflection-discovery-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\n- name: OAuth2PasswordBearer\n  source: openapi/inflection-embeddings-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\n- name: OAuth2PasswordBearer\n  source: openapi/inflection-external-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\n- name: OAuth2PasswordBearer\n  source: openapi/inflection-status-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\nscopes: []\nnote: The OAuth2\
  \ security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/scopes/inflection-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- LLM
- Personal AI
- PI
- Foundation Models
- Empathetic AI
token_bound: false
token_urls:
- token
---
