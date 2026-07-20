---
api_specs:
- filename: cube-planning-openapi-original.yml
  format: yaml
  label: Cube API
  slug: cube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-planning/refs/heads/main/openapi/cube-planning-openapi-original.yml
authorization_urls:
- https://portal.cubesoftware.com/o/authorize/
description: ''
docs: https://api.cubesoftware.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cube Planning Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cube Planning publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cube Planning API on a user''s behalf.


  Tokens are issued from https://api.cubesoftware.com/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cube Planning
provider_slug: cube-planning
schemes:
- description: Standard Cube OAuth 2.0 flow (authorization code + PKCE). The OpenAPI security scheme declares no scopes; the scopes below are taken verbatim from Cube's RFC 8414 OAuth authorization-server metadata document.
  flows:
  - authorizationUrl: https://portal.cubesoftware.com/o/authorize/
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    introspectionUrl: https://api.cubesoftware.com/o/introspect/
    pkce: S256
    tokenUrl: https://api.cubesoftware.com/o/token/
  name: OAuth2
  source: openapi/cube-planning-openapi-original.yml
scope_count: 3
scope_names:
- read
- write
- introspection
scopes:
- description: Read access to Cube resources.
  flows:
  - authorizationCode
  scope: read
- description: Write access to Cube resources.
  flows:
  - authorizationCode
  scope: write
- description: Permission to introspect access tokens via the introspection endpoint.
  flows:
  - authorizationCode
  scope: introspection
slug: cube-planning-scopes
source_filename: cube-planning-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cube-planning-openapi-original.yml\ndocs: https://api.cubesoftware.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: openapi/cube-planning-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://portal.cubesoftware.com/o/authorize/\n    tokenUrl: https://api.cubesoftware.com/o/token/\n    introspectionUrl: https://api.cubesoftware.com/o/introspect/\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n  description: Standard Cube OAuth 2.0 flow (authorization code + PKCE). The OpenAPI\n    security scheme declares no scopes; the scopes below are taken verbatim from Cube's\n    RFC 8414 OAuth authorization-server metadata document.\n# Scopes are NOT declared per-operation in the OpenAPI; they are published in Cube's\n# /.well-known/oauth-authorization-server document (scopes_supported).\nscopes:\n- scope: read\n  description: Read access\
  \ to Cube resources.\n  flows: [authorizationCode]\n  sources: ['well-known/cube-planning-oauth-authorization-server.json']\n- scope: write\n  description: Write access to Cube resources.\n  flows: [authorizationCode]\n  sources: ['well-known/cube-planning-oauth-authorization-server.json']\n- scope: introspection\n  description: Permission to introspect access tokens via the introspection endpoint.\n  flows: [authorizationCode]\n  sources: ['well-known/cube-planning-oauth-authorization-server.json']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cube-planning/refs/heads/main/scopes/cube-planning-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Budgeting
- Forecasting
- Analytics
- Planning
token_urls:
- https://api.cubesoftware.com/o/token/
---
