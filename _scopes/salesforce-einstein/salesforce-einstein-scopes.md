---
api_specs:
- filename: salesforce-einstein-ai-record-insights-api-openapi.yml
  format: yaml
  label: Salesforce Einstein AI Record Insights API
  slug: salesforce-einstein-ai-record-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-ai-record-insights-api-openapi.yml
- filename: salesforce-einstein-api-usage-api-openapi.yml
  format: yaml
  label: Salesforce Einstein API Usage API
  slug: salesforce-einstein-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-api-usage-api-openapi.yml
- filename: salesforce-einstein-bot-definitions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Bot Definitions API
  slug: salesforce-einstein-bot-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-bot-definitions-api-openapi.yml
- filename: salesforce-einstein-bot-versions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Bot Versions API
  slug: salesforce-einstein-bot-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-bot-versions-api-openapi.yml
- filename: salesforce-einstein-dashboards-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Dashboards API
  slug: salesforce-einstein-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-dashboards-api-openapi.yml
- filename: salesforce-einstein-datasets-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Datasets API
  slug: salesforce-einstein-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-datasets-api-openapi.yml
- filename: salesforce-einstein-examples-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Examples API
  slug: salesforce-einstein-examples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-examples-api-openapi.yml
- filename: salesforce-einstein-feedback-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Feedback API
  slug: salesforce-einstein-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-feedback-api-openapi.yml
- filename: salesforce-einstein-generations-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Generations API
  slug: salesforce-einstein-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-generations-api-openapi.yml
- filename: salesforce-einstein-lenses-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Lenses API
  slug: salesforce-einstein-lenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-lenses-api-openapi.yml
- filename: salesforce-einstein-messages-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Messages API
  slug: salesforce-einstein-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-messages-api-openapi.yml
- filename: salesforce-einstein-models-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Models API
  slug: salesforce-einstein-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-models-api-openapi.yml
- filename: salesforce-einstein-prediction-definitions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Prediction Definitions API
  slug: salesforce-einstein-prediction-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-prediction-definitions-api-openapi.yml
- filename: salesforce-einstein-predictions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Predictions API
  slug: salesforce-einstein-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-predictions-api-openapi.yml
- filename: salesforce-einstein-prompt-templates-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Prompt Templates API
  slug: salesforce-einstein-prompt-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-prompt-templates-api-openapi.yml
- filename: salesforce-einstein-sessions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Sessions API
  slug: salesforce-einstein-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-sessions-api-openapi.yml
- filename: salesforce-einstein-stories-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Stories API
  slug: salesforce-einstein-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-stories-api-openapi.yml
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
