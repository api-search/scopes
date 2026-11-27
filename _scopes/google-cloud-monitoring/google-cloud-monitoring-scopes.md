---
api_specs:
- filename: google-cloud-monitoring-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Monitoring Projects API
  slug: google-cloud-monitoring-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-monitoring/openapi/google-cloud-monitoring-projects-api-openapi.yml
- filename: google-cloud-monitoring-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Monitoring Cloud Monitoring Folders API
  slug: google-cloud-monitoring-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-monitoring/openapi/google-cloud-monitoring-folders-api-openapi.yml
- filename: google-cloud-monitoring-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Monitoring Cloud Monitoring Organizations API
  slug: google-cloud-monitoring-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-monitoring/openapi/google-cloud-monitoring-organizations-api-openapi.yml
- filename: google-cloud-monitoring-services-api-openapi.yml
  format: yaml
  label: Google Cloud Monitoring Cloud Monitoring Services API
  slug: google-cloud-monitoring-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-monitoring/openapi/google-cloud-monitoring-services-api-openapi.yml
- filename: google-cloud-monitoring-uptimecheckips-api-openapi.yml
  format: yaml
  label: Google Cloud Monitoring Uptime Check Ips API
  slug: google-cloud-monitoring-uptimecheckips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-monitoring/openapi/google-cloud-monitoring-uptimecheckips-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Monitoring Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Monitoring publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Monitoring API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Monitoring
provider_slug: google-cloud-monitoring
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-monitoring-folders-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-monitoring-organizations-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-monitoring-projects-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-monitoring-services-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-monitoring-uptime-check-ips-api-openapi.yml
scope_count: 4
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/monitoring
- https://www.googleapis.com/auth/monitoring.read
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
- description: View monitoring data for all of your Google Cloud and third-party projects
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/monitoring.read
- description: Publish metric data to your Google Cloud projects
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/monitoring.write
slug: google-cloud-monitoring-scopes
source_filename: google-cloud-monitoring-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-monitoring-folders-api-openapi.yml, openapi/google-cloud-monitoring-organizations-api-openapi.yml,\n  openapi/google-cloud-monitoring-projects-api-openapi.yml, openapi/google-cloud-monitoring-services-api-openapi.yml,\n  openapi/google-cloud-monitoring-uptime-check-ips-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-monitoring-folders-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-monitoring-organizations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-monitoring-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-monitoring-services-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-monitoring-uptime-check-ips-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-monitoring-folders-api-openapi.yml\n  - openapi/google-cloud-monitoring-organizations-api-openapi.yml\n  - openapi/google-cloud-monitoring-projects-api-openapi.yml\n\
  \  - openapi/google-cloud-monitoring-services-api-openapi.yml\n  - openapi/google-cloud-monitoring-uptime-check-ips-api-openapi.yml\n- scope: https://www.googleapis.com/auth/monitoring\n  description: View and write monitoring data for all of your Google and third-party Cloud and\n    API projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-monitoring-folders-api-openapi.yml\n  - openapi/google-cloud-monitoring-organizations-api-openapi.yml\n  - openapi/google-cloud-monitoring-projects-api-openapi.yml\n  - openapi/google-cloud-monitoring-services-api-openapi.yml\n  - openapi/google-cloud-monitoring-uptime-check-ips-api-openapi.yml\n- scope: https://www.googleapis.com/auth/monitoring.read\n  description: View monitoring data for all of your Google Cloud and third-party projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-monitoring-folders-api-openapi.yml\n  - openapi/google-cloud-monitoring-organizations-api-openapi.yml\n  - openapi/google-cloud-monitoring-projects-api-openapi.yml\n\
  \  - openapi/google-cloud-monitoring-services-api-openapi.yml\n  - openapi/google-cloud-monitoring-uptime-check-ips-api-openapi.yml\n- scope: https://www.googleapis.com/auth/monitoring.write\n  description: Publish metric data to your Google Cloud projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-monitoring-folders-api-openapi.yml\n  - openapi/google-cloud-monitoring-organizations-api-openapi.yml\n  - openapi/google-cloud-monitoring-projects-api-openapi.yml\n  - openapi/google-cloud-monitoring-services-api-openapi.yml\n  - openapi/google-cloud-monitoring-uptime-check-ips-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-monitoring/scopes/google-cloud-monitoring-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Alerting
- Dashboards
- Google Cloud
- Metrics
- Monitoring
- Observability
- SLO
- Uptime
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
