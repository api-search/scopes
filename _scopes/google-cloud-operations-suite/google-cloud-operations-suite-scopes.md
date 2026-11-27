---
api_specs:
- filename: google-cloud-operations-suite-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Operations Suite Projects API
  slug: google-cloud-operations-suite-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-operations-suite/openapi/google-cloud-operations-suite-projects-api-openapi.yml
- filename: google-cloud-operations-suite-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Observability Cloud Operations Suite Folders API
  slug: google-cloud-operations-suite-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-operations-suite/openapi/google-cloud-operations-suite-folders-api-openapi.yml
- filename: google-cloud-operations-suite-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Observability Cloud Operations Suite Organizations API
  slug: google-cloud-operations-suite-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-operations-suite/openapi/google-cloud-operations-suite-organizations-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Observability Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Observability publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Observability API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Observability
provider_slug: google-cloud-operations-suite
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-operations-suite-folders-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-operations-suite-organizations-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-operations-suite-projects-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-cloud-operations-suite-scopes
source_filename: google-cloud-operations-suite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-operations-suite-folders-api-openapi.yml, openapi/google-cloud-operations-suite-organizations-api-openapi.yml,\n  openapi/google-cloud-operations-suite-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-operations-suite-folders-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-operations-suite-organizations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-operations-suite-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n\
  scopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-operations-suite-folders-api-openapi.yml\n  - openapi/google-cloud-operations-suite-organizations-api-openapi.yml\n  - openapi/google-cloud-operations-suite-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-operations-suite/scopes/google-cloud-operations-suite-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Error Reporting
- Google Cloud
- Logging
- Monitoring
- Observability
- Profiling
- Stackdriver
- Tracing
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
