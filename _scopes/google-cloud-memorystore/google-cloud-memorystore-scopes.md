---
api_specs:
- filename: google-cloud-memorystore-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Memorystore Projects API
  slug: google-cloud-memorystore-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-memorystore/openapi/google-cloud-memorystore-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Memorystore Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Memorystore publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Memorystore API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Memorystore
provider_slug: google-cloud-memorystore
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-memorystore-memcache-projects-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-memorystore-redis-projects-api-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/redis.read-only
- https://www.googleapis.com/auth/redis.read-write
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: See your Google Cloud Memorystore for Redis data and the email address of your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/redis.read-only
- description: See, edit, configure, and delete your Google Cloud Memorystore for Redis data and see the email address for your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/redis.read-write
slug: google-cloud-memorystore-scopes
source_filename: google-cloud-memorystore-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-memorystore-memcache-projects-api-openapi.yml, openapi/google-cloud-memorystore-redis-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-memorystore-memcache-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-memorystore-redis-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-memorystore-memcache-projects-api-openapi.yml\n\
  \  - openapi/google-cloud-memorystore-redis-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/redis.read-only\n  description: See your Google Cloud Memorystore for Redis data and the email address of your\n    Google Account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-memorystore-redis-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/redis.read-write\n  description: See, edit, configure, and delete your Google Cloud Memorystore for Redis data\n    and see the email address for your Google Account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-memorystore-redis-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-memorystore/scopes/google-cloud-memorystore-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Cache
- Google Cloud
- In-Memory
- Memcached
- Redis
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
