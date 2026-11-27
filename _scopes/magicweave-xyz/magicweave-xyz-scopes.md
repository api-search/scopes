---
api_specs:
- filename: magicweave-xyz-openapi-generated.yml
  format: yaml
  label: Magicweave API
  slug: magicweave-xyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicweave-xyz/openapi/_ae-authored/magicweave-xyz-openapi-generated.yml
authorization_urls:
- https://mcp.magicweave.xyz/mcp
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Magicweave Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Magicweave uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://mcp.magicweave.xyz/mcp.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Magicweave
provider_slug: magicweave-xyz
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://mcp.magicweave.xyz/mcp
  - authorizationUrl: https://mcp.magicweave.xyz/mcp
    flow: authorizationCode
    tokenUrl: https://mcp.magicweave.xyz/mcp
  name: OAuth2
  source: openapi/magicweave-xyz-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: magicweave-xyz-scopes
source_filename: magicweave-xyz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: none\nsource: openapi/magicweave-xyz-openapi-generated.yml\nschemes:\n- name: OAuth2\n  source: openapi/magicweave-xyz-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://mcp.magicweave.xyz/mcp\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.magicweave.xyz/mcp\n    tokenUrl: https://mcp.magicweave.xyz/mcp\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/magicweave-xyz/scopes/magicweave-xyz-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Gaming
- Backend
- Artificial Intelligence
- Platform
- Economy
token_bound: false
token_urls:
- https://mcp.magicweave.xyz/mcp
---
