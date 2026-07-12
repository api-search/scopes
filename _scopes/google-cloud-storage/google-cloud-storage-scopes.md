---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Storage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Storage publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Storage API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Storage
provider_slug: google-cloud-storage
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/cloud-storage-openapi.yml
scope_count: 4
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/devstorage.full_control
- https://www.googleapis.com/auth/devstorage.read_only
- https://www.googleapis.com/auth/devstorage.read_write
scopes:
- description: Full access to Cloud Platform
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: Full control of Cloud Storage
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/devstorage.full_control
- description: Read-only access to Cloud Storage
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/devstorage.read_only
- description: Read-write access to Cloud Storage
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/devstorage.read_write
slug: google-cloud-storage-scopes
source_filename: google-cloud-storage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-storage-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cloud-storage-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Cloud Platform\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-storage-openapi.yml\n- scope: https://www.googleapis.com/auth/devstorage.full_control\n  description: Full control of Cloud Storage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-storage-openapi.yml\n- scope: https://www.googleapis.com/auth/devstorage.read_only\n  description: Read-only access to Cloud Storage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-storage-openapi.yml\n- scope: https://www.googleapis.com/auth/devstorage.read_write\n  description: Read-write\
  \ access to Cloud Storage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-storage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-storage/refs/heads/main/scopes/google-cloud-storage-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Buckets
- Cloud
- Google Cloud
- Objects
- Storage
token_urls:
- https://oauth2.googleapis.com/token
---
