---
api_specs:
- filename: rest
  format: yaml
  label: Android Management API
  slug: android-management-api
  spec_type: OpenAPI
  url: https://androidmanagement.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Play Developer API
  slug: google-play-developer-api
  spec_type: OpenAPI
  url: https://androidpublisher.googleapis.com/$discovery/rest?version=v3
- filename: rest
  format: yaml
  label: Firebase Cloud Messaging API
  slug: firebase-cloud-messaging-api
  spec_type: OpenAPI
  url: https://fcm.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Play Games Services API
  slug: google-play-games-services-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/games/v1/rest
- filename: rest
  format: yaml
  label: Android Over the Air API
  slug: android-over-the-air-api
  spec_type: OpenAPI
  url: https://androidovertheair.googleapis.com/$discovery/rest?version=v1
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Android Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Android publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Android API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Android
provider_slug: google-android
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-android-openapi.yml
scope_count: 1
scope_names:
- androidmanagement
scopes:
- description: Manage Android devices and apps for your customers
  flows:
  - authorizationCode
  scope: androidmanagement
slug: google-android-scopes
source_filename: google-android-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-android-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-android-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: androidmanagement\n  description: Manage Android devices and apps for your customers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-android-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/scopes/google-android-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Android
- Google
- Mobile Development
- Mobile Operating System
- Open Source
token_urls:
- https://oauth2.googleapis.com/token
---
