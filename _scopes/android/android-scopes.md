---
api_specs:
- filename: google-play-developer-api.yml
  format: yaml
  label: Google Play Developer APIs
  slug: google-play-developer-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/openapi/google-play-developer-api.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Android Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Android publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Android API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Android
provider_slug: android
schemes:
- description: OAuth 2.0 authentication for accessing the Google Play Developer API. Requires a service account with appropriate permissions in the Google Play Console.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-play-developer-api.yml
scope_count: 1
scope_names:
- androidpublisher
scopes:
- description: Full access to Google Play Developer API
  flows:
  - authorizationCode
  scope: androidpublisher
slug: android-scopes
source_filename: android-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-play-developer-api.yml\nschemes:\n- name: oauth2\n  source: openapi/google-play-developer-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for accessing the Google Play Developer API. Requires\n    a service account with appropriate permissions in the Google Play Console.\nscopes:\n- scope: androidpublisher\n  description: Full access to Google Play Developer API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-play-developer-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/scopes/android-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- AI
- Android
- Automotive
- Google
- Machine Learning
- Mobile Development
- SDK
- TV
- Wearables
token_urls:
- https://oauth2.googleapis.com/token
---
