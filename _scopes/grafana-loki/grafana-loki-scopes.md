---
authorization_urls: []
description: 'Grafana Loki itself has no OAuth surface. Two scope vocabularies govern access to Loki data: the OAuth 2.1 scopes published by the hosted Grafana Cloud MCP server (read anonymously from its RFC 8414 authorization-server metadata), and the Grafana Cloud / Grafana Enterprise Logs access policy scopes named in the Loki HTTP API reference for the logs surface.'
docs:
- https://grafana.com/docs/grafana-cloud/ai-tools/mcp-servers/cloud-mcp/
- https://grafana.com/docs/loki/latest/reference/loki-http-api/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Grafana Loki Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Grafana Loki uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Grafana Loki
provider_slug: grafana-loki
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: grafana-loki-scopes
source_filename: grafana-loki-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://mcp.grafana.com/.well-known/oauth-authorization-server\nname: Grafana Loki OAuth scopes and access policy scopes\ndescription: >-\n  Grafana Loki itself has no OAuth surface. Two scope vocabularies govern access to Loki data: the\n  OAuth 2.1 scopes published by the hosted Grafana Cloud MCP server (read anonymously from its\n  RFC 8414 authorization-server metadata), and the Grafana Cloud / Grafana Enterprise Logs access\n  policy scopes named in the Loki HTTP API reference for the logs surface.\noauth:\n  issuer: https://mcp.grafana.com/mcp\n  authorization_endpoint: https://mcp.grafana.com/mcp/oauth/authorize\n  token_endpoint: https://mcp.grafana.com/mcp/oauth/token\n  registration_endpoint: https://mcp.grafana.com/mcp/oauth/register\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  dynamic_client_registration:\
  \ true\n  metadata_probed:\n    - {url: 'https://mcp.grafana.com/.well-known/oauth-authorization-server', status: 200}\n    - {url: 'https://mcp.grafana.com/.well-known/oauth-protected-resource', status: 200}\nscopes:\n  - name: grafana:read\n    vocabulary: mcp-oauth\n    description: Read Grafana resources through the hosted Grafana Cloud MCP server.\n    source: https://mcp.grafana.com/.well-known/oauth-authorization-server\n  - name: grafana:query\n    vocabulary: mcp-oauth\n    description: >-\n      Execute datasource queries through the hosted Grafana Cloud MCP server. This is the scope the\n      Loki query tools (query_loki_logs, query_loki_stats, query_loki_patterns,\n      list_loki_label_names, list_loki_label_values) run under.\n    source: https://mcp.grafana.com/.well-known/oauth-authorization-server\n  - name: grafana:write\n    vocabulary: mcp-oauth\n    description: Write Grafana resources through the hosted Grafana Cloud MCP server.\n    source: https://mcp.grafana.com/.well-known/oauth-authorization-server\n\
  \  - name: logs:read\n    vocabulary: grafana-cloud-access-policy\n    description: Read/query logs for a tenant on Grafana Cloud Logs or Grafana Enterprise Logs.\n    source: https://grafana.com/docs/loki/latest/reference/loki-http-api/\n  - name: logs:write\n    vocabulary: grafana-cloud-access-policy\n    description: Push logs for a tenant on Grafana Cloud Logs or Grafana Enterprise Logs.\n    source: https://grafana.com/docs/loki/latest/reference/loki-http-api/\n  - name: logs:delete\n    vocabulary: grafana-cloud-access-policy\n    description: >-\n      Required on the access policy behind the token used with the log deletion endpoints\n      (POST/GET/DELETE /loki/api/v1/delete) for the tenant named in the Basic auth user field.\n    source: https://grafana.com/docs/loki/latest/reference/loki-http-api/\nrbac_scopes_mcp:\n  note: >-\n    Inside Grafana, every Loki MCP tool additionally requires the RBAC action datasources:query\n    scoped to the Loki datasource UID (datasources:uid:loki-uid).\n\
  \  action: datasources:query\n  scope: 'datasources:uid:loki-uid'\nscope_count: 6\ndocs:\n  - https://grafana.com/docs/grafana-cloud/ai-tools/mcp-servers/cloud-mcp/\n  - https://grafana.com/docs/loki/latest/reference/loki-http-api/\nchecked: '2026-08-27'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grafana-loki/refs/heads/main/scopes/grafana-loki-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Logs
- Logging
- Log Aggregation
- Observability
- Monitoring
- Open Source
- LogQL
- OpenTelemetry
- Telemetry
- Kubernetes
- Cloud Native
token_urls: []
---
