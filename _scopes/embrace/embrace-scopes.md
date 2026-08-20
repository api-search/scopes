---
authorization_urls:
- https://dash.embrace.io/oauth/authorize
description: Embrace's only OAuth scope surface is the MCP server. Three scopes are advertised in both the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata, and the same three are selectable when issuing a service-account bearer token in the dashboard. There is no OpenAPI document declaring oauth2 securitySchemes, so the derive-oauth-scopes.py pass has nothing to read; this file is built from the live discovery documents plus the docs, which is a stronger source than a derivation. The Metrics and Custom Metrics APIs are bearer-token APIs with no scope model at all.
docs: https://embrace.io/docs/product/settings/service-accounts/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Embrace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Embrace publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Embrace API on a user''s behalf.


  Tokens are issued from https://dash-api.embrace.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Embrace
provider_slug: embrace
schemes:
- authorization_servers:
  - https://dash-api.embrace.io
  bearer_methods_supported:
  - header
  flows:
  - authorizationUrl: https://dash.embrace.io/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://dash-api.embrace.io/oauth/token
  name: EmbraceMcpOAuth2
  resource: https://mcp.embrace.io/mcp
  resource_name: Embrace MCP
  source: well-known/embrace-mcp-oauth-authorization-server.json
scope_count: 3
scope_names:
- mcp:tools:call
- mcp:read
- mcp:write
scopes:
- description: Invoke MCP tools. Required for any MCP access — a token without it cannot call a single tool regardless of what else it carries.
  flows:
  - authorizationCode
  scope: mcp:tools:call
- description: Read data through the MCP server.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write data through the MCP server.
  flows:
  - authorizationCode
  scope: mcp:write
slug: embrace-scopes
source_filename: embrace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://mcp.embrace.io/.well-known/oauth-authorization-server\ndocs: https://embrace.io/docs/product/settings/service-accounts/\ndescription: >-\n  Embrace's only OAuth scope surface is the MCP server. Three scopes are advertised in both the\n  RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata, and the\n  same three are selectable when issuing a service-account bearer token in the dashboard. There\n  is no OpenAPI document declaring oauth2 securitySchemes, so the derive-oauth-scopes.py pass has\n  nothing to read; this file is built from the live discovery documents plus the docs, which is a\n  stronger source than a derivation.\n  The Metrics and Custom Metrics APIs are bearer-token APIs with no scope model at all.\nschemes:\n  - name: EmbraceMcpOAuth2\n    source: well-known/embrace-mcp-oauth-authorization-server.json\n    resource: https://mcp.embrace.io/mcp\n    resource_name: Embrace MCP\n\
  \    authorization_servers: [https://dash-api.embrace.io]\n    bearer_methods_supported: [header]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://dash.embrace.io/oauth/authorize\n        tokenUrl: https://dash-api.embrace.io/oauth/token\n        pkce: S256\nscopes:\n  - scope: mcp:tools:call\n    description: >-\n      Invoke MCP tools. Required for any MCP access — a token without it cannot call a single\n      tool regardless of what else it carries.\n    flows: [authorizationCode]\n    required: true\n    sources: [well-known/embrace-mcp-oauth-authorization-server.json, https://embrace.io/docs/product/settings/service-accounts/]\n  - scope: mcp:read\n    description: Read data through the MCP server.\n    flows: [authorizationCode]\n    required: false\n    sources: [well-known/embrace-mcp-oauth-authorization-server.json, https://embrace.io/docs/product/settings/service-accounts/]\n  - scope: mcp:write\n    description: Write data through the MCP server.\n\
  \    flows: [authorizationCode]\n    required: false\n    sources: [well-known/embrace-mcp-oauth-authorization-server.json, https://embrace.io/docs/product/settings/service-accounts/]\nnotes:\n  - >-\n    All 19 published MCP tools are read-oriented (list_/get_), so what mcp:write currently grants\n    is not documented. Recorded as advertised, not interpreted.\n  - >-\n    The WordPress site MCP at https://embrace.io/wp-json/mcp/mcp-oauth-server advertises a single\n    coarse \"mcp\" scope from a separate issuer (https://embrace.io). It is not part of the product\n    API and is not merged into the scope list above.\nscope_count: 3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embrace/refs/heads/main/scopes/embrace-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Observability
- Monitoring
- Mobile
- Real User Monitoring
- OpenTelemetry
- Metrics
- Crash Reporting
- Application Performance Monitoring
- Developer Tools
- MCP
token_urls:
- https://dash-api.embrace.io/oauth/token
---
