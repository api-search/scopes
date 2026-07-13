---
api_specs:
- filename: rest
  format: yaml
  label: Dialogflow API
  slug: dialogflow-api
  spec_type: OpenAPI
  url: https://dialogflow.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Dialogflow CX API
  slug: dialogflow-cx-api
  spec_type: OpenAPI
  url: https://dialogflow.googleapis.com/$discovery/rest?version=v3
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
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-dialogflow-openapi.yml
scope_count: 2
scope_names:
- cloud-platform
- dialogflow
scopes:
- description: View and manage your data across Google Cloud Platform services
  flows:
  - authorizationCode
  scope: cloud-platform
- description: View, manage and query your Dialogflow agents
  flows:
  - authorizationCode
  scope: dialogflow
slug: google-dialogflow-scopes
source_filename: google-dialogflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-dialogflow-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-dialogflow-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: cloud-platform\n  description: View and manage your data across Google Cloud Platform services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-dialogflow-openapi.yml\n- scope: dialogflow\n  description: View, manage and query your Dialogflow agents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-dialogflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-dialogflow/refs/heads/main/scopes/google-dialogflow-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Artificial Intelligence
- Chatbots
- Conversational AI
- Machine Learning
- Natural Language Processing
- Voice Assistants
token_urls:
- https://oauth2.googleapis.com/token
---
