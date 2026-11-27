---
api_specs:
- filename: coupondroid-com-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid A2a API
  slug: coupondroid-com-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-a2a-api-openapi.yml
- filename: coupondroid-com-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid Auth.md API
  slug: coupondroid-com-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-auth-md-api-openapi.yml
- filename: coupondroid-com-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid Llms.txt API
  slug: coupondroid-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-llms-txt-api-openapi.yml
- filename: coupondroid-com-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid MCP API
  slug: coupondroid-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-mcp-api-openapi.yml
- filename: coupondroid-com-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid .well Known API
  slug: coupondroid-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-com/openapi/coupondroid-com-well-known-api-openapi.yml
authorization_urls:
- https://coupondroid.com/oauth/authorize
description: ''
docs: https://coupondroid.com/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coupondroid Scopes
name_suffix: OAuth Scopes
note: 'auth.md: the scopes are read, write and delete; what a token can do is the smaller of its scopes and the role of the person behind it. Scopes apply only to the management MCP server https://coupondroid.com/mcp.'
overview: 'Coupondroid publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coupondroid API on a user''s behalf.


  Tokens are issued from https://coupondroid.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coupondroid
provider_slug: coupondroid-com
schemes:
- description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  flows:
  - authorizationUrl: https://coupondroid.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://coupondroid.com/oauth/token
  name: oauth2
  source: openapi/coupondroid-com-openapi.yml
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
slug: coupondroid-com-scopes
source_filename: coupondroid-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.com/auth.md\nschemes:\n- name: oauth2\n  source: openapi/coupondroid-com-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.com/oauth/authorize\n    tokenUrl: https://coupondroid.com/oauth/token\n  description: Authorization code with PKCE (S256); dynamic client registration at\n    /oauth/register.\nscopes:\n- scope: delete\n  description: Delete\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-com-openapi.yml\n  - https://coupondroid.com/auth.md\n- scope: read\n  description: Read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-com-openapi.yml\n  - https://coupondroid.com/auth.md\n- scope: write\n  description: Create and edit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-com-openapi.yml\n  - https://coupondroid.com/auth.md\ndocs: https://coupondroid.com/auth.md\nnote: 'auth.md: the scopes are\
  \ read, write and delete; what a token can do is the\n  smaller of its scopes and the role of the person behind it. Scopes apply only to\n  the management MCP server https://coupondroid.com/mcp.'\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-com/scopes/coupondroid-com-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Coupons
- Deals
- E-Commerce
- Shopping
- Affiliate Marketing
- MCP
- AI Agents
token_bound: false
token_urls:
- https://coupondroid.com/oauth/token
---
