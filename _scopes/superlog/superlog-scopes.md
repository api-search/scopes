---
api_specs:
- filename: superlog-management-openapi.json
  format: json
  label: Superlog Management API
  slug: superlog-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superlog/refs/heads/main/openapi/superlog-management-openapi.json
authorization_urls:
- https://api.superlog.sh/oauth/authorize
description: ''
docs: https://docs.superlog.sh/api/mcp-overview
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Superlog Scopes
name_suffix: OAuth Scopes
note: The Management REST API (/api/v1/*) uses opaque Bearer management keys, not OAuth, and has no scope surface. OAuth 2.0 applies to the Superlog MCP server, whose authorization-server metadata advertises authorization-code + PKCE (S256), refresh tokens, and dynamic client registration. Token-level scoping is also documented for Personal Access Tokens.
overview: 'Superlog publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Superlog API on a user''s behalf.


  Tokens are issued from https://api.superlog.sh/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Superlog
provider_slug: superlog
schemes:
- flows:
  - authorizationUrl: https://api.superlog.sh/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.superlog.sh/oauth/register
    tokenUrl: https://api.superlog.sh/oauth/token
  name: OAuth2 (MCP)
  source: https://api.superlog.sh/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- mcp:read
- superlog:telemetry
- full-access
scopes:
- description: Read access advertised by the MCP OAuth protected-resource / authorization-server metadata.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Telemetry-only token scope — limits an MCP token to the telemetry and project tools (query_logs, query_traces, query_metrics, list_services) with no dashboard/alert/agent access.
  flows:
  - pat
  scope: superlog:telemetry
- description: Default token scope granting all MCP tools (telemetry, incidents, dashboards, alerts, agent config).
  flows:
  - pat
  scope: full-access
slug: superlog-scopes
source_filename: superlog-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.superlog.sh/.well-known/oauth-authorization-server\ndocs: https://docs.superlog.sh/api/mcp-overview\nnote: >-\n  The Management REST API (/api/v1/*) uses opaque Bearer management keys, not OAuth, and has\n  no scope surface. OAuth 2.0 applies to the Superlog MCP server, whose authorization-server\n  metadata advertises authorization-code + PKCE (S256), refresh tokens, and dynamic client\n  registration. Token-level scoping is also documented for Personal Access Tokens.\nschemes:\n- name: OAuth2 (MCP)\n  source: https://api.superlog.sh/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.superlog.sh/oauth/authorize\n    tokenUrl: https://api.superlog.sh/oauth/token\n    registrationUrl: https://api.superlog.sh/oauth/register\n    pkce: S256\nscopes:\n- scope: mcp:read\n  description: Read access advertised by the MCP OAuth protected-resource / authorization-server\
  \ metadata.\n  flows: [authorizationCode]\n  sources: [https://api.superlog.sh/.well-known/oauth-protected-resource]\n- scope: superlog:telemetry\n  description: >-\n    Telemetry-only token scope — limits an MCP token to the telemetry and project tools\n    (query_logs, query_traces, query_metrics, list_services) with no dashboard/alert/agent access.\n  flows: [pat]\n  sources: [https://docs.superlog.sh/api/mcp-overview]\n- scope: full-access\n  description: Default token scope granting all MCP tools (telemetry, incidents, dashboards, alerts, agent config).\n  flows: [pat]\n  sources: [https://docs.superlog.sh/api/mcp-overview]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superlog/refs/heads/main/scopes/superlog-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Observability
- OpenTelemetry
- Monitoring
- Logging
- Tracing
- Metrics
- Incident Management
- AI Agents
- Model Context Protocol
- Developer Tools
token_urls:
- https://api.superlog.sh/oauth/token
---
