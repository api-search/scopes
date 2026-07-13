---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google AdMob API
  slug: google-admob
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Admob Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google AdMob publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google AdMob API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google AdMob
provider_slug: google-admob
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/admob.readonly
- https://www.googleapis.com/auth/admob.report
scopes:
- description: View AdMob data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admob.readonly
- description: View AdMob reports
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admob.report
slug: google-admob-scopes
source_filename: google-admob-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/admob.readonly\n  description: View AdMob data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n- scope: https://www.googleapis.com/auth/admob.report\n  description: View AdMob reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/scopes/google-admob-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Ad Mediation
- AdMob
- App Monetization
- Mobile Advertising
- Mobile Apps
- Reports
token_urls:
- https://oauth2.googleapis.com/token
---
