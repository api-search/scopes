---
api_specs:
- filename: immokit-ai-bodenrichtwert-api-openapi.yml
  format: yaml
  label: immokit-ai Bodenrichtwert API
  slug: immokit-ai-bodenrichtwert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immokit-ai/openapi/immokit-ai-bodenrichtwert-api-openapi.yml
- filename: immokit-ai-bodenwert-api-openapi.yml
  format: yaml
  label: immokit-ai Bodenwert API
  slug: immokit-ai-bodenwert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immokit-ai/openapi/immokit-ai-bodenwert-api-openapi.yml
- filename: immokit-ai-me-api-openapi.yml
  format: yaml
  label: immokit-ai Me API
  slug: immokit-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immokit-ai/openapi/immokit-ai-me-api-openapi.yml
authorization_urls:
- https://bodenrichtwert.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: immokit-ai Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'immokit-ai uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://bodenrichtwert.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: immokit-ai
provider_slug: immokit-ai
schemes:
- flows:
  - authorizationUrl: https://bodenrichtwert.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://bodenrichtwert.ai/oauth/token
  name: OAuth2
  source: openapi/immokit-ai-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: immokit-ai-scopes
source_filename: immokit-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: none\nsource: openapi/immokit-ai-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/immokit-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://bodenrichtwert.ai/oauth/authorize\n    tokenUrl: https://bodenrichtwert.ai/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/immokit-ai/scopes/immokit-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
token_bound: false
token_urls:
- https://bodenrichtwert.ai/oauth/token
---
