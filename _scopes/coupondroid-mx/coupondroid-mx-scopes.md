---
api_specs:
- filename: coupondroid-mx-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid México A2a API
  slug: coupondroid-mx-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-a2a-api-openapi.yml
- filename: coupondroid-mx-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid México Auth.md API
  slug: coupondroid-mx-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-auth-md-api-openapi.yml
- filename: coupondroid-mx-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid México Llms.txt API
  slug: coupondroid-mx-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-llms-txt-api-openapi.yml
- filename: coupondroid-mx-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid México MCP API
  slug: coupondroid-mx-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-mcp-api-openapi.yml
- filename: coupondroid-mx-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid México .well Known API
  slug: coupondroid-mx-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-mx/openapi/coupondroid-mx-well-known-api-openapi.yml
authorization_urls:
- https://coupondroid.mx/oauth/authorize
description: ''
docs: https://coupondroid.mx/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coupondroid México Scopes
name_suffix: OAuth Scopes
note: 'auth.md: the scopes are read, write and delete; what a token can do is the smaller of its scopes and the role of the person behind it. Applies only to the team-only management MCP server at /mcp.'
overview: 'Coupondroid México publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coupondroid México API on a user''s behalf.


  Tokens are issued from https://coupondroid.mx/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coupondroid México
provider_slug: coupondroid-mx
schemes:
- description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  flows:
  - authorizationUrl: https://coupondroid.mx/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://coupondroid.mx/oauth/token
  name: oauth2
  source: openapi/coupondroid-mx-openapi.yml
scope_count: 3
scope_names:
- delete
- read
- write
scopes:
- description: Delete
  flows:
  - authorizationCode
  scope: delete
- description: Read
  flows:
  - authorizationCode
  scope: read
- description: Create and edit
  flows:
  - authorizationCode
  scope: write
slug: coupondroid-mx-scopes
source_filename: coupondroid-mx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.mx/auth.md\nschemes:\n- name: oauth2\n  source: openapi/coupondroid-mx-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.mx/oauth/authorize\n    tokenUrl: https://coupondroid.mx/oauth/token\n  description: Authorization code with PKCE (S256); dynamic client registration at\n    /oauth/register.\nscopes:\n- scope: delete\n  description: Delete\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-mx-openapi.yml\n  - https://coupondroid.mx/auth.md\n- scope: read\n  description: Read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-mx-openapi.yml\n  - https://coupondroid.mx/auth.md\n- scope: write\n  description: Create and edit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-mx-openapi.yml\n  - https://coupondroid.mx/auth.md\ndocs: https://coupondroid.mx/auth.md\nnote: 'auth.md: the scopes are read, write\
  \ and delete; what a token can do is the\n  smaller of its scopes and the role of the person behind it. Applies only to the\n  team-only management MCP server at /mcp.'\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-mx/scopes/coupondroid-mx-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Coupons
- Discounts
- Deals
- E-Commerce
- Mexico
- Affiliate Marketing
- MCP
token_bound: false
token_urls:
- https://coupondroid.mx/oauth/token
---
