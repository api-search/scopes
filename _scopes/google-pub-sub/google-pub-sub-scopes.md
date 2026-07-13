---
api_specs:
- filename: google-pub-sub-openapi.yml
  format: yaml
  label: Google Pub/Sub
  slug: google-pub-sub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/openapi/google-pub-sub-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Pub Sub Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Pub/Sub publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Pub/Sub API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Pub/Sub
provider_slug: google-pub-sub
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-pub-sub-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/pubsub
scopes:
- description: Full access to Google Cloud
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: Manage Pub/Sub resources
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/pubsub
slug: google-pub-sub-scopes
source_filename: google-pub-sub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-pub-sub-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-pub-sub-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Google Cloud\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-pub-sub-openapi.yml\n- scope: https://www.googleapis.com/auth/pubsub\n  description: Manage Pub/Sub resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-pub-sub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/scopes/google-pub-sub-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Cloud
- Event-Driven
- Google Cloud
- Messaging
- Pub/Sub
- Streaming
token_urls:
- https://oauth2.googleapis.com/token
---
