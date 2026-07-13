---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Play Developer API
  slug: google-play-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-play/refs/heads/main/openapi/openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Play Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Play Developer publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Play Developer API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Play Developer
provider_slug: google-play
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/androidpublisher
scopes:
- description: Manage your Android apps
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/androidpublisher
slug: google-play-scopes
source_filename: google-play-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/androidpublisher\n  description: Manage your Android apps\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-play/refs/heads/main/scopes/google-play-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Android
- Apps
- Google Play
- In-App Purchases
- Mobile
- Publishing
- Subscriptions
token_urls:
- https://oauth2.googleapis.com/token
---
