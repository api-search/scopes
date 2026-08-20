---
api_specs:
- filename: ocean-io-api-openapi.yml
  format: yaml
  label: Ocean.io API
  slug: oceanio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-api-openapi.yml
authorization_urls: []
description: Ocean.io publishes RFC 8414 OAuth 2.0 Authorization Server Metadata at https://api.ocean.io/.well-known/oauth-authorization-server (HTTP 200, application/json). The document advertises a client_credentials token endpoint and an EMPTY scopes_supported array, and no public documentation page describes the flow. The REST API itself is authenticated with a single unscoped account API token, and the OpenAPI declares no oauth2 security scheme. There is therefore no scope surface to enumerate — this file records that absence with the evidence, rather than inventing one.
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Ocean Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ocean.io uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.ocean.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ocean.io
provider_slug: ocean-io
schemes:
- flows:
  - authorizationUrl: null
    flow: clientCredentials
    scopes: {}
    tokenUrl: https://api.ocean.io/oauth/token
    token_endpoint_auth_methods_supported:
    - client_secret_post
  issuer: https://api.ocean.io
  name: OAuth 2.0 (client credentials)
  source: well-known/ocean-io-oauth-authorization-server.json
scope_count: 0
scope_names: []
scopes: []
slug: ocean-io-scopes
source_filename: ocean-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.ocean.io/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Ocean.io publishes RFC 8414 OAuth 2.0 Authorization Server Metadata at\n  https://api.ocean.io/.well-known/oauth-authorization-server (HTTP 200, application/json). The\n  document advertises a client_credentials token endpoint and an EMPTY scopes_supported array, and no\n  public documentation page describes the flow. The REST API itself is authenticated with a single\n  unscoped account API token, and the OpenAPI declares no oauth2 security scheme. There is therefore\n  no scope surface to enumerate — this file records that absence with the evidence, rather than\n  inventing one.\nschemes:\n  - name: OAuth 2.0 (client credentials)\n    source: well-known/ocean-io-oauth-authorization-server.json\n    issuer: https://api.ocean.io\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.ocean.io/oauth/token\n        authorizationUrl:\
  \ null\n        token_endpoint_auth_methods_supported:\n          - client_secret_post\n        scopes: {}\nscopes: []\nscope_count: 0\nx-evidence:\n  - fetched: '2026-08-13'\n    url: https://api.ocean.io/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n    finding: scopes_supported is an empty array\n  - fetched: '2026-08-13'\n    url: https://api.ocean.io/openapi.json\n    http_status: 200\n    finding: components.securitySchemes is absent; no oauth2 scheme declared\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/scopes/ocean-io-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Sales Intelligence
- B2B
- Enrichment
- Lookalike
- Account Based Marketing
- Prospecting
- Company Data
- People Data
- Contact Data
- Segmentation
- Go-To-Market
- MCP
token_urls:
- https://api.ocean.io/oauth/token
---
