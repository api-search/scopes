---
api_specs:
- filename: rainbrand-account-api-openapi.yml
  format: yaml
  label: Rainbrand Account API
  slug: rainbrand-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-account-api-openapi.yml
- filename: rainbrand-brands-api-openapi.yml
  format: yaml
  label: Rainbrand Brands API
  slug: rainbrand-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-brands-api-openapi.yml
- filename: rainbrand-images-api-openapi.yml
  format: yaml
  label: Rainbrand Images API
  slug: rainbrand-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-images-api-openapi.yml
- filename: rainbrand-audio-api-openapi.yml
  format: yaml
  label: Rainbrand Audio API
  slug: rainbrand-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-audio-api-openapi.yml
- filename: rainbrand-briefs-api-openapi.yml
  format: yaml
  label: Rainbrand Briefs API
  slug: rainbrand-briefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-briefs-api-openapi.yml
- filename: rainbrand-feedback-api-openapi.yml
  format: yaml
  label: Rainbrand Feedback API
  slug: rainbrand-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-feedback-api-openapi.yml
- filename: rainbrand-generations-api-openapi.yml
  format: yaml
  label: Rainbrand Generations API
  slug: rainbrand-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-generations-api-openapi.yml
- filename: rainbrand-library-api-openapi.yml
  format: yaml
  label: Rainbrand Library API
  slug: rainbrand-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-library-api-openapi.yml
- filename: rainbrand-models-api-openapi.yml
  format: yaml
  label: Rainbrand Models API
  slug: rainbrand-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-models-api-openapi.yml
- filename: rainbrand-reviews-api-openapi.yml
  format: yaml
  label: Rainbrand Reviews API
  slug: rainbrand-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-reviews-api-openapi.yml
- filename: rainbrand-uploads-api-openapi.yml
  format: yaml
  label: Rainbrand Uploads API
  slug: rainbrand-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-uploads-api-openapi.yml
- filename: rainbrand-videos-api-openapi.yml
  format: yaml
  label: Rainbrand Videos API
  slug: rainbrand-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-videos-api-openapi.yml
authorization_urls:
- https://www.rainbrand.com/api/auth/oauth2/authorize
description: ''
docs: https://docs.rainbrand.com/authentication
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Rainbrand Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rainbrand publishes 2 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rainbrand API on a user''s behalf.


  Tokens are issued from https://www.rainbrand.com/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rainbrand
provider_slug: rainbrand
schemes:
- flows:
  - authorizationUrl: https://www.rainbrand.com/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce: S256 required for public clients
    tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token
  - flow: refreshToken
    tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token
  introspection: https://www.rainbrand.com/api/auth/oauth2/introspect
  issuer: https://www.rainbrand.com/api/auth
  jwks: https://www.rainbrand.com/api/auth/jwks
  name: Rainbrand OAuth
  registration: https://www.rainbrand.com/api/auth/oauth2/register
  revocation: https://www.rainbrand.com/api/auth/oauth2/revoke
  userinfo: https://www.rainbrand.com/api/auth/oauth2/userinfo
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: OpenID Connect identity scope (advertised in scopes_supported).
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token for long-lived access (advertised in scopes_supported).
  flows:
  - authorizationCode
  scope: offline_access
slug: rainbrand-scopes
source_filename: rainbrand-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://www.rainbrand.com/.well-known/oauth-authorization-server (RFC 8414\n  metadata, saved verbatim at well-known/rainbrand-oauth-authorization-server.json)\n  and https://docs.rainbrand.com/authentication.md. The OpenAPI declares\n  apiKey/bearer schemes only, so the scope surface comes from the published\n  OAuth metadata rather than the spec.\ndocs: https://docs.rainbrand.com/authentication\nnotes: >-\n  Rainbrand OAuth is identity-scoped rather than permission-scoped: access tokens\n  resolve to the same user identity as an API key, with the same access to\n  brands, images, credits, plan gates, and workspaces. Public clients use\n  Authorization Code + PKCE (S256) with dynamic client registration (RFC 7591)\n  and no client_secret; wildcard redirect URIs are not supported.\nschemes:\n  - name: Rainbrand OAuth\n    issuer: https://www.rainbrand.com/api/auth\n    flows:\n      - flow: authorizationCode\n       \
  \ authorizationUrl: https://www.rainbrand.com/api/auth/oauth2/authorize\n        tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token\n        pkce: S256 required for public clients\n      - flow: clientCredentials\n        tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token\n      - flow: refreshToken\n        tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token\n    registration: https://www.rainbrand.com/api/auth/oauth2/register\n    jwks: https://www.rainbrand.com/api/auth/jwks\n    introspection: https://www.rainbrand.com/api/auth/oauth2/introspect\n    revocation: https://www.rainbrand.com/api/auth/oauth2/revoke\n    userinfo: https://www.rainbrand.com/api/auth/oauth2/userinfo\nscopes:\n  - scope: openid\n    description: OpenID Connect identity scope (advertised in scopes_supported).\n    flows: [authorizationCode]\n    sources: [well-known/rainbrand-oauth-authorization-server.json]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived\
  \ access (advertised in scopes_supported).\n    flows: [authorizationCode]\n    sources: [well-known/rainbrand-oauth-authorization-server.json]\n"
source_yaml_url: https://artifacts.apis.io/rainbrand/scopes/rainbrand-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Company
- Brand Management
- Image Generation
- Artificial Intelligence
- Agents
- MCP
- Marketing
- Creative
token_bound: false
token_urls:
- https://www.rainbrand.com/api/auth/oauth2/token
---
