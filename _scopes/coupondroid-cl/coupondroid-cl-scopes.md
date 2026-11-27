---
api_specs:
- filename: coupondroid-cl-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid Chile A2a API
  slug: coupondroid-cl-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-a2a-api-openapi.yml
- filename: coupondroid-cl-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid Chile Auth.md API
  slug: coupondroid-cl-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-auth-md-api-openapi.yml
- filename: coupondroid-cl-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid Chile Llms.txt API
  slug: coupondroid-cl-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-llms-txt-api-openapi.yml
- filename: coupondroid-cl-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid Chile MCP API
  slug: coupondroid-cl-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-mcp-api-openapi.yml
- filename: coupondroid-cl-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid Chile .well Known API
  slug: coupondroid-cl-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-cl/openapi/coupondroid-cl-well-known-api-openapi.yml
authorization_urls:
- https://coupondroid.cl/oauth/authorize
description: ''
docs: https://coupondroid.cl/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coupondroid Chile Scopes
name_suffix: OAuth Scopes
note: 'auth.md: "the scopes are `read`, `write` and `delete`"; what a token can do is the smaller of its scopes and the role of the person behind it. Only the management MCP server (/mcp) uses them.'
overview: 'Coupondroid Chile publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coupondroid Chile API on a user''s behalf.


  Tokens are issued from https://coupondroid.cl/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coupondroid Chile
provider_slug: coupondroid-cl
schemes:
- description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  flows:
  - authorizationUrl: https://coupondroid.cl/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://coupondroid.cl/oauth/token
  name: oauth2
  source: openapi/coupondroid-cl-openapi.yml
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
slug: coupondroid-cl-scopes
source_filename: coupondroid-cl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.cl/auth.md\nschemes:\n- name: oauth2\n  source: openapi/coupondroid-cl-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.cl/oauth/authorize\n    tokenUrl: https://coupondroid.cl/oauth/token\n  description: Authorization code with PKCE (S256); dynamic client registration at\n    /oauth/register.\nscopes:\n- scope: delete\n  description: Delete\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-cl-openapi.yml\n- scope: read\n  description: Read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-cl-openapi.yml\n- scope: write\n  description: Create and edit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-cl-openapi.yml\ndocs: https://coupondroid.cl/auth.md\nnote: 'auth.md: \"the scopes are `read`, `write` and `delete`\"; what a token can do\n  is the smaller of its scopes and the role of the person behind\
  \ it. Only the management\n  MCP server (/mcp) uses them.'\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-cl/scopes/coupondroid-cl-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Coupons
- Deals
- Discounts
- E-Commerce
- Affiliate Marketing
- Retail
- Chile
- MCP
token_bound: false
token_urls:
- https://coupondroid.cl/oauth/token
---
