---
api_specs:
- filename: kviria-com-account-api-openapi.yml
  format: yaml
  label: Kviria Account API
  slug: kviria-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kviria-com/openapi/kviria-com-account-api-openapi.yml
- filename: kviria-com-agent-api-openapi.yml
  format: yaml
  label: Kviria Agent API
  slug: kviria-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kviria-com/openapi/kviria-com-agent-api-openapi.yml
- filename: kviria-com-healthz-api-openapi.yml
  format: yaml
  label: Kviria Healthz API
  slug: kviria-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kviria-com/openapi/kviria-com-healthz-api-openapi.yml
authorization_urls:
- https://api.kviria.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Kviria Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Kviria uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.kviria.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kviria
provider_slug: kviria-com
schemes:
- description: OAuth 2.1 with PKCE (MCP clients); the token is bound to one resource.
  flows:
  - authorizationUrl: https://api.kviria.com/authorize
    flow: authorizationCode
    tokenUrl: https://api.kviria.com/oauth/token
  name: oauth
  source: openapi/kviria-com-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: kviria-com-scopes
source_filename: kviria-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: none\nsource: openapi/kviria-com-openapi.json\nschemes:\n- name: oauth\n  source: openapi/kviria-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kviria.com/authorize\n    tokenUrl: https://api.kviria.com/oauth/token\n  description: OAuth 2.1 with PKCE (MCP clients); the token is bound to one resource.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/kviria-com/scopes/kviria-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- location understanding
- AI Agents
- Privacy
token_bound: false
token_urls:
- https://api.kviria.com/oauth/token
---
