---
api_specs:
- filename: bria-automotive-endpoints-api-openapi.yml
  format: yaml
  label: Bria Automotive Endpoints API
  slug: bria-automotive-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-automotive-endpoints-api-openapi.yml
- filename: bria-dataset-api-openapi.yml
  format: yaml
  label: Bria Dataset API
  slug: bria-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-dataset-api-openapi.yml
- filename: bria-editing-endpoints-api-openapi.yml
  format: yaml
  label: Bria Editing Endpoints API
  slug: bria-editing-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-editing-endpoints-api-openapi.yml
- filename: bria-endpoints-api-openapi.yml
  format: yaml
  label: Bria Endpoints API
  slug: bria-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-endpoints-api-openapi.yml
- filename: bria-image-attribution-api-openapi.yml
  format: yaml
  label: Bria Image Attribution API
  slug: bria-image-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-image-attribution-api-openapi.yml
- filename: bria-image-generation-api-openapi.yml
  format: yaml
  label: Bria Image Generation API
  slug: bria-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-image-generation-api-openapi.yml
- filename: bria-masking-endpoints-api-openapi.yml
  format: yaml
  label: Bria Masking Endpoints API
  slug: bria-masking-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-masking-endpoints-api-openapi.yml
- filename: bria-model-api-openapi.yml
  format: yaml
  label: Bria Model API
  slug: bria-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-model-api-openapi.yml
- filename: bria-product-endpoints-api-openapi.yml
  format: yaml
  label: Bria Product Endpoints API
  slug: bria-product-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-product-endpoints-api-openapi.yml
- filename: bria-project-api-openapi.yml
  format: yaml
  label: Bria Project API
  slug: bria-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-project-api-openapi.yml
- filename: bria-v2-endpoints-api-openapi.yml
  format: yaml
  label: Bria v2 endpoints API
  slug: bria-v2-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-v2-endpoints-api-openapi.yml
- filename: bria-video-attribution-api-openapi.yml
  format: yaml
  label: Bria Video Attribution API
  slug: bria-video-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-video-attribution-api-openapi.yml
- filename: bria-video-generation-api-openapi.yml
  format: yaml
  label: Bria Video Generation API
  slug: bria-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-video-generation-api-openapi.yml
authorization_urls:
- https://engine.prod.bria-api.com/v2/auth/authorize
- https://mcp.internal.production.bria-api.com/authorize
description: ''
docs: https://docs.bria.ai/mcp-authentication
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Bria Scopes
name_suffix: OAuth Scopes
note: No OpenAPI in this repo declares an oauth2 securityScheme, so nothing was derivable from the specs. These scopes come from Bria's own RFC 8414 authorization-server metadata, probed live on both the engine and MCP hosts. Bria publishes no scopes/permissions reference page; the three scopes below are the complete advertised set and are identity scopes only — Bria's API authorization is carried by the api_token key, not by OAuth scope.
overview: 'Bria publishes 3 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bria API on a user''s behalf.


  Tokens are issued from https://engine.prod.bria-api.com/v2/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bria
provider_slug: bria
schemes:
- flows:
  - authorizationUrl: https://engine.prod.bria-api.com/v2/auth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://engine.prod.bria-api.com/v2/auth/token
  - deviceAuthorizationUrl: https://engine.prod.bria-api.com/v2/auth/device/authorize
    flow: deviceCode
  name: OAuth2
  source: well-known/bria-engine-oauth-authorization-server.json
- flows:
  - authorizationUrl: https://mcp.internal.production.bria-api.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://mcp.internal.production.bria-api.com/token
  name: OAuth2-MCP
  source: well-known/bria-mcp-oauth-authorization-server.json
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect identity scope; requests an ID token for the authenticating user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticating user.
  flows:
  - authorizationCode
  scope: profile
- description: Email address claim for the authenticating user.
  flows:
  - authorizationCode
  scope: email
slug: bria-scopes
source_filename: bria-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: https://engine.prod.bria-api.com/.well-known/oauth-authorization-server\ndocs: https://docs.bria.ai/mcp-authentication\nnote: >-\n  No OpenAPI in this repo declares an oauth2 securityScheme, so nothing was derivable from the\n  specs. These scopes come from Bria's own RFC 8414 authorization-server metadata, probed live on\n  both the engine and MCP hosts. Bria publishes no scopes/permissions reference page; the three\n  scopes below are the complete advertised set and are identity scopes only — Bria's API\n  authorization is carried by the api_token key, not by OAuth scope.\nschemes:\n- name: OAuth2\n  source: well-known/bria-engine-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://engine.prod.bria-api.com/v2/auth/authorize\n    tokenUrl: https://engine.prod.bria-api.com/v2/auth/token\n    code_challenge_methods: [S256]\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://engine.prod.bria-api.com/v2/auth/device/authorize\n\
  - name: OAuth2-MCP\n  source: well-known/bria-mcp-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.internal.production.bria-api.com/authorize\n    tokenUrl: https://mcp.internal.production.bria-api.com/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: openid\n  description: OpenID Connect identity scope; requests an ID token for the authenticating user.\n  flows: [authorizationCode]\n  sources: [well-known/bria-engine-oauth-authorization-server.json, well-known/bria-mcp-oauth-authorization-server.json]\n- scope: profile\n  description: Basic profile claims for the authenticating user.\n  flows: [authorizationCode]\n  sources: [well-known/bria-engine-oauth-authorization-server.json, well-known/bria-mcp-oauth-authorization-server.json]\n- scope: email\n  description: Email address claim for the authenticating user.\n  flows: [authorizationCode]\n  sources: [well-known/bria-engine-oauth-authorization-server.json, well-known/bria-mcp-oauth-authorization-server.json]\n\
  gaps:\n- >-\n  No capability scopes are published. An agent cannot request read-only or per-product access;\n  a Bria token is all-or-nothing across every generation, editing and training operation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/scopes/bria-scopes.yml
summary_line: 3 scopes · authorizationCode/deviceCode
tags:
- Artificial Intelligence
- Generative AI
- Images
- Image Generation
- Image Editing
- Video
- Machine Learning
- Media
- Content
- Agents
- MCP
token_urls:
- https://engine.prod.bria-api.com/v2/auth/token
- https://mcp.internal.production.bria-api.com/token
---
