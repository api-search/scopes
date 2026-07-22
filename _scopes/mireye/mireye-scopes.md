---
api_specs:
- filename: mireye-openapi-original.json
  format: json
  label: Mireye Earth API
  slug: mireye-earth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-openapi-original.json
authorization_urls:
- https://api.mireye.com/authorize
description: ''
docs: https://docs.mireye.ai/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Mireye Scopes
name_suffix: OAuth Scopes
note: Scopes captured from the RFC 8414 authorization-server metadata and the auth docs; the OpenAPI declares no oauth2 securitySchemes so nothing was derivable from the spec.
overview: 'Mireye publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mireye API on a user''s behalf.


  Tokens are issued from https://api.mireye.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mireye
provider_slug: mireye
schemes:
- flows:
  - authorizationUrl: https://api.mireye.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://api.mireye.com/token
  name: mcpOAuth
  source: https://api.mireye.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Authorizes calls to Mireye's MCP tools (mireye_ask, mireye_fetch) via the hosted /mcp endpoint. Not valid for direct /v1/* HTTP API calls.
  flows:
  - authorizationCode
  scope: mcp:tools
slug: mireye-scopes
source_filename: mireye-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.mireye.com/.well-known/oauth-authorization-server\ndocs: https://docs.mireye.ai/authentication\nnote: >-\n  Scopes captured from the RFC 8414 authorization-server metadata and the auth docs; the\n  OpenAPI declares no oauth2 securitySchemes so nothing was derivable from the spec.\nschemes:\n- name: mcpOAuth\n  source: https://api.mireye.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.mireye.com/authorize\n    tokenUrl: https://api.mireye.com/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: mcp:tools\n  description: Authorizes calls to Mireye's MCP tools (mireye_ask, mireye_fetch) via the hosted /mcp endpoint. Not valid for direct /v1/* HTTP API calls.\n  flows: [authorizationCode]\n  sources: ['https://api.mireye.com/.well-known/oauth-authorization-server']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/scopes/mireye-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Geospatial
- Geographic Information System
- Location
- AI Agents
- Model Context Protocol
- Government Data
- Risk
- Insurance
- Data
token_urls:
- https://api.mireye.com/token
---
