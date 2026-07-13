---
api_specs:
- filename: rest
  format: yaml
  label: Compute Engine API
  slug: compute-engine
  spec_type: OpenAPI
  url: https://compute.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Storage API
  slug: cloud-storage
  spec_type: OpenAPI
  url: https://storage.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Functions API
  slug: cloud-functions
  spec_type: OpenAPI
  url: https://cloudfunctions.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Pub/Sub API
  slug: cloud-pubsub
  spec_type: OpenAPI
  url: https://pubsub.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: BigQuery API
  slug: bigquery
  spec_type: OpenAPI
  url: https://bigquery.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Cloud Vision API
  slug: cloud-vision
  spec_type: OpenAPI
  url: https://vision.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Natural Language API
  slug: cloud-natural-language
  spec_type: OpenAPI
  url: https://language.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Kubernetes Engine API
  slug: kubernetes-engine
  spec_type: OpenAPI
  url: https://container.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud SQL Admin API
  slug: cloud-sql
  spec_type: OpenAPI
  url: https://sqladmin.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Firestore API
  slug: cloud-firestore
  spec_type: OpenAPI
  url: https://firestore.googleapis.com/$discovery/rest?version=v1
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Gcp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Platform APIs publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Platform APIs API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Platform APIs
provider_slug: gcp
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/gcp-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/compute
scopes:
- description: View and manage all Google Cloud resources
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: Manage Compute Engine resources
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/compute
slug: gcp-scopes
source_filename: gcp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gcp-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/gcp-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: View and manage all Google Cloud resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gcp-openapi.yml\n- scope: https://www.googleapis.com/auth/compute\n  description: Manage Compute Engine resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gcp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/scopes/gcp-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Security
- Serverless
- Storage
token_urls:
- https://oauth2.googleapis.com/token
---
