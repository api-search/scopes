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
name: Google Cloud Sql Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud SQL publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud SQL API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud SQL
provider_slug: google-cloud-sql
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/cloud-sql-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/sqlservice.admin
scopes:
- description: Full access to Cloud Platform
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: Manage Cloud SQL instances
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/sqlservice.admin
slug: google-cloud-sql-scopes
source_filename: google-cloud-sql-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-sql-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cloud-sql-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Cloud Platform\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-sql-openapi.yml\n- scope: https://www.googleapis.com/auth/sqlservice.admin\n  description: Manage Cloud SQL instances\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-sql-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-sql/refs/heads/main/scopes/google-cloud-sql-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Database
- Google Cloud
- MySQL
- PostgreSQL
- Relational
- SQL
token_urls:
- https://oauth2.googleapis.com/token
---
