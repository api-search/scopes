---
api_specs:
- filename: dash0-openapi.json
  format: json
  label: Dash0 API
  slug: dash0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dash0/refs/heads/main/openapi/dash0-openapi.json
authorization_urls: []
description: ''
docs: https://api-docs.dash0.com/reference/get_well-known-oauth-authorization-server
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Dash0 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dash0 publishes 1 OAuth 2.0 scope via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dash0 API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dash0
provider_slug: dash0
schemes:
- authorizationUrl: https://api.<region>.aws.dash0.com/oauth/authorize
  flows:
  - authorizationCode
  - refreshToken
  name: OAuth2
  tokenUrl: https://api.<region>.aws.dash0.com/oauth/token
scope_count: 1
scope_names:
- '*'
scopes:
- description: 'Full-access wildcard scope. Dash0''s OAuth Authorization Server Metadata advertises `scopes_supported: ["*"]` — a single wildcard scope rather than a granular per-resource scope catalog. Fine-grained access is instead governed by organization roles/RBAC and dataset scoping (the `dataset` query parameter), not by OAuth scopes.'
  flows:
  - authorizationCode
  scope: '*'
slug: dash0-scopes
source_filename: dash0-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.eu-west-1.aws.dash0.com/.well-known/oauth-authorization-server\ndocs: https://api-docs.dash0.com/reference/get_well-known-oauth-authorization-server\nschemes:\n- name: OAuth2\n  authorizationUrl: https://api.<region>.aws.dash0.com/oauth/authorize\n  tokenUrl: https://api.<region>.aws.dash0.com/oauth/token\n  flows: [authorizationCode, refreshToken]\nscopes:\n- scope: '*'\n  description: >-\n    Full-access wildcard scope. Dash0's OAuth Authorization Server Metadata\n    advertises `scopes_supported: [\"*\"]` — a single wildcard scope rather than a\n    granular per-resource scope catalog. Fine-grained access is instead governed\n    by organization roles/RBAC and dataset scoping (the `dataset` query\n    parameter), not by OAuth scopes.\n  flows: [authorizationCode]\nnotes: >-\n  Bearer auth-token requests (the primary API auth) are not scoped via OAuth;\n  they carry organization-level access. This artifact reflects\
  \ the OAuth surface\n  used by the CLI and MCP clients.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dash0/refs/heads/main/scopes/dash0-scopes.yml
summary_line: 1 scope · authorizationCode/refreshToken
tags:
- Observability
- OpenTelemetry
- Monitoring
- Logs
- Metrics
- Tracing
- APM
- Prometheus
- DevOps
- Company
- Apis
token_urls: []
---
