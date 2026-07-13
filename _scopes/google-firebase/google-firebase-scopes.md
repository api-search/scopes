---
api_specs:
- filename: firebase-realtime-database-openapi.yml
  format: yaml
  label: Firebase Realtime Database API
  slug: firebase-realtime-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-firebase/refs/heads/main/openapi/firebase-realtime-database-openapi.yml
- filename: firebase-cloud-messaging-openapi.yml
  format: yaml
  label: Firebase Cloud Messaging API (FCM)
  slug: firebase-cloud-messaging-api-fcm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-firebase/refs/heads/main/openapi/firebase-cloud-messaging-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Firebase Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Firebase publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Firebase API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Firebase
provider_slug: google-firebase
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/firebase-cloud-messaging-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/firebase.messaging
scopes:
- description: Send FCM messages
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/firebase.messaging
slug: google-firebase-scopes
source_filename: google-firebase-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/firebase-cloud-messaging-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/firebase-cloud-messaging-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/firebase.messaging\n  description: Send FCM messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/firebase-cloud-messaging-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-firebase/refs/heads/main/scopes/google-firebase-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Analytics
- Authentication
- Backend as a Service
- Cloud Messaging
- Google Cloud
- Hosting
- Mobile
- Real-Time Database
token_urls:
- https://oauth2.googleapis.com/token
---
