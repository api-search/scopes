---
api_specs:
- filename: lancedb-materializedview-api-openapi.yml
  format: yaml
  label: LanceDB MaterializedView API
  slug: lancedb-materializedview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-materializedview-api-openapi.yml
- filename: lancedb-namespace-api-openapi.yml
  format: yaml
  label: LanceDB Namespace API
  slug: lancedb-namespace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-namespace-api-openapi.yml
- filename: lancedb-table-api-openapi.yml
  format: yaml
  label: LanceDB Table API
  slug: lancedb-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-table-api-openapi.yml
- filename: lancedb-transaction-api-openapi.yml
  format: yaml
  label: LanceDB Transaction API
  slug: lancedb-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/openapi/lancedb-transaction-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Lancedb Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'LanceDB uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LanceDB
provider_slug: lancedb
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/lancedb-materializedview-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/lancedb-namespace-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/lancedb-table-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/lancedb-transaction-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: lancedb-scopes
source_filename: lancedb-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/lancedb-materializedview-api-openapi.yml, openapi/lancedb-namespace-api-openapi.yml,\n  openapi/lancedb-table-api-openapi.yml, openapi/lancedb-transaction-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/lancedb-materializedview-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n- name: OAuth2\n  source: openapi/lancedb-namespace-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n- name: OAuth2\n  source: openapi/lancedb-table-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n- name: OAuth2\n  source: openapi/lancedb-transaction-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/scopes/lancedb-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Vector Search
- Multi-Modal
- Lance Format
- Lakehouse
- RAG
- Agent Memory
- Open Source
- Embeddings
- Full-Text Search
- Hybrid Search
- Columnar Storage
- Arrow
- AI Infrastructure
token_bound: false
token_urls:
- /oauth/token
---
