---
api_specs:
- filename: openapi.json
  format: json
  label: Einstein Vision API
  slug: einstein-vision-api
  spec_type: OpenAPI
  url: https://api.einstein.ai/v2/vision/openapi.json
- filename: openapi.json
  format: json
  label: Einstein Language API
  slug: einstein-language-api
  spec_type: OpenAPI
  url: https://api.einstein.ai/v2/language/openapi.json
- filename: salesforce-einstein-prediction-builder-openapi.yml
  format: yaml
  label: Einstein Prediction Builder API
  slug: einstein-prediction-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-prediction-builder-openapi.yml
- filename: salesforce-einstein-discovery-openapi.yml
  format: yaml
  label: Einstein Discovery API
  slug: einstein-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-discovery-openapi.yml
- filename: salesforce-einstein-bots-openapi.yml
  format: yaml
  label: Einstein Bots API
  slug: einstein-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-bots-openapi.yml
- filename: salesforce-einstein-gpt-openapi.yml
  format: yaml
  label: Einstein GPT API
  slug: einstein-gpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-gpt-openapi.yml
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Salesforce Einstein Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce Einstein publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Einstein API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Einstein
provider_slug: salesforce-einstein
schemes:
- description: Salesforce OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-einstein-bots-openapi.yml
- description: Salesforce OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-einstein-discovery-openapi.yml
- description: Salesforce OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-einstein-gpt-openapi.yml
- description: Salesforce OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-einstein-prediction-builder-openapi.yml
scope_count: 3
scope_names:
- api
- einstein_gpt
- wave_api
scopes:
- description: Full access to Salesforce APIs
  flows:
  - authorizationCode
  scope: api
- description: Access to Einstein AI features
  flows:
  - authorizationCode
  scope: einstein_gpt
- description: Access to Analytics APIs
  flows:
  - authorizationCode
  scope: wave_api
slug: salesforce-einstein-scopes
source_filename: salesforce-einstein-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-einstein-bots-openapi.yml, openapi/salesforce-einstein-discovery-openapi.yml,\n  openapi/salesforce-einstein-gpt-openapi.yml, openapi/salesforce-einstein-prediction-builder-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/salesforce-einstein-bots-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication.\n- name: oauth2\n  source: openapi/salesforce-einstein-discovery-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication.\n- name: oauth2\n  source: openapi/salesforce-einstein-gpt-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication.\n- name: oauth2\n  source: openapi/salesforce-einstein-prediction-builder-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication.\nscopes:\n- scope: api\n  description: Full access to Salesforce APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-einstein-bots-openapi.yml\n  - openapi/salesforce-einstein-discovery-openapi.yml\n  - openapi/salesforce-einstein-gpt-openapi.yml\n  - openapi/salesforce-einstein-prediction-builder-openapi.yml\n- scope: einstein_gpt\n  description: Access to Einstein AI features\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-einstein-bots-openapi.yml\n\
  \  - openapi/salesforce-einstein-gpt-openapi.yml\n  - openapi/salesforce-einstein-prediction-builder-openapi.yml\n- scope: wave_api\n  description: Access to Analytics APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-einstein-discovery-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/scopes/salesforce-einstein-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Artificial Intelligence
- Computer Vision
- CRM
- Machine Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
