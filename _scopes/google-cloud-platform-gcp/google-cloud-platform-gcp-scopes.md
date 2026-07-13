---
api_specs:
- filename: rest
  format: yaml
  label: Compute Engine API
  slug: compute-engine-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/compute/v1/rest
- filename: rest
  format: yaml
  label: Cloud Storage API
  slug: cloud-storage-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/storage/v1/rest
- filename: rest
  format: yaml
  label: BigQuery API
  slug: bigquery-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/bigquery/v2/rest
- filename: rest
  format: yaml
  label: Cloud Functions API
  slug: cloud-functions-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/cloudfunctions/v2/rest
- filename: rest
  format: yaml
  label: Kubernetes Engine API
  slug: kubernetes-engine-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/container/v1/rest
- filename: rest
  format: yaml
  label: Cloud Pub/Sub API
  slug: cloud-pubsub-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/pubsub/v1/rest
- filename: rest
  format: yaml
  label: Cloud Vision API
  slug: cloud-vision-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/vision/v1/rest
- filename: rest
  format: yaml
  label: Cloud SQL Admin API
  slug: cloud-sql-admin-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/sqladmin/v1/rest
- filename: rest
  format: yaml
  label: Cloud Run API
  slug: cloud-run-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/run/v2/rest
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Platform Gcp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Platform publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Platform API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform-gcp
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-cloud-platform-gcp-openapi.yml
scope_count: 2
scope_names:
- cloud-platform
- compute
scopes:
- description: View and manage your data across Google Cloud Platform services
  flows:
  - authorizationCode
  scope: cloud-platform
- description: View and manage your Google Compute Engine resources
  flows:
  - authorizationCode
  scope: compute
slug: google-cloud-platform-gcp-scopes
source_filename: google-cloud-platform-gcp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-platform-gcp-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-cloud-platform-gcp-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: cloud-platform\n  description: View and manage your data across Google Cloud Platform services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-platform-gcp-openapi.yml\n- scope: compute\n  description: View and manage your Google Compute Engine resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-platform-gcp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform-gcp/refs/heads/main/scopes/google-cloud-platform-gcp-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Cloud Computing
- Data Analytics
- IaaS
- Machine Learning
- PaaS
- SaaS
- Serverless
token_urls:
- https://oauth2.googleapis.com/token
---
