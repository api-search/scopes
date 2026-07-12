---
authorization_urls: []
description: ''
docs: https://docs.lancedb.com/api-reference/rest
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Lancedb Scopes
name_suffix: OAuth Scopes
note: LanceDB does not publish OAuth scopes; all requests to LanceDB Cloud/Enterprise APIs authenticate with an x-api-key header and no scope-based permissions are documented (https://docs.lancedb.com/api-reference/rest).
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
  source: openapi/lance-namespace-openapi.yaml
scope_count: 0
scope_names: []
scopes: []
slug: lancedb-scopes
source_filename: lancedb-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lance-namespace-openapi.yaml\ndocs: https://docs.lancedb.com/api-reference/rest\nnote: LanceDB does not publish OAuth scopes; all requests to LanceDB Cloud/Enterprise\n  APIs authenticate with an x-api-key header and no scope-based permissions are\n  documented (https://docs.lancedb.com/api-reference/rest).\nschemes:\n- name: OAuth2\n  source: openapi/lance-namespace-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/scopes/lancedb-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Vector Database
- Multimodal
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
token_urls:
- /oauth/token
---
