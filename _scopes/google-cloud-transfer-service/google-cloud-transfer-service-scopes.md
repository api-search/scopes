---
api_specs:
- filename: storage-transfer-api-openapi.yml
  format: yaml
  label: Storage Transfer API
  slug: storage-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-transfer-service/refs/heads/main/openapi/storage-transfer-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Transfer Service Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Transfer Service publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Transfer Service API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Transfer Service
provider_slug: google-cloud-transfer-service
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/storage-transfer-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: Full access to Google Cloud resources
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-cloud-transfer-service-scopes
source_filename: google-cloud-transfer-service-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/storage-transfer-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/storage-transfer-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Google Cloud resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/storage-transfer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-transfer-service/refs/heads/main/scopes/google-cloud-transfer-service-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Azure
- Cloud Storage
- Data Transfer
- Migration
- S3
- Storage
token_urls:
- https://oauth2.googleapis.com/token
---
