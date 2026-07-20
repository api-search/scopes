---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: https://developers.google.com/identity/protocols/oauth2/scopes#firebase
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Firebase Scopes
name_suffix: OAuth Scopes
note: Firebase's Google-hosted REST APIs authorize with Google OAuth 2.0 scopes. Scopes below are documented by Google for Firebase-related services.
overview: 'Firebase publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Firebase API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Firebase
provider_slug: firebase
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: GoogleOAuth2
scope_count: 8
scope_names:
- https://www.googleapis.com/auth/firebase
- https://www.googleapis.com/auth/firebase.readonly
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/cloud-platform.read-only
- https://www.googleapis.com/auth/datastore
- https://www.googleapis.com/auth/firebase.messaging
- https://www.googleapis.com/auth/firebase.database
- https://www.googleapis.com/auth/userinfo.email
scopes:
- description: View and administer all your Firebase data and settings.
  flows: []
  scope: https://www.googleapis.com/auth/firebase
- description: View all your Firebase data and settings.
  flows: []
  scope: https://www.googleapis.com/auth/firebase.readonly
- description: View and manage your data across Google Cloud Platform services.
  flows: []
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View your data across Google Cloud Platform services.
  flows: []
  scope: https://www.googleapis.com/auth/cloud-platform.read-only
- description: View and manage Cloud Firestore / Datastore data.
  flows: []
  scope: https://www.googleapis.com/auth/datastore
- description: Send messages and manage messaging via Firebase Cloud Messaging.
  flows: []
  scope: https://www.googleapis.com/auth/firebase.messaging
- description: View and administer Firebase Realtime Database data.
  flows: []
  scope: https://www.googleapis.com/auth/firebase.database
- description: See the primary Google Account email address.
  flows: []
  scope: https://www.googleapis.com/auth/userinfo.email
slug: firebase-scopes
source_filename: firebase-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://developers.google.com/identity/protocols/oauth2/scopes#firebase,\n  https://firebase.google.com/docs/projects/api/reference/rest\ndocs: https://developers.google.com/identity/protocols/oauth2/scopes#firebase\nnote: >-\n  Firebase's Google-hosted REST APIs authorize with Google OAuth 2.0 scopes.\n  Scopes below are documented by Google for Firebase-related services.\nschemes:\n- name: GoogleOAuth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/firebase\n  description: View and administer all your Firebase data and settings.\n- scope: https://www.googleapis.com/auth/firebase.readonly\n  description: View all your Firebase data and settings.\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: View and manage your data across Google Cloud\
  \ Platform services.\n- scope: https://www.googleapis.com/auth/cloud-platform.read-only\n  description: View your data across Google Cloud Platform services.\n- scope: https://www.googleapis.com/auth/datastore\n  description: View and manage Cloud Firestore / Datastore data.\n- scope: https://www.googleapis.com/auth/firebase.messaging\n  description: Send messages and manage messaging via Firebase Cloud Messaging.\n- scope: https://www.googleapis.com/auth/firebase.database\n  description: View and administer Firebase Realtime Database data.\n- scope: https://www.googleapis.com/auth/userinfo.email\n  description: See the primary Google Account email address.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firebase/refs/heads/main/scopes/firebase-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Company
- Backend as a Service
- Application Development
- Mobile
- Web
- Authentication
- Database
- Cloud Functions
- Messaging
- Google
token_urls:
- https://oauth2.googleapis.com/token
---
