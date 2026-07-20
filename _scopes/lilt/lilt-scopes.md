---
api_specs:
- filename: lilt-openapi-original.yml
  format: yaml
  label: LILT API
  slug: lilt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-openapi-original.yml
authorization_urls:
- https://blissful-celebration-62.authkit.app/oauth2/authorize
description: The LILT REST API at api.lilt.com does NOT use OAuth — it authenticates with an organization API key over HTTP Basic (or a `key` query parameter), so it has no scope surface (see authentication/lilt-authentication.yml). The OAuth surface documented here belongs to LILT's hosted remote MCP server at mcp.lilt.com, whose RFC 8414 authorization-server metadata was fetched live. Authorization is delegated to WorkOS AuthKit; the advertised scopes are the standard OIDC set, so LILT does not expose per-capability translation scopes — tool-level authorization is enforced by the MCP server, not by scope.
docs: https://support.lilt.com/kb/LILT-mcp
flows:
- authorizationCode
- deviceCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Lilt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lilt publishes 4 OAuth 2.0 scopes via the authorizationCode, deviceCode, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lilt API on a user''s behalf.


  Tokens are issued from https://blissful-celebration-62.authkit.app/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lilt
provider_slug: lilt
schemes:
- code_challenge_methods_supported:
  - S256
  dynamic_client_registration: https://blissful-celebration-62.authkit.app/oauth2/register
  flows:
  - authorizationUrl: https://blissful-celebration-62.authkit.app/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://blissful-celebration-62.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://blissful-celebration-62.authkit.app/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://blissful-celebration-62.authkit.app/oauth2/token
  - flow: refreshToken
    tokenUrl: https://blissful-celebration-62.authkit.app/oauth2/token
  introspection_endpoint: https://blissful-celebration-62.authkit.app/oauth2/introspection
  issuer: https://blissful-celebration-62.authkit.app
  jwks_uri: https://blissful-celebration-62.authkit.app/oauth2/jwks
  name: MCPOAuth
  source: well-known/lilt-mcp-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OIDC — issue an ID token identifying the LILT MCP app user.
  flows:
  - authorizationCode
  scope: openid
- description: OIDC — access the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: OIDC — access the user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the MCP host can act without re-prompting.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
slug: lilt-scopes
source_filename: lilt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.lilt.com/.well-known/oauth-authorization-server\ndocs: https://support.lilt.com/kb/LILT-mcp\ndescription: >-\n  The LILT REST API at api.lilt.com does NOT use OAuth — it authenticates with\n  an organization API key over HTTP Basic (or a `key` query parameter), so it\n  has no scope surface (see authentication/lilt-authentication.yml). The OAuth\n  surface documented here belongs to LILT's hosted remote MCP server at\n  mcp.lilt.com, whose RFC 8414 authorization-server metadata was fetched live.\n  Authorization is delegated to WorkOS AuthKit; the advertised scopes are the\n  standard OIDC set, so LILT does not expose per-capability translation scopes —\n  tool-level authorization is enforced by the MCP server, not by scope.\napplies_to: LILT MCP server (https://mcp.lilt.com/mcp)\nschemes:\n- name: MCPOAuth\n  type: oauth2\n  source: well-known/lilt-mcp-oauth-authorization-server.json\n  issuer: https://blissful-celebration-62.authkit.app\n\
  \  dynamic_client_registration: https://blissful-celebration-62.authkit.app/oauth2/register\n  jwks_uri: https://blissful-celebration-62.authkit.app/oauth2/jwks\n  introspection_endpoint: https://blissful-celebration-62.authkit.app/oauth2/introspection\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://blissful-celebration-62.authkit.app/oauth2/authorize\n    tokenUrl: https://blissful-celebration-62.authkit.app/oauth2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://blissful-celebration-62.authkit.app/oauth2/device_authorization\n    tokenUrl: https://blissful-celebration-62.authkit.app/oauth2/token\n  - flow: refreshToken\n    tokenUrl: https://blissful-celebration-62.authkit.app/oauth2/token\nscopes:\n- scope: openid\n  description: OIDC — issue an ID token identifying the LILT MCP app user.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/lilt-mcp-oauth-authorization-server.json]\n- scope: profile\n  description: OIDC — access the user's basic profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/lilt-mcp-oauth-authorization-server.json]\n- scope: email\n  description: OIDC — access the user's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/lilt-mcp-oauth-authorization-server.json]\n- scope: offline_access\n  description: Issue a refresh token so the MCP host can act without re-prompting.\n  flows: [authorizationCode, refreshToken]\n  sources: [well-known/lilt-mcp-oauth-authorization-server.json]\nnotes:\n- >-\n  No LILT-specific (translation, job, model) scopes are advertised. Agent\n  capability is bounded by the MCP tool set in mcp/lilt-mcp.yml, not by scope.\n- >-\n  MCP app accounts at mcp.lilt.com are separate from lilt.com platform accounts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/scopes/lilt-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode/refreshToken
tags:
- Company
- Ai
- Translation
- Localization
- Machine Translation
- Language
- Content
- Translation Memory
- Agents
token_urls:
- https://blissful-celebration-62.authkit.app/oauth2/token
---
