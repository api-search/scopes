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
docs: https://developers.google.com/android-publisher/authorization
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Android Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Android publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Android API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Android
provider_slug: android
schemes:
- description: OAuth 2.0 authentication for the Google Play Developer API. Server-to-server access uses a Google Cloud service account granted access in the Google Play Console; the Web Server (authorizationCode) flow is documented for interactive access. A single coarse-grained scope grants full API access.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-play-developer-api.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/androidpublisher
scopes:
- description: View and manage your Google Play Developer account — full access to publishing, purchases, subscriptions, reviews, and orders. This is the only scope the API exposes; per-resource authorization is enforced by Play Console account roles and permissions, not by additional OAuth scopes.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/androidpublisher
slug: android-scopes
source_filename: android-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/google-play-developer-api.yml\ndocs: https://developers.google.com/android-publisher/authorization\nschemes:\n- name: oauth2\n  source: openapi/google-play-developer-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: >-\n    OAuth 2.0 authentication for the Google Play Developer API. Server-to-server\n    access uses a Google Cloud service account granted access in the Google Play\n    Console; the Web Server (authorizationCode) flow is documented for interactive\n    access. A single coarse-grained scope grants full API access.\nscopes:\n- scope: https://www.googleapis.com/auth/androidpublisher\n  short: androidpublisher\n  description: >-\n    View and manage your Google Play Developer account — full access to publishing,\n    purchases, subscriptions, reviews, and orders. This is the only\
  \ scope the API\n    exposes; per-resource authorization is enforced by Play Console account roles\n    and permissions, not by additional OAuth scopes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-play-developer-api.yml\n  docs: https://developers.google.com/android-publisher/authorization\n"
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
