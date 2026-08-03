---
api_specs:
- filename: starfish-space-wordpress-openapi.yml
  format: yaml
  label: Starfish Space Website Content API
  slug: starfish-space-website-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starfish-space/refs/heads/main/openapi/starfish-space-wordpress-openapi.yml
authorization_urls:
- https://www.starfishspace.com/oauth/authorize
description: ''
docs: https://www.starfishspace.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Starfish Space Scopes
name_suffix: OAuth Scopes
note: Scopes come from the provider's own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata, not from an OpenAPI. The WordPress REST API itself declares no oauth2 security scheme; OAuth here guards the MCP server only.
overview: 'Starfish Space publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Starfish Space API on a user''s behalf.


  Tokens are issued from https://www.starfishspace.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Starfish Space
provider_slug: starfish-space
schemes:
- flows:
  - authorizationUrl: https://www.starfishspace.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://www.starfishspace.com/oauth/revoke
    tokenUrl: https://www.starfishspace.com/oauth/token
  name: mcp-oauth-server
  protected_resource: https://www.starfishspace.com/wp-json/mcp/mcp-oauth-server
  source: https://www.starfishspace.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: The single scope advertised by the Starfish Space authorization server; grants access to the MCP protected resource at /wp-json/mcp/mcp-oauth-server. The provider publishes no further scope breakdown.
  flows:
  - authorizationCode
  scope: mcp
slug: starfish-space-scopes
source_filename: starfish-space-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://www.starfishspace.com/.well-known/oauth-authorization-server\ndocs: https://www.starfishspace.com/.well-known/oauth-protected-resource\nnote: >-\n  Scopes come from the provider's own RFC 8414 authorization-server metadata and RFC 9728\n  protected-resource metadata, not from an OpenAPI. The WordPress REST API itself declares no oauth2\n  security scheme; OAuth here guards the MCP server only.\nschemes:\n- name: mcp-oauth-server\n  source: https://www.starfishspace.com/.well-known/oauth-authorization-server\n  protected_resource: https://www.starfishspace.com/wp-json/mcp/mcp-oauth-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.starfishspace.com/oauth/authorize\n    tokenUrl: https://www.starfishspace.com/oauth/token\n    revocationUrl: https://www.starfishspace.com/oauth/revoke\n    pkce: S256\nscopes:\n- scope: mcp\n  description: >-\n    The single scope advertised by the Starfish\
  \ Space authorization server; grants access to the\n    MCP protected resource at /wp-json/mcp/mcp-oauth-server. The provider publishes no further\n    scope breakdown.\n  flows: [authorizationCode]\n  sources:\n  - https://www.starfishspace.com/.well-known/oauth-authorization-server\n  - https://www.starfishspace.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starfish-space/refs/heads/main/scopes/starfish-space-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Aerospace
- Space
- Satellites
- Satellite Servicing
- Spacecraft
- Space Robotics
- Defense
- Content Management
- Model Context Protocol
token_urls:
- https://www.starfishspace.com/oauth/token
---
