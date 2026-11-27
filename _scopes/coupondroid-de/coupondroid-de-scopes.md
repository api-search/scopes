---
api_specs:
- filename: coupondroid-de-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland A2a API
  slug: coupondroid-de-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-a2a-api-openapi.yml
- filename: coupondroid-de-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland Auth.md API
  slug: coupondroid-de-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-auth-md-api-openapi.yml
- filename: coupondroid-de-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland Llms.txt API
  slug: coupondroid-de-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-llms-txt-api-openapi.yml
- filename: coupondroid-de-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland MCP API
  slug: coupondroid-de-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-mcp-api-openapi.yml
- filename: coupondroid-de-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid Deutschland .well Known API
  slug: coupondroid-de-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-de/openapi/coupondroid-de-well-known-api-openapi.yml
authorization_urls:
- https://coupondroid.de/oauth/authorize
description: ''
docs: https://coupondroid.de/oauth/about
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coupondroid Deutschland Scopes
name_suffix: OAuth Scopes
note: Scopes apply only to the team management MCP server (https://coupondroid.de/mcp). What a token can do is the smaller of its scopes and the role of the person behind it (auth.md).
overview: 'Coupondroid Deutschland publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coupondroid Deutschland API on a user''s behalf.


  Tokens are issued from https://coupondroid.de/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coupondroid Deutschland
provider_slug: coupondroid-de
schemes:
- description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  flows:
  - authorizationUrl: https://coupondroid.de/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://coupondroid.de/oauth/token
  name: oauth2
  source: openapi/coupondroid-de-openapi.yml
scope_count: 3
scope_names:
- read
- write
- delete
scopes:
- description: 'Read only: view sites, shops, coupons, articles and all other data.'
  flows:
  - authorizationCode
  scope: read
- description: 'Read and write: also create and edit, always with your own permissions and a record of every change.'
  flows:
  - authorizationCode
  scope: write
- description: 'Everything, including delete: also delete. Every deletion asks for a separate confirmation.'
  flows:
  - authorizationCode
  scope: delete
slug: coupondroid-de-scopes
source_filename: coupondroid-de-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.de/oauth/about\ndocs: https://coupondroid.de/oauth/about\nschemes:\n- name: oauth2\n  source: openapi/coupondroid-de-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.de/oauth/authorize\n    tokenUrl: https://coupondroid.de/oauth/token\n  description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.\nnote: Scopes apply only to the team management MCP server (https://coupondroid.de/mcp). What a token can do is the smaller of its scopes and the role of the person behind it (auth.md).\nscopes:\n- scope: read\n  description: 'Read only: view sites, shops, coupons, articles and all other data.'\n  flows: [authorizationCode]\n  sources: [openapi/coupondroid-de-openapi.yml, https://coupondroid.de/oauth/about]\n- scope: write\n  description: 'Read and write: also create and edit, always with your own permissions and a record of every\
  \ change.'\n  flows: [authorizationCode]\n  sources: [openapi/coupondroid-de-openapi.yml, https://coupondroid.de/oauth/about]\n- scope: delete\n  description: 'Everything, including delete: also delete. Every deletion asks for a separate confirmation.'\n  flows: [authorizationCode]\n  sources: [openapi/coupondroid-de-openapi.yml, https://coupondroid.de/oauth/about]\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-de/scopes/coupondroid-de-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Coupons
- Deals
- Discounts
- E-Commerce
- Germany
- Shopping
- Vouchers
token_bound: false
token_urls:
- https://coupondroid.de/oauth/token
---
