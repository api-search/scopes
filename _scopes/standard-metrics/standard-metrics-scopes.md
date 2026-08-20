---
api_specs:
- filename: standard-metrics-budgets-api-openapi.yml
  format: yaml
  label: Standard Metrics budgets API
  slug: standard-metrics-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-budgets-api-openapi.yml
- filename: standard-metrics-cap-table-api-openapi.yml
  format: yaml
  label: Standard Metrics cap_table API
  slug: standard-metrics-cap-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-cap-table-api-openapi.yml
- filename: standard-metrics-companies-api-openapi.yml
  format: yaml
  label: Standard Metrics companies API
  slug: standard-metrics-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-companies-api-openapi.yml
- filename: standard-metrics-custom-columns-api-openapi.yml
  format: yaml
  label: Standard Metrics custom-columns API
  slug: standard-metrics-custom-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-custom-columns-api-openapi.yml
- filename: standard-metrics-documents-api-openapi.yml
  format: yaml
  label: Standard Metrics documents API
  slug: standard-metrics-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-documents-api-openapi.yml
- filename: standard-metrics-firm-details-api-openapi.yml
  format: yaml
  label: Standard Metrics firm-details API
  slug: standard-metrics-firm-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-firm-details-api-openapi.yml
- filename: standard-metrics-funds-api-openapi.yml
  format: yaml
  label: Standard Metrics funds API
  slug: standard-metrics-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-funds-api-openapi.yml
- filename: standard-metrics-information-reports-api-openapi.yml
  format: yaml
  label: Standard Metrics information-reports API
  slug: standard-metrics-information-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-information-reports-api-openapi.yml
- filename: standard-metrics-information-requests-api-openapi.yml
  format: yaml
  label: Standard Metrics information-requests API
  slug: standard-metrics-information-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-information-requests-api-openapi.yml
- filename: standard-metrics-metrics-api-openapi.yml
  format: yaml
  label: Standard Metrics metrics API
  slug: standard-metrics-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-metrics-api-openapi.yml
- filename: standard-metrics-notes-api-openapi.yml
  format: yaml
  label: Standard Metrics notes API
  slug: standard-metrics-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-notes-api-openapi.yml
- filename: standard-metrics-o-api-openapi.yml
  format: yaml
  label: Standard Metrics O API
  slug: standard-metrics-o-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-o-api-openapi.yml
- filename: standard-metrics-users-api-openapi.yml
  format: yaml
  label: Standard Metrics users API
  slug: standard-metrics-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-users-api-openapi.yml
- filename: standard-metrics-whoami-api-openapi.yml
  format: yaml
  label: Standard Metrics whoami API
  slug: standard-metrics-whoami-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-metrics/refs/heads/main/openapi/standard-metrics-whoami-api-openapi.yml
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
- Portfolio-Management
- Financial Data
- Investment Data
- Cap Table
- Metrics
- Reporting
- MCP
token_urls: []
---
