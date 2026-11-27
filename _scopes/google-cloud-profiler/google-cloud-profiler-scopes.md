---
api_specs:
- filename: google-cloud-profiler-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Profiler Projects API
  slug: google-cloud-profiler-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-profiler/openapi/google-cloud-profiler-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Profiler Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Profiler publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Profiler API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Profiler
provider_slug: google-cloud-profiler
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-profiler-projects-api-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/monitoring
- https://www.googleapis.com/auth/monitoring.write
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View and write monitoring data for all of your Google and third-party Cloud and API projects
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/monitoring
- description: Publish metric data to your Google Cloud projects
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/monitoring.write
slug: google-cloud-profiler-scopes
source_filename: google-cloud-profiler-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-profiler-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-profiler-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-profiler-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/monitoring\n  description: View and write monitoring data for all of your Google and third-party Cloud and\n    API projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-profiler-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/monitoring.write\n  description:\
  \ Publish metric data to your Google Cloud projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-profiler-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-profiler/scopes/google-cloud-profiler-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- CPU
- Flame Graphs
- Google Cloud
- Memory
- Observability
- Performance
- Profiling
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
