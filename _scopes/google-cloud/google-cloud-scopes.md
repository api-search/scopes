---
api_specs:
- filename: rest
  format: yaml
  label: Google Compute Engine API
  slug: google-compute-engine-api
  spec_type: OpenAPI
  url: https://compute.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud Storage API
  slug: google-cloud-storage-api
  spec_type: OpenAPI
  url: https://storage.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Kubernetes Engine API
  slug: google-kubernetes-engine-api
  spec_type: OpenAPI
  url: https://container.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud Functions API
  slug: google-cloud-functions-api
  spec_type: OpenAPI
  url: https://cloudfunctions.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google BigQuery API
  slug: google-bigquery-api
  spec_type: OpenAPI
  url: https://bigquery.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Google Cloud Pub/Sub API
  slug: google-cloud-pubsub-api
  spec_type: OpenAPI
  url: https://pubsub.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud Vision API
  slug: google-cloud-vision-api
  spec_type: OpenAPI
  url: https://vision.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud SQL Admin API
  slug: google-cloud-sql-admin-api
  spec_type: OpenAPI
  url: https://sqladmin.googleapis.com/$discovery/rest?version=v1
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Platform publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Platform API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Platform
provider_slug: google-cloud
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-cloud-openapi.yml
scope_count: 3
scope_names:
- cloud-platform
- compute
- compute.readonly
scopes:
- description: View and manage your data across Google Cloud Platform services
  flows:
  - authorizationCode
  scope: cloud-platform
- description: View and manage your Google Compute Engine resources
  flows:
  - authorizationCode
  scope: compute
- description: View your Google Compute Engine resources
  flows:
  - authorizationCode
  scope: compute.readonly
slug: google-cloud-scopes
source_filename: google-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-cloud-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: cloud-platform\n  description: View and manage your data across Google Cloud Platform services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-openapi.yml\n- scope: compute\n  description: View and manage your Google Compute Engine resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-openapi.yml\n- scope: compute.readonly\n  description: View your Google Compute Engine resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud/refs/heads/main/scopes/google-cloud-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Cloud Computing
- Data Analytics
- Infrastructure
- Machine Learning
- Platform as a Service
token_urls:
- https://oauth2.googleapis.com/token
---
