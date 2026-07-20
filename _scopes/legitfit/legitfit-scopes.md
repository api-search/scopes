---
authorization_urls:
- https://legitfit.com/api/oauth2/authorize
description: ''
docs: https://legitfit.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Legitfit Scopes
name_suffix: OAuth Scopes
note: LegitFit publishes no OpenAPI, so these scopes were read directly from the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata. Both documents advertise the same two scopes, which gate the MCP server at https://legitfit.com/api/mcp. LegitFit publishes no human-readable scope reference page; the descriptions below restate the scope names and the resource they protect, and no finer-grained permission mapping is asserted.
overview: 'LegitFit publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LegitFit API on a user''s behalf.


  Tokens are issued from https://legitfit.com/api/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LegitFit
provider_slug: legitfit
schemes:
- flows:
  - authorizationUrl: https://legitfit.com/api/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://legitfit.com/api/oauth2/token
  name: LegitFitOAuth2
  source: well-known/legitfit-oauth-authorization-server.json
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Read access to the LegitFit MCP server at https://legitfit.com/api/mcp.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access to the LegitFit MCP server at https://legitfit.com/api/mcp.
  flows:
  - authorizationCode
  scope: mcp:write
slug: legitfit-scopes
source_filename: legitfit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://legitfit.com/.well-known/oauth-authorization-server\ndocs: https://legitfit.com/.well-known/oauth-protected-resource\nnote: >-\n  LegitFit publishes no OpenAPI, so these scopes were read directly from the\n  RFC 8414 authorization-server metadata and the RFC 9728 protected-resource\n  metadata. Both documents advertise the same two scopes, which gate the MCP\n  server at https://legitfit.com/api/mcp. LegitFit publishes no human-readable\n  scope reference page; the descriptions below restate the scope names and the\n  resource they protect, and no finer-grained permission mapping is asserted.\nschemes:\n- name: LegitFitOAuth2\n  source: well-known/legitfit-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://legitfit.com/api/oauth2/authorize\n    tokenUrl: https://legitfit.com/api/oauth2/token\nscopes:\n- scope: mcp:read\n  description: Read access to the LegitFit MCP\
  \ server at https://legitfit.com/api/mcp.\n  flows:\n  - authorizationCode\n  resources:\n  - https://legitfit.com/api/mcp\n  sources:\n  - well-known/legitfit-oauth-authorization-server.json\n  - well-known/legitfit-oauth-protected-resource.json\n- scope: mcp:write\n  description: Write access to the LegitFit MCP server at https://legitfit.com/api/mcp.\n  flows:\n  - authorizationCode\n  resources:\n  - https://legitfit.com/api/mcp\n  sources:\n  - well-known/legitfit-oauth-authorization-server.json\n  - well-known/legitfit-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legitfit/refs/heads/main/scopes/legitfit-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Fitness
- Gym Management
- Studio Management
- Scheduling
- Memberships
- Payments
- SaaS
- MCP
- Ireland
token_urls:
- https://legitfit.com/api/oauth2/token
---
