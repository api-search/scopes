---
api_specs:
- filename: doingwork-work-status-api-openapi.yml
  format: yaml
  label: doingwork-work Status API
  slug: doingwork-work-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doingwork-work/openapi/doingwork-work-status-api-openapi.yml
authorization_urls:
- https://app.doingwork.work/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Doingwork Work Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'doingwork-work publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the doingwork-work API on a user''s behalf.


  Tokens are issued from https://app.doingwork.work/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: doingwork-work
provider_slug: doingwork-work
schemes:
- description: 'Authorization code flow with PKCE (S256). Dynamic client registration at /oauth/register. Metadata: https://app.doingwork.work/.well-known/oauth-authorization-server'
  flows:
  - authorizationUrl: https://app.doingwork.work/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.doingwork.work/oauth/token
  name: doingWorkOAuth
  source: openapi/doingwork-work-openapi.json
scope_count: 4
scope_names:
- quotes
- quotes:read
- shop
- shop:read
scopes:
- description: 'Homeowner connector (/mcp/home): full use of the quote tools for the signed-in homeowner'
  flows:
  - authorizationCode
  scope: quotes
- description: 'Homeowner connector (/mcp/home): read only'
  flows:
  - authorizationCode
  scope: quotes:read
- description: 'Shop connector (/mcp/shop): full use of the shop tools for the signed-in shop'
  flows:
  - authorizationCode
  scope: shop
- description: 'Shop connector (/mcp/shop): read only'
  flows:
  - authorizationCode
  scope: shop:read
slug: doingwork-work-scopes
source_filename: doingwork-work-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/doingwork-work-openapi.json\nschemes:\n- name: doingWorkOAuth\n  source: openapi/doingwork-work-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.doingwork.work/oauth/authorize\n    tokenUrl: https://app.doingwork.work/oauth/token\n  description: 'Authorization code flow with PKCE (S256). Dynamic client registration at /oauth/register.\n    Metadata: https://app.doingwork.work/.well-known/oauth-authorization-server'\nscopes:\n- scope: quotes\n  description: 'Homeowner connector (/mcp/home): full use of the quote tools for the signed-in\n    homeowner'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/doingwork-work-openapi.json\n- scope: quotes:read\n  description: 'Homeowner connector (/mcp/home): read only'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/doingwork-work-openapi.json\n- scope: shop\n  description: 'Shop connector (/mcp/shop): full use of the shop\
  \ tools for the signed-in shop'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/doingwork-work-openapi.json\n- scope: shop:read\n  description: 'Shop connector (/mcp/shop): read only'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/doingwork-work-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/doingwork-work/scopes/doingwork-work-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Field Service Management
- Invoicing
- Mobile
token_bound: false
token_urls:
- https://app.doingwork.work/oauth/token
---
