---
api_specs:
- filename: coupondroid-it-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid Italia A2a API
  slug: coupondroid-it-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-a2a-api-openapi.yml
- filename: coupondroid-it-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid Italia Auth.md API
  slug: coupondroid-it-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-auth-md-api-openapi.yml
- filename: coupondroid-it-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid Italia Llms.txt API
  slug: coupondroid-it-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-llms-txt-api-openapi.yml
- filename: coupondroid-it-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid Italia MCP API
  slug: coupondroid-it-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-mcp-api-openapi.yml
- filename: coupondroid-it-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid Italia .well Known API
  slug: coupondroid-it-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-it/openapi/coupondroid-it-well-known-api-openapi.yml
authorization_urls:
- https://coupondroid.it/oauth/authorize
description: ''
docs: https://coupondroid.it/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coupondroid Italia Scopes
name_suffix: OAuth Scopes
note: Scopes read, write and delete per auth.md; what a token can do is the smaller of its scopes and the role of the person behind it.
overview: 'Coupondroid Italia publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coupondroid Italia API on a user''s behalf.


  Tokens are issued from https://coupondroid.it/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coupondroid Italia
provider_slug: coupondroid-it
schemes:
- description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  flows:
  - authorizationUrl: https://coupondroid.it/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://coupondroid.it/oauth/token
  name: oauth2
  source: openapi/coupondroid-it-openapi.yml
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
slug: coupondroid-it-scopes
source_filename: coupondroid-it-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.it/auth.md\nschemes:\n- name: oauth2\n  source: openapi/coupondroid-it-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.it/oauth/authorize\n    tokenUrl: https://coupondroid.it/oauth/token\n  description: Authorization code with PKCE (S256); dynamic client registration at\n    /oauth/register.\nscopes:\n- scope: delete\n  description: Delete\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-it-openapi.yml\n- scope: read\n  description: Read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-it-openapi.yml\n- scope: write\n  description: Create and edit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-it-openapi.yml\ndocs: https://coupondroid.it/auth.md\nnote: Scopes read, write and delete per auth.md; what a token can do is the smaller\n  of its scopes and the role of the person behind it.\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-it/scopes/coupondroid-it-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Coupons
- Discount Codes
- Deals
- E-Commerce
- Affiliate Marketing
- Italy
- MCP
token_bound: false
token_urls:
- https://coupondroid.it/oauth/token
---
