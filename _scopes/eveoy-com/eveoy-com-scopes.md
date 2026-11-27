---
api_specs:
- filename: eveoy-com-mcp-api-openapi.yml
  format: yaml
  label: Eveoy MCP API
  slug: eveoy-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eveoy-com/openapi/eveoy-com-mcp-api-openapi.yml
- filename: eveoy-com-order-api-openapi.yml
  format: yaml
  label: Eveoy Order API
  slug: eveoy-com-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eveoy-com/openapi/eveoy-com-order-api-openapi.yml
authorization_urls:
- https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Eveoy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Eveoy publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Eveoy API on a user''s behalf.


  Tokens are issued from https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Eveoy
provider_slug: eveoy-com
schemes:
- flows:
  - authorizationUrl: https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/token
  name: oauth2
  source: openapi/eveoy-com-openapi.json
scope_count: 3
scope_names:
- email
- openid
- profile
scopes:
- description: Read account email
  flows:
  - authorizationCode
  scope: email
- description: OIDC sign-in
  flows:
  - authorizationCode
  scope: openid
- description: Read account profile
  flows:
  - authorizationCode
  scope: profile
slug: eveoy-com-scopes
source_filename: eveoy-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/eveoy-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/eveoy-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/token\nscopes:\n- scope: email\n  description: Read account email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/eveoy-com-openapi.json\n- scope: openid\n  description: OIDC sign-in\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/eveoy-com-openapi.json\n- scope: profile\n  description: Read account profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/eveoy-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/eveoy-com/scopes/eveoy-com-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- CustomerPhotos
- InStoreSampling
- BuyAndTry
- Marketing
- Retail
token_bound: false
token_urls:
- https://ascyiwwrflizprjypxxr.supabase.co/auth/v1/oauth/token
---
