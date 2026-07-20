---
api_specs:
- filename: cubesoftware-openapi-original.yml
  format: yaml
  label: Cube API
  slug: cube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubesoftware/refs/heads/main/openapi/cubesoftware-openapi-original.yml
authorization_urls:
- https://portal.cubesoftware.com/o/authorize/
description: ''
docs: https://api.cubesoftware.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cubesoftware Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cube publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cube API on a user''s behalf.


  Tokens are issued from https://api.cubesoftware.com/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cube
provider_slug: cubesoftware
schemes:
- description: Standard Cube OAuth 2.0 flow (authorization code + PKCE S256, refresh_token supported)
  flows:
  - authorizationUrl: https://portal.cubesoftware.com/o/authorize/
    flow: authorizationCode
    tokenUrl: https://api.cubesoftware.com/o/token/
  name: OAuth2
  source: openapi/cubesoftware-openapi-original.yml
scope_count: 3
scope_names:
- read
- write
- introspection
scopes:
- description: Read access to Cube data and resources.
  flows:
  - authorizationCode
  scope: read
- description: Write/modify access to Cube data and resources.
  flows:
  - authorizationCode
  scope: write
- description: Permission to call the OAuth token introspection endpoint.
  flows:
  - authorizationCode
  scope: introspection
slug: cubesoftware-scopes
source_filename: cubesoftware-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cubesoftware-openapi-original.yml\ndocs: https://api.cubesoftware.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: openapi/cubesoftware-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://portal.cubesoftware.com/o/authorize/\n    tokenUrl: https://api.cubesoftware.com/o/token/\n  description: Standard Cube OAuth 2.0 flow (authorization code + PKCE S256, refresh_token supported)\nscopes:\n- scope: read\n  description: Read access to Cube data and resources.\n  flows: [authorizationCode]\n  sources: [well-known/cubesoftware-oauth-authorization-server.json]\n- scope: write\n  description: Write/modify access to Cube data and resources.\n  flows: [authorizationCode]\n  sources: [well-known/cubesoftware-oauth-authorization-server.json]\n- scope: introspection\n  description: Permission to call the OAuth token introspection endpoint.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/cubesoftware-oauth-authorization-server.json]\nnotes: >-\n  The published OpenAPI declares an OAuth2 authorizationCode scheme with an empty\n  scopes map; the coarse scopes (read, write, introspection) are advertised by the\n  provider's /.well-known/oauth-authorization-server document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubesoftware/refs/heads/main/scopes/cubesoftware-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Budgeting
- Forecasting
- Analytics
- Spreadsheets
- SaaS
token_urls:
- https://api.cubesoftware.com/o/token/
---
