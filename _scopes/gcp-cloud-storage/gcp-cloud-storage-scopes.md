---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Gcp Cloud Storage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Storage publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Storage API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
schemes:
- description: OAuth 2.0 authentication for Google Cloud APIs
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/gcp-cloud-storage-json-api-openapi.yml
scope_count: 5
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/cloud-platform.read-only
- https://www.googleapis.com/auth/devstorage.full_control
- https://www.googleapis.com/auth/devstorage.read_only
- https://www.googleapis.com/auth/devstorage.read_write
scopes:
- description: View and manage your data across Google Cloud services
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View your data across Google Cloud services
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform.read-only
- description: Full control of Cloud Storage resources
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/devstorage.full_control
- description: View your data in Cloud Storage
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/devstorage.read_only
- description: Manage your data in Cloud Storage
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/devstorage.read_write
slug: gcp-cloud-storage-scopes
source_filename: gcp-cloud-storage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gcp-cloud-storage-json-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/gcp-cloud-storage-json-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for Google Cloud APIs\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: View and manage your data across Google Cloud services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gcp-cloud-storage-json-api-openapi.yml\n- scope: https://www.googleapis.com/auth/cloud-platform.read-only\n  description: View your data across Google Cloud services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gcp-cloud-storage-json-api-openapi.yml\n- scope: https://www.googleapis.com/auth/devstorage.full_control\n  description: Full control of Cloud Storage resources\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/gcp-cloud-storage-json-api-openapi.yml\n- scope: https://www.googleapis.com/auth/devstorage.read_only\n  description: View your data in Cloud Storage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gcp-cloud-storage-json-api-openapi.yml\n- scope: https://www.googleapis.com/auth/devstorage.read_write\n  description: Manage your data in Cloud Storage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gcp-cloud-storage-json-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/scopes/gcp-cloud-storage-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Archival
- Backup
- Blob Storage
- Cloud Storage
- Data
- File Storage
- Google Cloud
- Object Storage
- Storage
token_urls:
- https://oauth2.googleapis.com/token
---
