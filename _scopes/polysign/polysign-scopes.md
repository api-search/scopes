---
api_specs:
- filename: polysign-atomicnet-api-server-openapi.json
  format: json
  label: AtomicNet API Server
  slug: atomicnet-api-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-atomicnet-api-server-openapi.json
- filename: polysign-merchant-gate-openapi.json
  format: json
  label: AtomicNet Merchant Gate Node
  slug: atomicnet-merchant-gate-node
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-merchant-gate-openapi.json
- filename: polysign-abc-proxy-service-openapi.json
  format: json
  label: AtomicNet ABC Proxy Service
  slug: atomicnet-abc-proxy-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-proxy-service-openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Polysign Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PolySign publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PolySign API on a user''s behalf.


  Tokens are issued from /v1/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PolySign
provider_slug: polysign
schemes:
- description: OAuth 2.0 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/auth/token
  name: OAuth2
  source: openapi/polysign-abc-proxy-service-openapi.json
- description: OAuth 2.0 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/auth/token
  name: OAuth2
  source: openapi/polysign-atomicnet-api-server-openapi.json
- description: OAuth 2.0 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/auth/token
  name: OAuth2
  source: openapi/polysign-merchant-gate-openapi.json
scope_count: 1
scope_names:
- participant
scopes:
- description: Grants access to participant.
  flows:
  - clientCredentials
  scope: participant
slug: polysign-scopes
source_filename: polysign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/polysign-abc-proxy-service-openapi.json, openapi/polysign-atomicnet-api-server-openapi.json,\n  openapi/polysign-merchant-gate-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/polysign-abc-proxy-service-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n  description: OAuth 2.0 with the client credentials grant flow.\n- name: OAuth2\n  source: openapi/polysign-atomicnet-api-server-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n  description: OAuth 2.0 with the client credentials grant flow.\n- name: OAuth2\n  source: openapi/polysign-merchant-gate-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n  description: OAuth 2.0 with the client credentials grant flow.\nscopes:\n- scope: participant\n  description: Grants access to participant.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/polysign-abc-proxy-service-openapi.json\n\
  \  - openapi/polysign-atomicnet-api-server-openapi.json\n  - openapi/polysign-merchant-gate-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/scopes/polysign-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- digital-assets
- blockchain
- institutional-custody
- settlement
- escrow
- capital-markets
- payments
- fintech
- distributed-ledger
- atomicnet
token_urls:
- /v1/auth/token
---
