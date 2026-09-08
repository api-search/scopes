---
api_specs:
- filename: betterstack-heartbeats-api-openapi.yml
  format: yaml
  label: Better Stack Heartbeats API
  slug: betterstack-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/openapi/betterstack-heartbeats-api-openapi.yml
- filename: betterstack-incidents-api-openapi.yml
  format: yaml
  label: Better Stack Incidents API
  slug: betterstack-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/openapi/betterstack-incidents-api-openapi.yml
- filename: betterstack-monitors-api-openapi.yml
  format: yaml
  label: Better Stack Monitors API
  slug: betterstack-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/openapi/betterstack-monitors-api-openapi.yml
- filename: betterstack-status-pages-api-openapi.yml
  format: yaml
  label: Better Stack Status Pages API
  slug: betterstack-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/openapi/betterstack-status-pages-api-openapi.yml
authorization_urls: []
description: ''
docs: https://betterstack.com/docs/getting-started/integrations/mcp/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Betterstack Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Better Stack uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Better Stack
provider_slug: betterstack
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: betterstack-scopes
source_filename: betterstack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://betterstack.com/.well-known/oauth-authorization-server (RFC 8414, HTTP 200) and\n  https://mcp.betterstack.com/.well-known/oauth-protected-resource (RFC 9728, HTTP 200),\n  both fetched 2026-09-04 and saved verbatim under well-known/.\ndocs: https://betterstack.com/docs/getting-started/integrations/mcp/\nprovider: Better Stack\nproviderId: betterstack\nauthorization_server: https://betterstack.com\nissuer: https://betterstack.com\nauthorization_endpoint: https://betterstack.com/oauth/authorize\ntoken_endpoint: https://betterstack.com/oauth/token\nregistration_endpoint: https://betterstack.com/oauth/register\ndynamic_client_registration: true\ngrant_types_supported: [authorization_code, refresh_token]\ncode_challenge_methods_supported: [S256]\ntoken_endpoint_auth_methods_supported: [none]\nprotected_resources:\n- resource: https://mcp.betterstack.com\n  resource_name: Better Stack MCP Server\n  bearer_methods_supported:\
  \ [header]\nscopes:\n- name: read\n  description: Read access to Better Stack resources. Declared in both the authorization-server\n    metadata and the MCP protected-resource metadata; Better Stack publishes no finer-grained\n    description of what it covers.\n  source: /.well-known/oauth-authorization-server\n- name: write\n  description: Write access to Better Stack resources. Declared in both discovery documents;\n    no per-product or per-resource narrowing is offered.\n  source: /.well-known/oauth-authorization-server\ncoverage:\n  scope_count: 2\n  granularity: coarse\n  note: >-\n    Two scopes cover a ~106-tool agent surface spanning uptime monitoring, incident management,\n    on-call paging, status pages, ClickHouse query execution over telemetry, dashboards, error\n    triage and team-member administration. `write` grants an agent the ability to page an\n    on-call engineer, delete a dashboard and remove a team member with the same token. The only\n    real narrowing Better\
  \ Stack offers is not a scope at all — it is the X-MCP-Tools-Only /\n    X-MCP-Tools-Except header allowlist documented for the MCP server.\nrest_api_note: >-\n  These scopes apply to the OAuth surface (the MCP server) only. The Uptime v2, Telemetry v1\n  and Errors v1 REST APIs authenticate with static bearer tokens that carry no scope at all —\n  a token is either global or team-scoped, and within its team it is unrestricted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/scopes/betterstack-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Observability
- Uptime Monitoring
- Incidents
- Logs
- Monitoring
- Status Pages
- On-Call
- Error Tracking
- OpenTelemetry
- Model Context Protocol
token_urls: []
---
