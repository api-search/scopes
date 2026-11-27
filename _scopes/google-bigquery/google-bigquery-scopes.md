---
api_specs:
- filename: google-bigquery-analyticshub-organizations-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Analyticshub Organizations API
  slug: google-bigquery-analyticshub-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-analyticshub-organizations-api-openapi.yml
- filename: google-bigquery-analyticshub-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Analyticshub Projects API
  slug: google-bigquery-analyticshub-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-analyticshub-projects-api-openapi.yml
- filename: google-bigquery-bigquery-datasets-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Datasets API
  slug: google-bigquery-bigquery-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-datasets-api-openapi.yml
- filename: google-bigquery-bigquery-jobs-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Jobs API
  slug: google-bigquery-bigquery-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-jobs-api-openapi.yml
- filename: google-bigquery-bigquery-models-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Models API
  slug: google-bigquery-bigquery-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-models-api-openapi.yml
- filename: google-bigquery-bigquery-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Projects API
  slug: google-bigquery-bigquery-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-projects-api-openapi.yml
- filename: google-bigquery-bigquery-routines-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Routines API
  slug: google-bigquery-bigquery-routines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-routines-api-openapi.yml
- filename: google-bigquery-bigquery-row-access-policies-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Row Access Policies API
  slug: google-bigquery-bigquery-row-access-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-row-access-policies-api-openapi.yml
- filename: google-bigquery-bigquery-tabledata-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Tabledata API
  slug: google-bigquery-bigquery-tabledata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-tabledata-api-openapi.yml
- filename: google-bigquery-bigquery-tables-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Tables API
  slug: google-bigquery-bigquery-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-tables-api-openapi.yml
- filename: google-bigquery-bigqueryconnection-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigqueryconnection Projects API
  slug: google-bigquery-bigqueryconnection-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigqueryconnection-projects-api-openapi.yml
- filename: google-bigquery-bigquerydatapolicy-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquerydatapolicy Projects API
  slug: google-bigquery-bigquerydatapolicy-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquerydatapolicy-projects-api-openapi.yml
- filename: google-bigquery-bigquerydatatransfer-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquerydatatransfer Projects API
  slug: google-bigquery-bigquerydatatransfer-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquerydatatransfer-projects-api-openapi.yml
- filename: google-bigquery-bigqueryreservation-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigqueryreservation Projects API
  slug: google-bigquery-bigqueryreservation-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigqueryreservation-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google BigQuery Scopes
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
source_yaml_url: https://artifacts.apis.io/google-bigquery/scopes/google-bigquery-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Analytics
- Big Data
- Cloud
- Data Warehouse
- Serverless
- SQL
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
