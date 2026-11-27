---
api_specs:
- filename: google-dialogflow-projects-api-openapi.yml
  format: yaml
  label: Google Dialogflow Projects API
  slug: google-dialogflow-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-dialogflow/openapi/google-dialogflow-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Dialogflow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Dialogflow publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Dialogflow API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Dialogflow
provider_slug: google-dialogflow
schemes:
- description: Google OAuth 2.0. Scopes are declared per operation in the Discovery Document.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-dialogflow-cx-v3-openapi.yml
- description: Google OAuth 2.0. Scopes are declared per operation in the Discovery Document.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-dialogflow-es-v2-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/dialogflow
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View, manage and query your Dialogflow agents
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/dialogflow
slug: google-dialogflow-scopes
source_filename: google-dialogflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: derived\nsource: openapi/google-dialogflow-cx-v3-openapi.yml, openapi/google-dialogflow-es-v2-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-dialogflow-cx-v3-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0. Scopes are declared per operation in the Discovery Document.\n- name: OAuth2\n  source: openapi/google-dialogflow-es-v2-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0. Scopes are declared per operation in the Discovery Document.\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-dialogflow-cx-v3-openapi.yml\n  - openapi/google-dialogflow-es-v2-openapi.yml\n- scope: https://www.googleapis.com/auth/dialogflow\n  description: View, manage and query your Dialogflow agents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-dialogflow-cx-v3-openapi.yml\n  - openapi/google-dialogflow-es-v2-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-dialogflow/scopes/google-dialogflow-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Agents
- Artificial Intelligence
- Chatbots
- Conversational AI
- Google Cloud
- Machine Learning
- Natural Language Processing
- Speech Recognition
- Virtual Agents
- Voice Assistant
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
