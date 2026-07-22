---
api_specs:
- filename: trybloom-api-openapi.json
  format: json
  label: Bloom API
  slug: bloom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/openapi/trybloom-api-openapi.json
authorization_urls:
- https://www.trybloom.ai/api/auth/oauth2/authorize
description: ''
docs: https://www.trybloom.ai/docs/api/authentication
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Trybloom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bloom publishes 2 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bloom API on a user''s behalf.


  Tokens are issued from https://www.trybloom.ai/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bloom
provider_slug: trybloom
schemes:
- flows:
  - authorizationUrl: https://www.trybloom.ai/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce: S256 required for public clients
    tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token
  - flow: refreshToken
    tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token
  introspection: https://www.trybloom.ai/api/auth/oauth2/introspect
  issuer: https://www.trybloom.ai/api/auth
  jwks: https://www.trybloom.ai/api/auth/jwks
  name: Bloom OAuth
  registration: https://www.trybloom.ai/api/auth/oauth2/register
  revocation: https://www.trybloom.ai/api/auth/oauth2/revoke
  userinfo: https://www.trybloom.ai/api/auth/oauth2/userinfo
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
slug: trybloom-scopes
source_filename: trybloom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://www.trybloom.ai/.well-known/oauth-authorization-server (RFC 8414\n  metadata, saved verbatim at well-known/trybloom-oauth-authorization-server.json)\n  and https://www.trybloom.ai/docs/api/authentication.md. The OpenAPI declares\n  apiKey/bearer schemes only, so the scope surface comes from the published\n  OAuth metadata rather than the spec.\ndocs: https://www.trybloom.ai/docs/api/authentication\nnotes: >-\n  Bloom OAuth is identity-scoped rather than permission-scoped: access tokens\n  resolve to the same user identity as an API key, with the same access to\n  brands, images, credits, plan gates, and workspaces. Public clients use\n  Authorization Code + PKCE (S256) with dynamic client registration (RFC 7591)\n  and no client_secret; wildcard redirect URIs are not supported.\nschemes:\n  - name: Bloom OAuth\n    issuer: https://www.trybloom.ai/api/auth\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://www.trybloom.ai/api/auth/oauth2/authorize\n        tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token\n        pkce: S256 required for public clients\n      - flow: clientCredentials\n        tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token\n      - flow: refreshToken\n        tokenUrl: https://www.trybloom.ai/api/auth/oauth2/token\n    registration: https://www.trybloom.ai/api/auth/oauth2/register\n    jwks: https://www.trybloom.ai/api/auth/jwks\n    introspection: https://www.trybloom.ai/api/auth/oauth2/introspect\n    revocation: https://www.trybloom.ai/api/auth/oauth2/revoke\n    userinfo: https://www.trybloom.ai/api/auth/oauth2/userinfo\nscopes:\n  - scope: openid\n    description: OpenID Connect identity scope (advertised in scopes_supported).\n    flows: [authorizationCode]\n    sources: [well-known/trybloom-oauth-authorization-server.json]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived access (advertised in scopes_supported).\n\
  \    flows: [authorizationCode]\n    sources: [well-known/trybloom-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trybloom/refs/heads/main/scopes/trybloom-scopes.yml
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
token_urls:
- https://www.trybloom.ai/api/auth/oauth2/token
---
