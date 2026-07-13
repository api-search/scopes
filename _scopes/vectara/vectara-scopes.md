---
api_specs:
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara REST API
  slug: vectara-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Corpora API
  slug: vectara-corpora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Indexing API
  slug: vectara-indexing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Query API
  slug: vectara-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Agents API
  slug: vectara-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.vectara.com/docs/security/authentication/oauth-2
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Vectara Scopes
name_suffix: OAuth Scopes
note: Vectara's OAuth 2.0 supports only the client credentials grant and does not use or document OAuth scopes; permissions are governed by role-based access assigned to app clients at creation (https://docs.vectara.com/docs/security/authentication/oauth-2).
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
  source: openapi/vectara-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: vectara-scopes
source_filename: vectara-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vectara-openapi.yml\ndocs: https://docs.vectara.com/docs/security/authentication/oauth-2\nnote: >-\n  Vectara's OAuth 2.0 supports only the client credentials grant and does not\n  use or document OAuth scopes; permissions are governed by role-based access\n  assigned to app clients at creation\n  (https://docs.vectara.com/docs/security/authentication/oauth-2).\nschemes:\n- name: OAuth2\n  source: openapi/vectara-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.vectara.io/oauth2/token\n  description: OAuth 2.0 client credentials flow.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/scopes/vectara-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI
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
token_urls:
- https://auth.vectara.io/oauth2/token
---
