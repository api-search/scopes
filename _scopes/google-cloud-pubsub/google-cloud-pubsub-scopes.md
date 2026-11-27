---
api_specs:
- filename: google-cloud-pubsub-admin-api-openapi.yml
  format: yaml
  label: Google Cloud Pub/Sub Admin API
  slug: google-cloud-pubsub-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-pubsub/openapi/google-cloud-pubsub-admin-api-openapi.yml
- filename: google-cloud-pubsub-cursor-api-openapi.yml
  format: yaml
  label: Google Cloud Pub/Sub Cursor API
  slug: google-cloud-pubsub-cursor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-pubsub/openapi/google-cloud-pubsub-cursor-api-openapi.yml
- filename: google-cloud-pubsub-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Pub/Sub Projects API
  slug: google-cloud-pubsub-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-pubsub/openapi/google-cloud-pubsub-projects-api-openapi.yml
- filename: google-cloud-pubsub-topicstats-api-openapi.yml
  format: yaml
  label: Google Cloud Pub/Sub Topic Stats API
  slug: google-cloud-pubsub-topicstats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-pubsub/openapi/google-cloud-pubsub-topicstats-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Pub/Sub Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Pub/Sub publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Pub/Sub API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Pub/Sub
provider_slug: google-cloud-pubsub
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-pubsub-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/pubsub
scopes:
- description: Full access to Google Cloud Platform
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View and manage Pub/Sub topics and subscriptions
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/pubsub
slug: google-cloud-pubsub-scopes
source_filename: google-cloud-pubsub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-pubsub-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-pubsub-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Google Cloud Platform\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-pubsub-openapi.yml\n- scope: https://www.googleapis.com/auth/pubsub\n  description: View and manage Pub/Sub topics and subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-pubsub-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-pubsub/scopes/google-cloud-pubsub-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Event-Driven
- Google Cloud
- Messaging
- Pub/Sub
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
