---
api_specs:
- filename: lawmadi-com-agent-discovery-api-openapi.yml
  format: yaml
  label: Lawmadi Agent discovery API
  slug: lawmadi-com-agent-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-agent-discovery-api-openapi.yml
- filename: lawmadi-com-ask-api-openapi.yml
  format: yaml
  label: Lawmadi Ask API
  slug: lawmadi-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-ask-api-openapi.yml
- filename: lawmadi-com-ask-stream-api-openapi.yml
  format: yaml
  label: Lawmadi Ask Stream API
  slug: lawmadi-com-ask-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-ask-stream-api-openapi.yml
- filename: lawmadi-com-pricing-api-openapi.yml
  format: yaml
  label: Lawmadi Pricing API
  slug: lawmadi-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-pricing-api-openapi.yml
authorization_urls:
- https://lawmadi.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Lawmadi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lawmadi publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lawmadi API on a user''s behalf.


  Tokens are issued from https://lawmadi.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lawmadi
provider_slug: lawmadi-com
schemes:
- description: 'Authorization code + PKCE (S256 only). Dynamic client registration is open (RFC 7591). Scope `mcp:read` cannot spend the user''s credits. Server metadata: https://lawmadi.com/.well-known/oauth-authorization-server (RFC 8414); protected resource metadata: https://lawmadi.com/mcp/.well-known/oauth-protected-resource (RFC 9728).'
  flows:
  - authorizationUrl: https://lawmadi.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://lawmadi.com/oauth/token
  name: oauth2
  source: openapi/lawmadi-com-openapi.json
scope_count: 2
scope_names:
- mcp
- mcp:read
scopes:
- description: Call any tool, including tools that spend credits.
  flows:
  - authorizationCode
  scope: mcp
- description: Call tools that never spend credits.
  flows:
  - authorizationCode
  scope: mcp:read
slug: lawmadi-com-scopes
source_filename: lawmadi-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/lawmadi-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/lawmadi-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lawmadi.com/oauth/authorize\n    tokenUrl: https://lawmadi.com/oauth/token\n  description: 'Authorization code + PKCE (S256 only). Dynamic client registration is open (RFC\n    7591). Scope `mcp:read` cannot spend the user''s credits. Server metadata: https://lawmadi.com/.well-known/oauth-authorization-server\n    (RFC 8414); protected resource metadata: https://lawmadi.com/mcp/.well-known/oauth-protected-resource\n    (RFC 9728).'\nscopes:\n- scope: mcp\n  description: Call any tool, including tools that spend credits.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lawmadi-com-openapi.json\n- scope: mcp:read\n  description: Call tools that never spend credits.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lawmadi-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lawmadi-com/scopes/lawmadi-com-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Legal Tech
- Artificial Intelligence
- Korean
- Law
token_bound: false
token_urls:
- https://lawmadi.com/oauth/token
---
