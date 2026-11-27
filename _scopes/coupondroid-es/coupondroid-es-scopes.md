---
api_specs:
- filename: coupondroid-es-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid España A2a API
  slug: coupondroid-es-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-a2a-api-openapi.yml
- filename: coupondroid-es-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid España Auth.md API
  slug: coupondroid-es-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-auth-md-api-openapi.yml
- filename: coupondroid-es-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid España Llms.txt API
  slug: coupondroid-es-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-llms-txt-api-openapi.yml
- filename: coupondroid-es-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid España MCP API
  slug: coupondroid-es-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-mcp-api-openapi.yml
- filename: coupondroid-es-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid España .well Known API
  slug: coupondroid-es-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-es/openapi/coupondroid-es-well-known-api-openapi.yml
authorization_urls:
- https://coupondroid.es/oauth/authorize
description: ''
docs: https://coupondroid.es/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coupondroid España Scopes
name_suffix: OAuth Scopes
note: 'auth.md: ''What a token can do is the smaller of its scopes and the role of the person behind it.'''
overview: 'Coupondroid España publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coupondroid España API on a user''s behalf.


  Tokens are issued from https://coupondroid.es/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coupondroid España
provider_slug: coupondroid-es
schemes:
- description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  flows:
  - authorizationUrl: https://coupondroid.es/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://coupondroid.es/oauth/token
  name: oauth2
  source: openapi/coupondroid-es-openapi.yml
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
slug: coupondroid-es-scopes
source_filename: coupondroid-es-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.es/auth.md\nschemes:\n- name: oauth2\n  source: openapi/coupondroid-es-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.es/oauth/authorize\n    tokenUrl: https://coupondroid.es/oauth/token\n  description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.\nscopes:\n- scope: delete\n  description: Delete\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-es-openapi.yml\n- scope: read\n  description: Read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-es-openapi.yml\n- scope: write\n  description: Create and edit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-es-openapi.yml\ndocs: https://coupondroid.es/auth.md\nnote: 'auth.md: ''What a token can do is the smaller of its scopes and the role of the person behind it.'''\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-es/scopes/coupondroid-es-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Coupons
- Deals
- Discounts
- E-Commerce
- Shopping
- Spain
- MCP
token_bound: false
token_urls:
- https://coupondroid.es/oauth/token
---
