---
api_specs:
- filename: google-play-console-anomalies-api-openapi.yml
  format: yaml
  label: Google Play Console Developer Reporting Play Console Anomalies API
  slug: google-play-console-anomalies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-play-console/openapi/google-play-console-anomalies-api-openapi.yml
- filename: google-play-console-apps-api-openapi.yml
  format: yaml
  label: Google Play Console Developer Reporting Play Console Apps API
  slug: google-play-console-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-play-console/openapi/google-play-console-apps-api-openapi.yml
- filename: google-play-console-vitals-api-openapi.yml
  format: yaml
  label: Google Play Console Developer Reporting Play Console Vitals API
  slug: google-play-console-vitals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-play-console/openapi/google-play-console-vitals-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Play Console Developer Reporting Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Play Console Developer Reporting publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Play Console Developer Reporting API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Play Console Developer Reporting
provider_slug: google-play-console
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-play-console-anomalies-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-play-console-apps-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-play-console-vitals-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/playdeveloperreporting
scopes:
- description: See metrics and data about the apps in your Google Play Developer account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/playdeveloperreporting
slug: google-play-console-scopes
source_filename: google-play-console-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-play-console-anomalies-api-openapi.yml, openapi/google-play-console-apps-api-openapi.yml,\n  openapi/google-play-console-vitals-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-play-console-anomalies-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-play-console-apps-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-play-console-vitals-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/playdeveloperreporting\n\
  \  description: See metrics and data about the apps in your Google Play Developer account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-play-console-anomalies-api-openapi.yml\n  - openapi/google-play-console-apps-api-openapi.yml\n  - openapi/google-play-console-vitals-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-play-console/scopes/google-play-console-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Analytics
- Android
- Application
- Google Play Console
- Quality
- Reporting
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
