---
authorization_urls:
- https://artisight.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Artisight Scopes
name_suffix: OAuth Scopes
note: Derived scopes were not available (no OpenAPI in this repo). These scopes are taken verbatim from the live RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata Artisight serves from artisight.com. Artisight publishes no scopes/permissions reference page.
overview: 'Artisight publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Artisight API on a user''s behalf.


  Tokens are issued from https://artisight.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Artisight
provider_slug: artisight
schemes:
- flows:
  - authorizationUrl: https://artisight.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://artisight.com/oauth/token
  name: mcp-oauth
  source: well-known/artisight-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access to the WordPress MCP server at https://artisight.com/wp-json/mcp/mcp-oauth-server and its backing WordPress Abilities. The only scope advertised by the authorization server; there is no finer-grained read/write split published.
  flows:
  - authorizationCode
  scope: mcp
slug: artisight-scopes
source_filename: artisight-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://artisight.com/.well-known/oauth-authorization-server\ndocs: null\nnote: Derived scopes were not available (no OpenAPI in this repo). These scopes are\n  taken verbatim from the live RFC 8414 authorization-server metadata and the RFC 9728\n  protected-resource metadata Artisight serves from artisight.com. Artisight publishes\n  no scopes/permissions reference page.\nschemes:\n- name: mcp-oauth\n  source: well-known/artisight-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://artisight.com/oauth/authorize\n    tokenUrl: https://artisight.com/oauth/token\nscopes:\n- scope: mcp\n  description: Access to the WordPress MCP server at https://artisight.com/wp-json/mcp/mcp-oauth-server\n    and its backing WordPress Abilities. The only scope advertised by the authorization\n    server; there is no finer-grained read/write split published.\n  flows: [authorizationCode]\n  sources:\n\
  \  - well-known/artisight-oauth-authorization-server.json\n  - well-known/artisight-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://artisight.com/.well-known/oauth-authorization-server\n  http_status: 200\n  scopes_supported: [mcp]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artisight/refs/heads/main/scopes/artisight-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Healthcare
- Artificial Intelligence
- Computer-Vision
- Hospitals
- Ambient Intelligence
- Electronic Health Records
- Machine-Learning
- Patient Monitoring
- Internet of Things
token_urls:
- https://artisight.com/oauth/token
---
