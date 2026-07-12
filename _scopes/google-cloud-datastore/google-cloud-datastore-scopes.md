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
name: Google Cloud Datastore Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Datastore publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Datastore API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Datastore
provider_slug: google-cloud-datastore
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-cloud-datastore-openapi.yml
scope_count: 2
scope_names:
- cloud-platform
- datastore
scopes:
- description: View and manage your data across Google Cloud Platform services
  flows:
  - authorizationCode
  scope: cloud-platform
- description: View and manage your Google Cloud Datastore data
  flows:
  - authorizationCode
  scope: datastore
slug: google-cloud-datastore-scopes
source_filename: google-cloud-datastore-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-datastore-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-cloud-datastore-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: cloud-platform\n  description: View and manage your data across Google Cloud Platform services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-datastore-openapi.yml\n- scope: datastore\n  description: View and manage your Google Cloud Datastore data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-datastore-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-datastore/refs/heads/main/scopes/google-cloud-datastore-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- NoSQL
- Database
- Document Database
- Google Cloud
- Firestore
- Managed Service
- Key-Value Store
token_urls:
- https://oauth2.googleapis.com/token
---
