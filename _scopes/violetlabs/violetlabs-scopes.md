---
authorization_urls:
- https://app.violetlabs.com/api/oauth/authorize
description: OAuth 2.0 scopes advertised by the Violet Labs authorization server. The server (app.violetlabs.com) publishes a single scope, `mcp`, used to authorize the hosted Model Context Protocol server against a selected workspace. The REST Explore API itself is authorized by API key rather than OAuth scopes.
docs: https://docs.violetlabs.com/ai/mcp
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Violetlabs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Violetlabs publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Violetlabs API on a user''s behalf.


  Tokens are issued from https://app.violetlabs.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Violetlabs
provider_slug: violetlabs
schemes:
- flows:
  - authorizationUrl: https://app.violetlabs.com/api/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://app.violetlabs.com/api/oauth/token
  - flow: clientCredentials
    tokenUrl: https://app.violetlabs.com/api/oauth/token
  name: oauth2
  source: well-known/violetlabs-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Authorize the Violet hosted MCP server to access the selected workspace's structured data on the user's behalf.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp
slug: violetlabs-scopes
source_filename: violetlabs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://app.violetlabs.com/.well-known/oauth-authorization-server\ndocs: https://docs.violetlabs.com/ai/mcp\ndescription: >-\n  OAuth 2.0 scopes advertised by the Violet Labs authorization server. The\n  server (app.violetlabs.com) publishes a single scope, `mcp`, used to authorize\n  the hosted Model Context Protocol server against a selected workspace. The\n  REST Explore API itself is authorized by API key rather than OAuth scopes.\nschemes:\n- name: oauth2\n  source: well-known/violetlabs-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.violetlabs.com/api/oauth/authorize\n    tokenUrl: https://app.violetlabs.com/api/oauth/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://app.violetlabs.com/api/oauth/token\nscopes:\n- scope: mcp\n  description: >-\n    Authorize the Violet hosted MCP server to access the selected workspace's\n    structured\
  \ data on the user's behalf.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/violetlabs-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/violetlabs/refs/heads/main/scopes/violetlabs-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Hardware
- Engineering
- Manufacturing
- PLM
- ERP
- Data Integration
- Requirements Management
- Aerospace
- Defense
- MCP
- Systems Engineering
token_urls:
- https://app.violetlabs.com/api/oauth/token
---
