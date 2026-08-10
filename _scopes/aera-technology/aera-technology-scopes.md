---
authorization_urls:
- https://www.aeratechnology.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Aera Technology Scopes
name_suffix: OAuth Scopes
note: Scopes as advertised by Aera Technology's own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata. Aera publishes no scopes / permissions reference page, so this is the complete publicly observable scope surface — a single coarse scope. Nothing is inferred.
overview: 'Aera Technology publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aera Technology API on a user''s behalf.


  Tokens are issued from https://www.aeratechnology.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aera Technology
provider_slug: aera-technology
schemes:
- flows:
  - authorizationUrl: https://www.aeratechnology.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.aeratechnology.com/oauth/token
  name: mcp-oauth
  source: well-known/aera-technology-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the Aera Technology MCP server at /wp-json/mcp/mcp-oauth-server. Advertised in both scopes_supported lists; no finer-grained or per-tool scopes are published.
  flows:
  - authorizationCode
  scope: mcp
slug: aera-technology-scopes
source_filename: aera-technology-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://www.aeratechnology.com/.well-known/oauth-authorization-server\nnote: >-\n  Scopes as advertised by Aera Technology's own RFC 8414 authorization-server\n  metadata and RFC 9728 protected-resource metadata. Aera publishes no scopes /\n  permissions reference page, so this is the complete publicly observable scope\n  surface — a single coarse scope. Nothing is inferred.\nschemes:\n- name: mcp-oauth\n  source: well-known/aera-technology-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.aeratechnology.com/oauth/authorize\n    tokenUrl: https://www.aeratechnology.com/oauth/token\nscopes:\n- scope: mcp\n  description: >-\n    Access the Aera Technology MCP server at\n    /wp-json/mcp/mcp-oauth-server. Advertised in both scopes_supported lists; no\n    finer-grained or per-tool scopes are published.\n  flows: [authorizationCode]\n  sources:\n  - well-known/aera-technology-oauth-authorization-server.json\n\
  \  - well-known/aera-technology-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://www.aeratechnology.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://www.aeratechnology.com/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aera-technology/refs/heads/main/scopes/aera-technology-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Decision Intelligence
- Artificial Intelligence
- Enterprise Software
- Supply Chain
- Automation
- Analytics
- Agents
token_urls:
- https://www.aeratechnology.com/oauth/token
---
