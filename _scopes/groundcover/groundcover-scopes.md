---
authorization_urls: []
description: groundcover's only published OAuth surface is the remote MCP server. Its RFC 9728 Protected Resource Metadata declares exactly one scope. The REST API at api.groundcover.com does not use OAuth at all — it authenticates with a service-account bearer API key, and authorization is expressed through RBAC policies rather than scopes (see authentication/groundcover-authentication.yml). No scopes/permissions reference page exists in the docs; this file records what the server itself publishes.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Groundcover Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Groundcover uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Groundcover
provider_slug: groundcover
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: groundcover-scopes
source_filename: groundcover-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://mcp.groundcover.com/.well-known/oauth-protected-resource\nprovider: Groundcover\nproviderId: groundcover\ndescription: >-\n  groundcover's only published OAuth surface is the remote MCP server. Its RFC 9728 Protected\n  Resource Metadata declares exactly one scope. The REST API at api.groundcover.com does not use\n  OAuth at all — it authenticates with a service-account bearer API key, and authorization is\n  expressed through RBAC policies rather than scopes (see authentication/groundcover-authentication.yml).\n  No scopes/permissions reference page exists in the docs; this file records what the server itself\n  publishes.\nresource: https://mcp.groundcover.com/api/mcp\nauthorization_servers:\n  - https://mcp.groundcover.com\nbearer_methods_supported:\n  - header\nscopes:\n  - name: access:router\n    description: >-\n      The single scope advertised by groundcover's MCP protected-resource metadata. Grants an\n    \
  \  OAuth-authenticated agent access to the MCP router endpoint; groundcover publishes no\n      per-tool or per-signal scope breakdown, so the effective permission is the one the logged-in\n      member already holds under RBAC.\n    source: https://mcp.groundcover.com/.well-known/oauth-protected-resource\n    http_status: 200\n    probed: '2026-08-29'\nscope_count: 1\nx-evidence:\n  - url: https://mcp.groundcover.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://mcp.groundcover.com/.well-known/oauth-authorization-server\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groundcover/refs/heads/main/scopes/groundcover-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AIOps
- Observability
- Kubernetes
- eBPF
- Monitoring
- Logs
- Traces
- Metrics
- OpenTelemetry
- MCP
token_urls: []
---
