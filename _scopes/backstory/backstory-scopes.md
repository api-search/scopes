---
authorization_urls:
- https://mcp.backstory.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Backstory Scopes
name_suffix: OAuth Scopes
note: Backstory publishes no OpenAPI and no scopes/permissions reference page, so this file is read directly off the MCP server's RFC 8414 and RFC 9728 discovery documents (both HTTP 200, anonymous). Nothing here is inferred.
overview: 'Backstory publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Backstory API on a user''s behalf.


  Tokens are issued from https://mcp.backstory.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Backstory
provider_slug: backstory
schemes:
- flows:
  - authorizationUrl: https://mcp.backstory.ai/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://mcp.backstory.ai/token
  issuer: https://mcp.backstory.ai/
  name: backstory-mcp-oauth2
  source: https://mcp.backstory.ai/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- claudeai
scopes:
- description: The only scope advertised by the Backstory MCP authorization server, in both its authorization-server metadata (scopes_supported) and its protected-resource metadata for https://mcp.backstory.ai/mcp. It is a connector-grant marker rather than a capability scope.
  flows:
  - authorizationCode
  scope: claudeai
slug: backstory-scopes
source_filename: backstory-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.backstory.ai/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Backstory publishes no OpenAPI and no scopes/permissions reference page, so\n  this file is read directly off the MCP server's RFC 8414 and RFC 9728\n  discovery documents (both HTTP 200, anonymous). Nothing here is inferred.\nschemes:\n- name: backstory-mcp-oauth2\n  source: https://mcp.backstory.ai/.well-known/oauth-authorization-server\n  issuer: https://mcp.backstory.ai/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.backstory.ai/authorize\n    tokenUrl: https://mcp.backstory.ai/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: claudeai\n  description: >-\n    The only scope advertised by the Backstory MCP authorization server, in both\n    its authorization-server metadata (scopes_supported) and its\n    protected-resource metadata for https://mcp.backstory.ai/mcp. It is a\n    connector-grant marker\
  \ rather than a capability scope.\n  flows: [authorizationCode]\n  sources:\n  - https://mcp.backstory.ai/.well-known/oauth-authorization-server\n  - https://mcp.backstory.ai/.well-known/oauth-protected-resource/mcp\nscope_count: 1\nauthorization_note: >-\n  Backstory does not express authorization as OAuth scopes. Per the provider's\n  MCP article, a connected client \"can only access the same accounts,\n  opportunities, activities, and other sales data that you can already view in\n  Backstory Engagement Dashboards\" — the effective permission set is the\n  authenticating user's own, administered through User Access / Object Visibility\n  settings, not through the token's scope string.\nx-evidence:\n- fetched: '2026-08-14'\n  url: https://mcp.backstory.ai/.well-known/oauth-authorization-server\n  http_status: 200\n- fetched: '2026-08-14'\n  url: https://mcp.backstory.ai/.well-known/oauth-protected-resource/mcp\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstory/refs/heads/main/scopes/backstory-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Artificial Intelligence
- Revenue Intelligence
- Sales
- CRM
- Sales Analytics
- Forecasting
- Revenue Operations
- MCP
- AI Agents
token_urls:
- https://mcp.backstory.ai/token
---
