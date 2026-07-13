---
api_specs:
- filename: google-cloud-dataflow-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow API
  slug: google-cloud-dataflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Dataflow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Dataflow publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Dataflow API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
schemes:
- description: OAuth 2.0 authentication for Google Cloud APIs.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-dataflow-api-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/compute
- https://www.googleapis.com/auth/compute.readonly
scopes:
- description: Full access to all Google Cloud resources.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View and manage Google Compute Engine resources.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/compute
- description: View Google Compute Engine resources.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/compute.readonly
slug: google-cloud-dataflow-scopes
source_filename: google-cloud-dataflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-dataflow-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-dataflow-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for Google Cloud APIs.\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to all Google Cloud resources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-dataflow-api-openapi.yml\n- scope: https://www.googleapis.com/auth/compute\n  description: View and manage Google Compute Engine resources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-dataflow-api-openapi.yml\n- scope: https://www.googleapis.com/auth/compute.readonly\n  description: View Google Compute Engine resources.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/google-cloud-dataflow-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/scopes/google-cloud-dataflow-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
token_urls:
- https://oauth2.googleapis.com/token
---
