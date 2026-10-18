---
api_specs:
- filename: vectara-agents-api-openapi.yml
  format: yaml
  label: Vectara Agents API
  slug: vectara-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-agents-api-openapi.yml
- filename: vectara-authentication-api-openapi.yml
  format: yaml
  label: Vectara Authentication API
  slug: vectara-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-authentication-api-openapi.yml
- filename: vectara-corpora-api-openapi.yml
  format: yaml
  label: Vectara Corpora API
  slug: vectara-corpora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-corpora-api-openapi.yml
- filename: vectara-documents-api-openapi.yml
  format: yaml
  label: Vectara Documents API
  slug: vectara-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-documents-api-openapi.yml
- filename: vectara-pipelines-api-openapi.yml
  format: yaml
  label: Vectara Pipelines API
  slug: vectara-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-pipelines-api-openapi.yml
- filename: vectara-query-api-openapi.yml
  format: yaml
  label: Vectara Query API
  slug: vectara-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-query-api-openapi.yml
- filename: vectara-tools-api-openapi.yml
  format: yaml
  label: Vectara Tools API
  slug: vectara-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-tools-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Vectara Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Vectara uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.vectara.io/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vectara
provider_slug: vectara
schemes:
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.vectara.io/oauth2/token
  name: OAuth2
  source: openapi/vectara-agents-api-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.vectara.io/oauth2/token
  name: OAuth2
  source: openapi/vectara-authentication-api-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.vectara.io/oauth2/token
  name: OAuth2
  source: openapi/vectara-corpora-api-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.vectara.io/oauth2/token
  name: OAuth2
  source: openapi/vectara-documents-api-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.vectara.io/oauth2/token
  name: OAuth2
  source: openapi/vectara-pipelines-api-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.vectara.io/oauth2/token
  name: OAuth2
  source: openapi/vectara-query-api-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.vectara.io/oauth2/token
  name: OAuth2
  source: openapi/vectara-tools-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: vectara-scopes
source_filename: vectara-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/vectara-agents-api-openapi.yml, openapi/vectara-authentication-api-openapi.yml,\n  openapi/vectara-corpora-api-openapi.yml, openapi/vectara-documents-api-openapi.yml, openapi/vectara-pipelines-api-openapi.yml,\n  openapi/vectara-query-api-openapi.yml, openapi/vectara-tools-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/vectara-agents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.vectara.io/oauth2/token\n  description: OAuth 2.0 client credentials flow.\n- name: OAuth2\n  source: openapi/vectara-authentication-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.vectara.io/oauth2/token\n  description: OAuth 2.0 client credentials flow.\n- name: OAuth2\n  source: openapi/vectara-corpora-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.vectara.io/oauth2/token\n  description: OAuth 2.0 client credentials flow.\n\
  - name: OAuth2\n  source: openapi/vectara-documents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.vectara.io/oauth2/token\n  description: OAuth 2.0 client credentials flow.\n- name: OAuth2\n  source: openapi/vectara-pipelines-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.vectara.io/oauth2/token\n  description: OAuth 2.0 client credentials flow.\n- name: OAuth2\n  source: openapi/vectara-query-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.vectara.io/oauth2/token\n  description: OAuth 2.0 client credentials flow.\n- name: OAuth2\n  source: openapi/vectara-tools-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.vectara.io/oauth2/token\n  description: OAuth 2.0 client credentials flow.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/scopes/vectara-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Agents
- Corpora
- Embeddings
- Enterprise Search
- Generative AI
- Grounded Generation
- Hallucination Detection
- LLM
- MCP
- RAG
- Retrieval
- Search
- Semantic Search
- Vector Search
token_bound: false
token_urls:
- https://auth.vectara.io/oauth2/token
---
