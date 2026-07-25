---
api_specs:
- filename: google-android-android-management-api-api-openapi.yml
  format: yaml
  label: Google Android Android Management API API
  slug: google-android-android-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-android-management-api-api-openapi.yml
- filename: google-android-device-api-openapi.yml
  format: yaml
  label: Google Android Device API
  slug: google-android-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-device-api-openapi.yml
- filename: google-android-devices-api-openapi.yml
  format: yaml
  label: Google Android Devices API
  slug: google-android-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-devices-api-openapi.yml
- filename: google-android-enrollmenttokens-api-openapi.yml
  format: yaml
  label: Google Android EnrollmentTokens API
  slug: google-android-enrollmenttokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-enrollmenttokens-api-openapi.yml
- filename: google-android-enterprises-api-openapi.yml
  format: yaml
  label: Google Android Enterprises API
  slug: google-android-enterprises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-enterprises-api-openapi.yml
- filename: google-android-policies-api-openapi.yml
  format: yaml
  label: Google Android Policies API
  slug: google-android-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-policies-api-openapi.yml
- filename: google-android-policy-api-openapi.yml
  format: yaml
  label: Google Android Policy API
  slug: google-android-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-policy-api-openapi.yml
- filename: google-android-webapps-api-openapi.yml
  format: yaml
  label: Google Android WebApps API
  slug: google-android-webapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/openapi/google-android-webapps-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.google.com/identity/protocols/oauth2/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Android Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Android publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Android API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Android
provider_slug: google-android
schemes:
- authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
  name: OAuth2
  tokenUrl: https://oauth2.googleapis.com/token
  type: authorizationCode
scope_count: 9
scope_names:
- https://www.googleapis.com/auth/androidmanagement
- https://www.googleapis.com/auth/androidpublisher
- https://www.googleapis.com/auth/androidenterprise
- https://www.googleapis.com/auth/firebase.messaging
- https://www.googleapis.com/auth/games
- https://www.googleapis.com/auth/drive.appdata
- https://www.googleapis.com/auth/playintegrity
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/cloud-platform.read-only
scopes:
- description: Manage Android devices and apps for your customers
  flows: []
  scope: https://www.googleapis.com/auth/androidmanagement
- description: View and manage your Google Play Developer account
  flows: []
  scope: https://www.googleapis.com/auth/androidpublisher
- description: Manage corporate Android devices
  flows: []
  scope: https://www.googleapis.com/auth/androidenterprise
- description: Send messages and manage messaging subscriptions for your Firebase applications
  flows: []
  scope: https://www.googleapis.com/auth/firebase.messaging
- description: Create, edit, and delete your Google Play Games activity
  flows: []
  scope: https://www.googleapis.com/auth/games
- description: See, create, and delete its own configuration data in your Google Drive
  flows: []
  scope: https://www.googleapis.com/auth/drive.appdata
- description: Access the Play Integrity API to verify device and app integrity
  flows: []
  scope: https://www.googleapis.com/auth/playintegrity
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account
  flows: []
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View your data across Google Cloud services and see the email address of your Google Account
  flows: []
  scope: https://www.googleapis.com/auth/cloud-platform.read-only
slug: google-android-scopes
source_filename: google-android-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: Google API Discovery documents ($discovery/rest) for each API\ndocs: https://developers.google.com/identity/protocols/oauth2/scopes\nnotes: >-\n  All Google Android APIs authorize via Google OAuth 2.0 (authorization code for\n  users, service-account JWT bearer for server-to-server). Scopes below are taken\n  verbatim from each API's authoritative Google Discovery document. The Android\n  Device Provisioning Partner API and Android Over the Air API do not declare\n  public oauth2 scopes in their Discovery docs (partner/allow-listed access).\nschemes:\n  - name: OAuth2\n    type: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n  - scope: https://www.googleapis.com/auth/androidmanagement\n    description: Manage Android devices and apps for your customers\n    apis: [android-management-api]\n  - scope: https://www.googleapis.com/auth/androidpublisher\n\
  \    description: View and manage your Google Play Developer account\n    apis: [google-play-developer-api, google-play-games-services-api]\n  - scope: https://www.googleapis.com/auth/androidenterprise\n    description: Manage corporate Android devices\n    apis: [google-play-emm-api]\n  - scope: https://www.googleapis.com/auth/firebase.messaging\n    description: Send messages and manage messaging subscriptions for your Firebase applications\n    apis: [firebase-cloud-messaging-api]\n  - scope: https://www.googleapis.com/auth/games\n    description: Create, edit, and delete your Google Play Games activity\n    apis: [google-play-games-services-api]\n  - scope: https://www.googleapis.com/auth/drive.appdata\n    description: See, create, and delete its own configuration data in your Google Drive\n    apis: [google-play-games-services-api]\n  - scope: https://www.googleapis.com/auth/playintegrity\n    description: Access the Play Integrity API to verify device and app integrity\n    apis:\
  \ [play-integrity-api]\n  - scope: https://www.googleapis.com/auth/cloud-platform\n    description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account\n    apis: [firebase-cloud-messaging-api, cloud-testing-api]\n  - scope: https://www.googleapis.com/auth/cloud-platform.read-only\n    description: View your data across Google Cloud services and see the email address of your Google Account\n    apis: [cloud-testing-api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/scopes/google-android-scopes.yml
summary_line: 9 scopes
tags:
- Android
- Google
- Mobile Development
- Mobile Operating System
- Open Source
token_urls: []
---
