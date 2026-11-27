---
api_specs:
- filename: google-cloud-endpoints-operations-api-openapi.yml
  format: yaml
  label: Google Cloud Endpoints Operations API
  slug: google-cloud-endpoints-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-endpoints/openapi/google-cloud-endpoints-operations-api-openapi.yml
- filename: google-cloud-endpoints-services-api-openapi.yml
  format: yaml
  label: Google Cloud Endpoints Services API
  slug: google-cloud-endpoints-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-endpoints/openapi/google-cloud-endpoints-services-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Endpoints Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Endpoints publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Endpoints API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Endpoints
provider_slug: google-cloud-endpoints
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-endpoints-servicecontrol-services-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-endpoints-servicemanagement-operations-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-endpoints-servicemanagement-services-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-endpoints-serviceusage-operations-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-endpoints-serviceusage-services-api-openapi.yml
scope_count: 5
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/cloud-platform.read-only
- https://www.googleapis.com/auth/service.management
- https://www.googleapis.com/auth/service.management.readonly
- https://www.googleapis.com/auth/servicecontrol
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View your data across Google Cloud services and see the email address of your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform.read-only
- description: Manage your Google API service configuration
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/service.management
- description: View your Google API service configuration
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/service.management.readonly
- description: Manage your Google Service Control data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/servicecontrol
slug: google-cloud-endpoints-scopes
source_filename: google-cloud-endpoints-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-endpoints-servicecontrol-services-api-openapi.yml, openapi/google-cloud-endpoints-servicemanagement-operations-api-openapi.yml,\n  openapi/google-cloud-endpoints-servicemanagement-services-api-openapi.yml, openapi/google-cloud-endpoints-serviceusage-operations-api-openapi.yml,\n  openapi/google-cloud-endpoints-serviceusage-services-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-endpoints-servicecontrol-services-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-endpoints-servicemanagement-operations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-endpoints-servicemanagement-services-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-endpoints-serviceusage-operations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-endpoints-serviceusage-services-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-endpoints-servicecontrol-services-api-openapi.yml\n  - openapi/google-cloud-endpoints-servicemanagement-operations-api-openapi.yml\n\
  \  - openapi/google-cloud-endpoints-servicemanagement-services-api-openapi.yml\n  - openapi/google-cloud-endpoints-serviceusage-operations-api-openapi.yml\n  - openapi/google-cloud-endpoints-serviceusage-services-api-openapi.yml\n- scope: https://www.googleapis.com/auth/cloud-platform.read-only\n  description: View your data across Google Cloud services and see the email address of your\n    Google Account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-endpoints-servicemanagement-operations-api-openapi.yml\n  - openapi/google-cloud-endpoints-servicemanagement-services-api-openapi.yml\n  - openapi/google-cloud-endpoints-serviceusage-operations-api-openapi.yml\n  - openapi/google-cloud-endpoints-serviceusage-services-api-openapi.yml\n- scope: https://www.googleapis.com/auth/service.management\n  description: Manage your Google API service configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-endpoints-servicemanagement-operations-api-openapi.yml\n\
  \  - openapi/google-cloud-endpoints-servicemanagement-services-api-openapi.yml\n  - openapi/google-cloud-endpoints-serviceusage-operations-api-openapi.yml\n  - openapi/google-cloud-endpoints-serviceusage-services-api-openapi.yml\n- scope: https://www.googleapis.com/auth/service.management.readonly\n  description: View your Google API service configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-endpoints-servicemanagement-operations-api-openapi.yml\n  - openapi/google-cloud-endpoints-servicemanagement-services-api-openapi.yml\n- scope: https://www.googleapis.com/auth/servicecontrol\n  description: Manage your Google Service Control data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-endpoints-servicecontrol-services-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-endpoints/scopes/google-cloud-endpoints-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- API Gateway
- API Management
- Authentication
- Google Cloud
- Monitoring
- Rate Limiting
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
