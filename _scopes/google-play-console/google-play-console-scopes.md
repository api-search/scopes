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
name: Google Play Console Scopes
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
  source: openapi/openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/playdeveloperreporting
scopes:
- description: Access Play developer reporting data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/playdeveloperreporting
slug: google-play-console-scopes
source_filename: google-play-console-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/playdeveloperreporting\n  description: Access Play developer reporting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-play-console/refs/heads/main/scopes/google-play-console-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Analytics
- Android
- Apps
- Google Play Console
- Quality
- Reporting
token_urls:
- https://oauth2.googleapis.com/token
---
