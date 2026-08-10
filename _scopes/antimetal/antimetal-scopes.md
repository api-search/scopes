---
api_specs:
- filename: antimetal-artifacts-api-openapi.yml
  format: yaml
  label: Antimetal Artifacts API
  slug: antimetal-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-artifacts-api-openapi.yml
- filename: antimetal-issues-api-openapi.yml
  format: yaml
  label: Antimetal Issues API
  slug: antimetal-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-issues-api-openapi.yml
- filename: antimetal-query-api-openapi.yml
  format: yaml
  label: Antimetal Query API
  slug: antimetal-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-query-api-openapi.yml
authorization_urls:
- https://antimetal.authkit.app/oauth2/authorize
description: ''
docs: https://docs.antimetal.com/connect
flows:
- authorizationCode
- deviceCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Antimetal Scopes
name_suffix: OAuth Scopes
note: The Antimetal External REST API uses bearer API keys only and declares no oauth2 security scheme, so derive-oauth-scopes.py found nothing in openapi/. The OAuth surface belongs to the remote MCP server, whose RFC 8414 authorization-server metadata is anonymously readable and is the source below.
overview: 'Antimetal publishes 4 OAuth 2.0 scopes via the authorizationCode, deviceCode, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Antimetal API on a user''s behalf.


  Tokens are issued from https://antimetal.authkit.app/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Antimetal
provider_slug: antimetal
schemes:
- endpoints:
    introspection_endpoint: https://antimetal.authkit.app/oauth2/introspection
    jwks_uri: https://antimetal.authkit.app/oauth2/jwks
    registration_endpoint: https://antimetal.authkit.app/oauth2/register
  flows:
  - authorizationUrl: https://antimetal.authkit.app/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://antimetal.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://antimetal.authkit.app/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://antimetal.authkit.app/oauth2/token
  - flow: refreshToken
    tokenUrl: https://antimetal.authkit.app/oauth2/token
  issuer: https://antimetal.authkit.app
  name: mcp-oauth2
  protected_resource: https://mcp.antimetal.com
  provider: WorkOS AuthKit
  source: https://mcp.antimetal.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issues an ID token identifying the user.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Email address claim for the authenticated user.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Issues a refresh token so the client can act after the access token expires.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: antimetal-scopes
source_filename: antimetal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://mcp.antimetal.com/.well-known/oauth-authorization-server\ndocs: https://docs.antimetal.com/connect\napplies_to: mcp/antimetal-mcp.yml\nnote: The Antimetal External REST API uses bearer API keys only and declares no oauth2\n  security scheme, so derive-oauth-scopes.py found nothing in openapi/. The OAuth surface\n  belongs to the remote MCP server, whose RFC 8414 authorization-server metadata is\n  anonymously readable and is the source below.\nschemes:\n- name: mcp-oauth2\n  source: https://mcp.antimetal.com/.well-known/oauth-authorization-server\n  issuer: https://antimetal.authkit.app\n  provider: WorkOS AuthKit\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://antimetal.authkit.app/oauth2/authorize\n    tokenUrl: https://antimetal.authkit.app/oauth2/token\n    pkce: [S256]\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://antimetal.authkit.app/oauth2/device_authorization\n    tokenUrl:\
  \ https://antimetal.authkit.app/oauth2/token\n  - flow: refreshToken\n    tokenUrl: https://antimetal.authkit.app/oauth2/token\n  endpoints:\n    jwks_uri: https://antimetal.authkit.app/oauth2/jwks\n    introspection_endpoint: https://antimetal.authkit.app/oauth2/introspection\n    registration_endpoint: https://antimetal.authkit.app/oauth2/register\n  token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n  protected_resource: https://mcp.antimetal.com\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token identifying the user.\n  flows: [authorizationCode, deviceCode]\n- scope: profile\n  description: Basic profile claims for the authenticated user.\n  flows: [authorizationCode, deviceCode]\n- scope: email\n  description: Email address claim for the authenticated user.\n  flows: [authorizationCode, deviceCode]\n- scope: offline_access\n  description: Issues a refresh token so the client can act after the access token\n\
  \    expires.\n  flows: [authorizationCode, deviceCode]\ngaps:\n- The advertised scopes are the standard OIDC identity set only. Antimetal publishes\n  no resource-level or tool-level scopes (no read/write separation across issues, artifacts\n  or query), so an MCP token is not scoped to a subset of the tool surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/scopes/antimetal-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode/refreshToken
tags:
- Company
- Observability
- Incident Management
- Site Reliability Engineering
- Artificial Intelligence
- Agents
- DevOps
- Cloud Infrastructure
- Kubernetes
- Root Cause Analysis
- MCP
token_urls:
- https://antimetal.authkit.app/oauth2/token
---
