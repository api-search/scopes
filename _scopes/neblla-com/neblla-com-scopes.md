---
api_specs:
- filename: neblla-com-connect-api-openapi.yml
  format: yaml
  label: Neblla Connect API
  slug: neblla-com-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-connect-api-openapi.yml
- filename: neblla-com-gallery-api-openapi.yml
  format: yaml
  label: Neblla Gallery API
  slug: neblla-com-gallery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-gallery-api-openapi.yml
- filename: neblla-com-llms-api-openapi.yml
  format: yaml
  label: Neblla Llms API
  slug: neblla-com-llms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-llms-api-openapi.yml
- filename: neblla-com-llms-full-txt-api-openapi.yml
  format: yaml
  label: Neblla Llms Full.txt API
  slug: neblla-com-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-llms-full-txt-api-openapi.yml
- filename: neblla-com-llms-txt-api-openapi.yml
  format: yaml
  label: Neblla Llms.txt API
  slug: neblla-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-llms-txt-api-openapi.yml
- filename: neblla-com-mcp-api-openapi.yml
  format: yaml
  label: Neblla MCP API
  slug: neblla-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-mcp-api-openapi.yml
- filename: neblla-com-stripe-api-openapi.yml
  format: yaml
  label: Neblla Stripe API
  slug: neblla-com-stripe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-stripe-api-openapi.yml
authorization_urls:
- https://developers.neblla.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Neblla Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Neblla uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://developers.neblla.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Neblla
provider_slug: neblla-com
schemes:
- flows:
  - authorizationUrl: https://developers.neblla.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://developers.neblla.com/oauth/token
  name: oauth2
  source: openapi/neblla-com.json
scope_count: 0
scope_names: []
scopes: []
slug: neblla-com-scopes
source_filename: neblla-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: none\nsource: openapi/neblla-com.json\nschemes:\n- name: oauth2\n  source: openapi/neblla-com.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developers.neblla.com/oauth/authorize\n    tokenUrl: https://developers.neblla.com/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/neblla-com/scopes/neblla-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Backend
- BaaS
- Gaming
- Artificial Intelligence
- Real-Time
token_bound: false
token_urls:
- https://developers.neblla.com/oauth/token
---
