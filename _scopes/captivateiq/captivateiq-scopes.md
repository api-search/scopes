---
api_specs:
- filename: captivateiq-attribute-worksheets-api-openapi.yml
  format: yaml
  label: CaptivateIQ Attribute Worksheets API
  slug: captivateiq-attribute-worksheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-attribute-worksheets-api-openapi.yml
- filename: captivateiq-audit-logs-api-openapi.yml
  format: yaml
  label: CaptivateIQ Audit Logs API
  slug: captivateiq-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-audit-logs-api-openapi.yml
- filename: captivateiq-commission-plans-api-openapi.yml
  format: yaml
  label: CaptivateIQ Commission Plans API
  slug: captivateiq-commission-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-commission-plans-api-openapi.yml
- filename: captivateiq-dashboards-api-openapi.yml
  format: yaml
  label: CaptivateIQ Dashboards API
  slug: captivateiq-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-dashboards-api-openapi.yml
- filename: captivateiq-data-workbooks-api-openapi.yml
  format: yaml
  label: CaptivateIQ Data Workbooks API
  slug: captivateiq-data-workbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-data-workbooks-api-openapi.yml
- filename: captivateiq-data-worksheets-api-openapi.yml
  format: yaml
  label: CaptivateIQ Data Worksheets API
  slug: captivateiq-data-worksheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-data-worksheets-api-openapi.yml
- filename: captivateiq-employee-assumptions-api-openapi.yml
  format: yaml
  label: CaptivateIQ Employee Assumptions API
  slug: captivateiq-employee-assumptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-employee-assumptions-api-openapi.yml
- filename: captivateiq-employees-api-openapi.yml
  format: yaml
  label: CaptivateIQ Employees API
  slug: captivateiq-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-employees-api-openapi.yml
- filename: captivateiq-hierarchies-api-openapi.yml
  format: yaml
  label: CaptivateIQ Hierarchies API
  slug: captivateiq-hierarchies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-hierarchies-api-openapi.yml
- filename: captivateiq-jobs-api-openapi.yml
  format: yaml
  label: CaptivateIQ Jobs API
  slug: captivateiq-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-jobs-api-openapi.yml
- filename: captivateiq-metadata-api-openapi.yml
  format: yaml
  label: CaptivateIQ Metadata API
  slug: captivateiq-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-metadata-api-openapi.yml
- filename: captivateiq-payouts-api-openapi.yml
  format: yaml
  label: CaptivateIQ Payouts API
  slug: captivateiq-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-payouts-api-openapi.yml
- filename: captivateiq-report-models-api-openapi.yml
  format: yaml
  label: CaptivateIQ Report Models API
  slug: captivateiq-report-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-report-models-api-openapi.yml
- filename: captivateiq-transformation-worksheets-api-openapi.yml
  format: yaml
  label: CaptivateIQ Transformation Worksheets API
  slug: captivateiq-transformation-worksheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-transformation-worksheets-api-openapi.yml
- filename: captivateiq-uploads-api-openapi.yml
  format: yaml
  label: CaptivateIQ Uploads API
  slug: captivateiq-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-uploads-api-openapi.yml
- filename: captivateiq-users-api-openapi.yml
  format: yaml
  label: CaptivateIQ Users API
  slug: captivateiq-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-users-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Captivateiq Scopes
name_suffix: OAuth Scopes
note: 'These scopes were read from CaptivateIQ''s own RFC 8414 authorization-server metadata document (HTTP 200, application/json), NOT from the OpenAPI and NOT from the docs. The public developer reference documents only static token auth ("Authorization: Token <value>") and never mentions OAuth, so there is no scopes/permissions reference page to enrich this from — the OAuth surface is served but undocumented. The server advertises exactly one scope, `read`, which means the OAuth path as published is read-only and cannot authorize any of the write operations (create/update/delete/batch/import) in the ciq/v1 OpenAPI; those require a static API token. Do not infer additional scopes: the metadata document names one.'
overview: 'CaptivateIQ uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CaptivateIQ
provider_slug: captivateiq
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: captivateiq-scopes
source_filename: captivateiq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.captivateiq.com/.well-known/oauth-authorization-server\ndocs: null\nverbatim: well-known/captivateiq-oauth-authorization-server.json\nnote: >-\n  These scopes were read from CaptivateIQ's own RFC 8414 authorization-server metadata document\n  (HTTP 200, application/json), NOT from the OpenAPI and NOT from the docs. The public developer\n  reference documents only static token auth (\"Authorization: Token <value>\") and never mentions\n  OAuth, so there is no scopes/permissions reference page to enrich this from — the OAuth surface\n  is served but undocumented. The server advertises exactly one scope, `read`, which means the\n  OAuth path as published is read-only and cannot authorize any of the write operations\n  (create/update/delete/batch/import) in the ciq/v1 OpenAPI; those require a static API token.\n  Do not infer additional scopes: the metadata document names one.\nissuer: https://app.captivateiq.com\nauthorization_endpoint:\
  \ https://app.captivateiq.com/o/authorize/\ntoken_endpoint: https://app.captivateiq.com/o/token/\nrevocation_endpoint: https://app.captivateiq.com/o/revoke_token/\nintrospection_endpoint: https://app.captivateiq.com/o/introspect/\ngrant_types_supported:\n- authorization_code\n- refresh_token\nresponse_types_supported:\n- code\ncode_challenge_methods_supported:\n- S256\ntoken_endpoint_auth_methods_supported:\n- none\n- client_secret_post\n- client_secret_basic\nclient_id_metadata_document_supported: true\nscope_count: 1\nscopes:\n- name: read\n  description: >-\n    The only scope advertised in scopes_supported. Description is not published by the\n    provider; no scope reference page exists.\n  source: scopes_supported in the RFC 8414 metadata document\n  documented_by_provider: false\ngaps:\n- No write scope is advertised, so OAuth clients cannot perform ciq/v1 write operations.\n- No scope-to-operation mapping is published; the OpenAPI declares only the apiKey scheme.\n- No /.well-known/openid-configuration\
  \ and no jwks.json (404) — OAuth 2.0 only, not OIDC.\nevidence:\n- url: https://app.captivateiq.com/.well-known/oauth-authorization-server\n  status: 200\n- url: https://app.captivateiq.com/.well-known/openid-configuration\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/scopes/captivateiq-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cloud Saas
- Sales Commissions
- Incentive Compensation Management
- Sales Performance Management
- Revenue Operations
- Finance
- Payouts
- Commission Plans
- Sales Compensation
token_urls: []
---
