---
api_specs:
- filename: effect-photonics-wp-v2-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Wp/v2 API
  slug: effect-photonics-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-wp-v2-api-openapi.yml
- filename: effect-photonics-effect-v1-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Effect/v1 API
  slug: effect-photonics-effect-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-effect-v1-api-openapi.yml
- filename: effect-photonics-mcp-api-openapi.yml
  format: yaml
  label: EFFECT Photonics MCP API
  slug: effect-photonics-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-mcp-api-openapi.yml
- filename: effect-photonics-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Wp Abilities/v1 API
  slug: effect-photonics-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-wp-abilities-v1-api-openapi.yml
- filename: effect-photonics-oembed-1-0-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Oembed/1.0 API
  slug: effect-photonics-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-oembed-1-0-api-openapi.yml
- filename: effect-photonics-root-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Root API
  slug: effect-photonics-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-root-api-openapi.yml
authorization_urls:
- https://effectphotonics.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Effect Photonics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EFFECT Photonics publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the EFFECT Photonics API on a user''s behalf.


  Tokens are issued from https://effectphotonics.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EFFECT Photonics
provider_slug: effect-photonics
schemes:
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched 2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://effectphotonics.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://effectphotonics.com/oauth/token
  name: mcpOAuth2
  source: openapi/effect-photonics-effect-v1-api-openapi.yml
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched 2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://effectphotonics.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://effectphotonics.com/oauth/token
  name: mcpOAuth2
  source: openapi/effect-photonics-mcp-api-openapi.yml
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched 2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://effectphotonics.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://effectphotonics.com/oauth/token
  name: mcpOAuth2
  source: openapi/effect-photonics-oembed-1-0-api-openapi.yml
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched 2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://effectphotonics.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://effectphotonics.com/oauth/token
  name: mcpOAuth2
  source: openapi/effect-photonics-root-api-openapi.yml
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched 2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://effectphotonics.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://effectphotonics.com/oauth/token
  name: mcpOAuth2
  source: openapi/effect-photonics-wp-abilities-v1-api-openapi.yml
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched 2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://effectphotonics.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://effectphotonics.com/oauth/token
  name: mcpOAuth2
  source: openapi/effect-photonics-wp-v2-api-openapi.yml
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the site's Model Context Protocol server.
  flows:
  - authorizationCode
  scope: mcp
slug: effect-photonics-scopes
source_filename: effect-photonics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/effect-photonics-effect-v1-api-openapi.yml, openapi/effect-photonics-mcp-api-openapi.yml,\n  openapi/effect-photonics-oembed-1-0-api-openapi.yml, openapi/effect-photonics-root-api-openapi.yml,\n  openapi/effect-photonics-wp-abilities-v1-api-openapi.yml, openapi/effect-photonics-wp-v2-api-openapi.yml\nschemes:\n- name: mcpOAuth2\n  source: openapi/effect-photonics-effect-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://effectphotonics.com/oauth/authorize\n    tokenUrl: https://effectphotonics.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched\n    2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC\n    9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.\n- name: mcpOAuth2\n\
  \  source: openapi/effect-photonics-mcp-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://effectphotonics.com/oauth/authorize\n    tokenUrl: https://effectphotonics.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched\n    2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC\n    9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.\n- name: mcpOAuth2\n  source: openapi/effect-photonics-oembed-1-0-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://effectphotonics.com/oauth/authorize\n    tokenUrl: https://effectphotonics.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server\
  \ (fetched\n    2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC\n    9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.\n- name: mcpOAuth2\n  source: openapi/effect-photonics-root-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://effectphotonics.com/oauth/authorize\n    tokenUrl: https://effectphotonics.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched\n    2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC\n    9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.\n- name: mcpOAuth2\n  source: openapi/effect-photonics-wp-abilities-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://effectphotonics.com/oauth/authorize\n    tokenUrl: https://effectphotonics.com/oauth/token\n\
  \  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched\n    2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC\n    9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.\n- name: mcpOAuth2\n  source: openapi/effect-photonics-wp-v2-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://effectphotonics.com/oauth/authorize\n    tokenUrl: https://effectphotonics.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched\n    2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC\n    9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.\nscopes:\n- scope: mcp\n  description:\
  \ Access the site's Model Context Protocol server.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/effect-photonics-effect-v1-api-openapi.yml\n  - openapi/effect-photonics-mcp-api-openapi.yml\n  - openapi/effect-photonics-oembed-1-0-api-openapi.yml\n  - openapi/effect-photonics-root-api-openapi.yml\n  - openapi/effect-photonics-wp-abilities-v1-api-openapi.yml\n  - openapi/effect-photonics-wp-v2-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/scopes/effect-photonics-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Photonics
- Optical Networking
- Optical Transceivers
- Photonic Integrated Circuits
- Semiconductors
- Telecommunications
- Data Center Interconnect
- Hardware
- Model Context Protocol
- WordPress
- Netherlands
token_urls:
- https://effectphotonics.com/oauth/token
---
