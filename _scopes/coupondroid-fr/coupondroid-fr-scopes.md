---
api_specs:
- filename: coupondroid-fr-a2a-api-openapi.yml
  format: yaml
  label: Coupondroid France A2a API
  slug: coupondroid-fr-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-a2a-api-openapi.yml
- filename: coupondroid-fr-auth-md-api-openapi.yml
  format: yaml
  label: Coupondroid France Auth.md API
  slug: coupondroid-fr-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-auth-md-api-openapi.yml
- filename: coupondroid-fr-llms-txt-api-openapi.yml
  format: yaml
  label: Coupondroid France Llms.txt API
  slug: coupondroid-fr-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-llms-txt-api-openapi.yml
- filename: coupondroid-fr-mcp-api-openapi.yml
  format: yaml
  label: Coupondroid France MCP API
  slug: coupondroid-fr-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-mcp-api-openapi.yml
- filename: coupondroid-fr-well-known-api-openapi.yml
  format: yaml
  label: Coupondroid France .well Known API
  slug: coupondroid-fr-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coupondroid-fr/openapi/coupondroid-fr-well-known-api-openapi.yml
authorization_urls:
- https://coupondroid.fr/oauth/authorize
description: ''
docs: https://coupondroid.fr/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coupondroid France Scopes
name_suffix: OAuth Scopes
note: Scopes confirmed by scopes_supported in /.well-known/oauth-protected-resource and /.well-known/oauth-authorization-server (both HTTP 200 on 2026-11-04). Effective permission is the smaller of the token scopes and the role of the team member behind it (auth.md).
overview: 'Coupondroid France publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coupondroid France API on a user''s behalf.


  Tokens are issued from https://coupondroid.fr/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coupondroid France
provider_slug: coupondroid-fr
schemes:
- description: Authorization code with PKCE (S256); dynamic client registration at /oauth/register.
  flows:
  - authorizationUrl: https://coupondroid.fr/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://coupondroid.fr/oauth/token
  name: oauth2
  source: openapi/coupondroid-fr-openapi.yml
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
slug: coupondroid-fr-scopes
source_filename: coupondroid-fr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coupondroid.fr/auth.md\nschemes:\n- name: oauth2\n  source: openapi/coupondroid-fr-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coupondroid.fr/oauth/authorize\n    tokenUrl: https://coupondroid.fr/oauth/token\n  description: Authorization code with PKCE (S256); dynamic client registration at\n    /oauth/register.\nscopes:\n- scope: delete\n  description: Delete\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-fr-openapi.yml\n- scope: read\n  description: Read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-fr-openapi.yml\n- scope: write\n  description: Create and edit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/coupondroid-fr-openapi.yml\ndocs: https://coupondroid.fr/auth.md\nderived_from: openapi/coupondroid-fr-openapi.yml\nnote: Scopes confirmed by scopes_supported in /.well-known/oauth-protected-resource\n  and /.well-known/oauth-authorization-server\
  \ (both HTTP 200 on 2026-11-04). Effective\n  permission is the smaller of the token scopes and the role of the team member behind\n  it (auth.md).\n"
source_yaml_url: https://artifacts.apis.io/coupondroid-fr/scopes/coupondroid-fr-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Coupons
- Promo Codes
- Deals
- E-Commerce
- Affiliate Marketing
- France
- MCP
token_bound: false
token_urls:
- https://coupondroid.fr/oauth/token
---
