---
authorization_urls:
- https://www.dispatchhealth.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Dispatchhealth Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DispatchHealth publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the DispatchHealth API on a user''s behalf.


  Tokens are issued from https://www.dispatchhealth.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DispatchHealth
provider_slug: dispatchhealth
schemes:
- flows:
  - authorizationUrl: https://www.dispatchhealth.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.dispatchhealth.com/oauth/token
  name: MCPOAuth2
  source: well-known/dispatchhealth-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the MCP server at https://www.dispatchhealth.com/wp-json/mcp/mcp-oauth-server
  flows:
  - authorizationCode
  scope: mcp
slug: dispatchhealth-scopes
source_filename: dispatchhealth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://www.dispatchhealth.com/.well-known/oauth-authorization-server\ndocs: null\nschemes:\n- name: MCPOAuth2\n  source: well-known/dispatchhealth-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.dispatchhealth.com/oauth/authorize\n    tokenUrl: https://www.dispatchhealth.com/oauth/token\nscopes:\n- scope: mcp\n  description: Access the MCP server at https://www.dispatchhealth.com/wp-json/mcp/mcp-oauth-server\n  flows: [authorizationCode]\n  sources:\n  - well-known/dispatchhealth-oauth-authorization-server.json\n  - well-known/dispatchhealth-oauth-protected-resource.json\nnotes: A single coarse scope is advertised by both the RFC 8414 authorization-server\n  metadata and the RFC 9728 protected-resource metadata. No scope/permission reference\n  page is published, and no finer-grained scopes were observed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dispatchhealth/refs/heads/main/scopes/dispatchhealth-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Healthcare
- Health Systems
- Hospital at Home
- Home Health
- Urgent Care
- Care Delivery
- Medical Services
- Telehealth
- Digital Health
token_urls:
- https://www.dispatchhealth.com/oauth/token
---
