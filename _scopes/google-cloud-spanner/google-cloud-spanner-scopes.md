---
api_specs:
- filename: cloud-spanner-openapi.yml
  format: yaml
  label: Cloud Spanner API
  slug: cloud-spanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-spanner/refs/heads/main/openapi/cloud-spanner-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Spanner Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Spanner publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Spanner API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Spanner
provider_slug: google-cloud-spanner
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/cloud-spanner-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/spanner.admin
- https://www.googleapis.com/auth/spanner.data
scopes:
- description: Full access to Cloud Platform
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: Administer Spanner databases
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/spanner.admin
- description: View and manage Spanner data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/spanner.data
slug: google-cloud-spanner-scopes
source_filename: google-cloud-spanner-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-spanner-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cloud-spanner-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Cloud Platform\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-spanner-openapi.yml\n- scope: https://www.googleapis.com/auth/spanner.admin\n  description: Administer Spanner databases\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-spanner-openapi.yml\n- scope: https://www.googleapis.com/auth/spanner.data\n  description: View and manage Spanner data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-spanner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-spanner/refs/heads/main/scopes/google-cloud-spanner-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Database
- Distributed
- Google Cloud
- Relational
- SQL
token_urls:
- https://oauth2.googleapis.com/token
---
