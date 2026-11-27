---
api_specs:
- filename: google-translate-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Translation API Translate Projects API
  slug: google-translate-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-translate/openapi/google-translate-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Translation API Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Translation API publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Translation API API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Translation API
provider_slug: google-translate
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-translate-projects-api-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/cloud-translation
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: Translate text from one language to another using Google Translate
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-translation
slug: google-translate-scopes
source_filename: google-translate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-translate-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-translate-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-translate-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/cloud-translation\n  description: Translate text from one language to another using Google Translate\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-translate-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-translate/scopes/google-translate-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Google Cloud
- Internationalization
- Language Detection
- Localization
- Machine Translation
- Natural Language Processing
- Translation
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
