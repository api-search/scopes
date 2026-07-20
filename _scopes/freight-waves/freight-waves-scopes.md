---
api_specs:
- filename: freight-waves-sonar-openapi.yml
  format: yaml
  label: SONAR API
  slug: sonar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freight-waves/refs/heads/main/openapi/freight-waves-sonar-openapi.yml
authorization_urls:
- https://api.freightwaves.com/oauth/authorize
description: ''
docs: https://api.freightwaves.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Freight Waves Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Freight Waves publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Freight Waves API on a user''s behalf.


  Tokens are issued from https://api.freightwaves.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Freight Waves
provider_slug: freight-waves
schemes:
- flows:
  - authorizationUrl: https://api.freightwaves.com/oauth/authorize
    codeChallengeMethods:
    - S256
    flow: authorizationCode
    tokenUrl: https://api.freightwaves.com/oauth/token
  name: mcpOAuth
  source: well-known/freight-waves-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp:read
scopes:
- description: Read-only access to SONAR freight-market data through the MCP server.
  flows:
  - authorizationCode
  scope: mcp:read
slug: freight-waves-scopes
source_filename: freight-waves-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: well-known/freight-waves-oauth-authorization-server.json\ndocs: https://api.freightwaves.com/.well-known/oauth-authorization-server\nnotes: >-\n  Scopes here belong to the FreightWaves hosted MCP server's OAuth 2.1\n  authorization server (issuer https://api.freightwaves.com), not the SONAR REST\n  API (which uses opaque bearer tokens with no scope surface).\nschemes:\n- name: mcpOAuth\n  source: well-known/freight-waves-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.freightwaves.com/oauth/authorize\n    tokenUrl: https://api.freightwaves.com/oauth/token\n    codeChallengeMethods: [S256]\nscopes:\n- scope: mcp:read\n  description: Read-only access to SONAR freight-market data through the MCP server.\n  flows: [authorizationCode]\n  sources: [well-known/freight-waves-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freight-waves/refs/heads/main/scopes/freight-waves-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Freight
- Logistics
- Supply Chain
- Transportation
- Trucking
- Market Data
- Analytics
- Freight Rates
- SONAR
token_urls:
- https://api.freightwaves.com/oauth/token
---
