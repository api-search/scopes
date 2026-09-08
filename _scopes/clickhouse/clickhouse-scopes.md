---
api_specs:
- filename: clickhouse-clickhouse-http-interface-api-openapi.yml
  format: yaml
  label: ClickHouse ClickHouse HTTP Interface API
  slug: clickhouse-clickhouse-http-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-clickhouse-http-interface-api-openapi.yml
- filename: clickhouse-ping-api-openapi.yml
  format: yaml
  label: ClickHouse Ping API
  slug: clickhouse-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-ping-api-openapi.yml
- filename: clickhouse-play-api-openapi.yml
  format: yaml
  label: ClickHouse Play API
  slug: clickhouse-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-play-api-openapi.yml
- filename: clickhouse-replicas-status-api-openapi.yml
  format: yaml
  label: ClickHouse Replicas Status API
  slug: clickhouse-replicas-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-replicas-status-api-openapi.yml
- filename: clickhouse-cloud-api-openapi.json
  format: json
  label: ClickHouse Cloud API
  slug: clickhouse-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-cloud-api-openapi.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Clickhouse Scopes
name_suffix: OAuth Scopes
note: The ClickHouse Cloud REST API at api.clickhouse.cloud does NOT use OAuth — it declares a single securityScheme, HTTP Basic with an API key ID and secret, and therefore has no scopes. The only OAuth surface ClickHouse publishes is the remote MCP server, and the scopes below are read straight from its RFC 8414 / RFC 9728 discovery documents. Permissions on the REST API are expressed as key ROLES (developer / admin) rather than scopes; those are recorded here too because they are the closest equivalent a caller has to reason about.
overview: 'ClickHouse uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClickHouse
provider_slug: clickhouse
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: clickhouse-scopes
source_filename: clickhouse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: OAuth Scopes\nspecificationVersion: '0.1'\nprovider: ClickHouse\nproviderId: clickhouse\ngenerated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://mcp.clickhouse.cloud/.well-known/oauth-authorization-server and\n  https://mcp.clickhouse.cloud/.well-known/oauth-protected-resource (+ the per-resource variant\n  /.well-known/oauth-protected-resource/mcp), all fetched anonymously on 2026-09-05 with HTTP 200\nnote: >-\n  The ClickHouse Cloud REST API at api.clickhouse.cloud does NOT use OAuth — it declares a single\n  securityScheme, HTTP Basic with an API key ID and secret, and therefore has no scopes. The only OAuth\n  surface ClickHouse publishes is the remote MCP server, and the scopes below are read straight from its\n  RFC 8414 / RFC 9728 discovery documents. Permissions on the REST API are expressed as key ROLES\n  (developer / admin) rather than scopes; those are recorded here too because they are the closest\n  equivalent a caller has to reason about.\n\
  oauth:\n  applies_to: https://mcp.clickhouse.cloud/mcp\n  issuer: https://mcp.clickhouse.cloud\n  authorization_endpoint: https://mcp.clickhouse.cloud/authorize\n  token_endpoint: https://mcp.clickhouse.cloud/token\n  registration_endpoint: https://mcp.clickhouse.cloud/register\n  grant_types_supported:\n    - authorization_code\n    - refresh_token\n  response_types_supported:\n    - code\n  code_challenge_methods_supported:\n    - S256\n  token_endpoint_auth_methods_supported:\n    - none\n  docs: https://clickhouse.com/docs/cloud/features/ai-ml/remote-mcp\nscope_count: 5\nscopes:\n  - name: 'mcp:access'\n    description: Access the ClickHouse Cloud remote MCP server and its read-only tools\n    resource: https://mcp.clickhouse.cloud/mcp\n  - name: 'clickstack:access'\n    description: Access ClickStack observability resources through the MCP server\n    resource: https://mcp.clickhouse.cloud\n  - name: openid\n    description: Standard OpenID Connect scope — issue an ID token for the\
  \ authenticated ClickHouse Cloud user\n  - name: profile\n    description: Standard OIDC scope — basic profile claims\n  - name: email\n    description: Standard OIDC scope — email claim\nrest_api_permissions:\n  model: role-per-key (not scopes)\n  scheme: basicAuth (HTTP Basic — key ID as username, key secret as password)\n  roles:\n    - name: developer\n      grants: read-only permissions for assigned services\n    - name: admin\n      grants: full read and write permissions\n  additional_controls:\n    - Per-key expiration\n    - Per-key IP allowlist (single IP or CIDR)\n    - Query API Endpoints require Organization Role `Member` (minimum) plus Service Role access to `Query Endpoints`\n  docs: https://clickhouse.com/docs/cloud/manage/openapi\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/scopes/clickhouse-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Cloud Database
- Column-Oriented
- Database
- OLAP
- Open-Source
- Real-Time
- SQL
token_urls: []
---
