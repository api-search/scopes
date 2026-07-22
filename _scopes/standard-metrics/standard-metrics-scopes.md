---
api_specs:
- filename: standard-metrics-main-openapi.json
  format: json
  label: Standard Metrics API
  slug: standard-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-main-openapi.json
- filename: standard-metrics-investment-data-openapi.json
  format: json
  label: Standard Metrics Investment Data API
  slug: standard-metrics-investment-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-investment-data-openapi.json
authorization_urls: []
description: Standard Metrics uses OAuth2 client-credentials. A client_id/client_secret pair (created per OAuth application in Developer Settings) is exchanged at the token endpoint for a Bearer access token. The token response returns a coarse-grained scope string; per-user data access is additionally governed by API-key permissions set by firm admins, not by fine-grained OAuth scopes.
docs: https://docs.standardmetrics.io/api-reference/get-oauth-access-token
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Standard Metrics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Standard Metrics publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Standard Metrics API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Standard Metrics
provider_slug: standard-metrics
schemes:
- flow: clientCredentials
  name: OAuth2 Client Credentials
  tokenUrl: https://api.standardmetrics.io/o/token/
scope_count: 3
scope_names:
- read
- write
- all
scopes:
- description: Read access to firm portfolio, metric, and investment data.
  flows: []
  scope: read
- description: Write access (create/update metrics, companies, documents, notes, cap-table data).
  flows: []
  scope: write
- description: Full read and write access (observed in token responses as "all read write").
  flows: []
  scope: all
slug: standard-metrics-scopes
source_filename: standard-metrics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.standardmetrics.io/api-reference/setting-up\ndocs: https://docs.standardmetrics.io/api-reference/get-oauth-access-token\ndescription: >-\n  Standard Metrics uses OAuth2 client-credentials. A client_id/client_secret pair\n  (created per OAuth application in Developer Settings) is exchanged at the token\n  endpoint for a Bearer access token. The token response returns a coarse-grained\n  scope string; per-user data access is additionally governed by API-key permissions\n  set by firm admins, not by fine-grained OAuth scopes.\ntoken_endpoint: https://api.standardmetrics.io/o/token/\ngrant_type: client_credentials\nschemes:\n- name: OAuth2 Client Credentials\n  flow: clientCredentials\n  tokenUrl: https://api.standardmetrics.io/o/token/\nscopes:\n- scope: read\n  description: Read access to firm portfolio, metric, and investment data.\n- scope: write\n  description: Write access (create/update metrics, companies, documents,\
  \ notes, cap-table data).\n- scope: all\n  description: Full read and write access (observed in token responses as \"all read write\").\npermissions_note: >-\n  Admins can define specific user permissions for each API key. See\n  https://intercom.help/standardmetrics/en/articles/10088424-permissions-for-api-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/scopes/standard-metrics-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Venture Capital
- Private Equity
- Portfolio Management
- Financial Data
- Investment Data
- Cap Table
- Metrics
- Reporting
- MCP
token_urls: []
---
