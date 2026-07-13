---
api_specs:
- filename: cloud-bigtable-openapi.yml
  format: yaml
  label: Cloud Bigtable Admin API
  slug: cloud-bigtable-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-bigtable/refs/heads/main/openapi/cloud-bigtable-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Bigtable Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Bigtable publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Bigtable API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Bigtable
provider_slug: google-cloud-bigtable
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/cloud-bigtable-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/bigtable.admin
- https://www.googleapis.com/auth/bigtable.admin.table
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: Administer Bigtable instances and tables
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/bigtable.admin
- description: Administer Bigtable tables
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/bigtable.admin.table
- description: Full access to Cloud Platform
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-cloud-bigtable-scopes
source_filename: google-cloud-bigtable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-bigtable-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cloud-bigtable-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/bigtable.admin\n  description: Administer Bigtable instances and tables\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-bigtable-openapi.yml\n- scope: https://www.googleapis.com/auth/bigtable.admin.table\n  description: Administer Bigtable tables\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-bigtable-openapi.yml\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Cloud Platform\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-bigtable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-bigtable/refs/heads/main/scopes/google-cloud-bigtable-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Bigtable
- Database
- Google Cloud
- NoSQL
- Wide Column
token_urls:
- https://oauth2.googleapis.com/token
---
