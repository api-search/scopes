---
api_specs:
- filename: bigquery-api-openapi.yml
  format: yaml
  label: BigQuery API
  slug: bigquery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-bigquery/refs/heads/main/openapi/bigquery-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Bigquery Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google BigQuery publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google BigQuery API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google BigQuery
provider_slug: google-bigquery
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/bigquery-api-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/bigquery
- https://www.googleapis.com/auth/bigquery.readonly
scopes:
- description: Full access to BigQuery
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/bigquery
- description: Read-only access to BigQuery
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/bigquery.readonly
slug: google-bigquery-scopes
source_filename: google-bigquery-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bigquery-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/bigquery-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/bigquery\n  description: Full access to BigQuery\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bigquery-api-openapi.yml\n- scope: https://www.googleapis.com/auth/bigquery.readonly\n  description: Read-only access to BigQuery\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bigquery-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-bigquery/refs/heads/main/scopes/google-bigquery-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Analytics
- Big Data
- Cloud
- Data Warehouse
- Serverless
- SQL
token_urls:
- https://oauth2.googleapis.com/token
---
