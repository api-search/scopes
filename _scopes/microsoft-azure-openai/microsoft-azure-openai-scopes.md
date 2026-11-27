---
api_specs:
- filename: azure-openai-asyncapi.yml
  format: yaml
  label: Azure OpenAI Inference REST API
  slug: inference-api
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/azure-openai/asyncapi/azure-openai-asyncapi.yml
- filename: microsoft-azure-openai-batch-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Batch: API'
  slug: microsoft-azure-openai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-batch-api-openapi.yml
- filename: microsoft-azure-openai-deployments-api-openapi.yml
  format: yaml
  label: Azure OpenAI Service Deployments API
  slug: microsoft-azure-openai-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-deployments-api-openapi.yml
- filename: microsoft-azure-openai-files-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Files: API'
  slug: microsoft-azure-openai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-files-api-openapi.yml
- filename: microsoft-azure-openai-fine-tuning-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Fine Tuning: API'
  slug: microsoft-azure-openai-fine-tuning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-fine-tuning-api-openapi.yml
- filename: microsoft-azure-openai-models-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Models: API'
  slug: microsoft-azure-openai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-models-api-openapi.yml
- filename: microsoft-azure-openai-uploadfile-api-openapi.yml
  format: yaml
  label: 'Azure OpenAI Service Upload File: API'
  slug: microsoft-azure-openai-uploadfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-openai/openapi/microsoft-azure-openai-uploadfile-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure OpenAI Service Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure OpenAI Service publishes 2 OAuth 2.0 scopes via the clientCredentials and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure OpenAI Service API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure OpenAI Service
provider_slug: microsoft-azure-openai
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/microsoft-azure-openai-audio-api-openapi.yml
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/microsoft-azure-openai-chat-completions-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/microsoft-azure-openai-chat-completions-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/microsoft-azure-openai-completions-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/microsoft-azure-openai-embeddings-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/microsoft-azure-openai-images-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: implicit
  name: OAuth2Auth
  source: openapi/microsoft-azure-openai-v1-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-openai-openapi.yml
scope_count: 2
scope_names:
- https://cognitiveservices.azure.com/.default
- user_impersonation
scopes:
- description: Azure Cognitive Services data plane
  flows:
  - clientCredentials
  - implicit
  scope: https://cognitiveservices.azure.com/.default
- description: Impersonate user
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-openai-scopes
source_filename: microsoft-azure-openai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-openai-audio-api-openapi.yml, openapi/_superseded/microsoft-azure-openai-chat-completions-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-openai-completions-api-openapi.yml, openapi/_superseded/microsoft-azure-openai-embeddings-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-openai-images-api-openapi.yml, openapi/microsoft-azure-openai-openapi.yml,\n  openapi/microsoft-azure-openai-v1-openapi.yml\nschemes:\n- name: entra\n  source: openapi/_superseded/microsoft-azure-openai-audio-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n- name: entra\n  source: openapi/_superseded/microsoft-azure-openai-chat-completions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n\
  \  description: Microsoft Entra ID OAuth 2.0 bearer token\n- name: azure_auth\n  source: openapi/_superseded/microsoft-azure-openai-chat-completions-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: azure_auth\n  source: openapi/_superseded/microsoft-azure-openai-completions-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: azure_auth\n  source: openapi/_superseded/microsoft-azure-openai-embeddings-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: azure_auth\n  source: openapi/_superseded/microsoft-azure-openai-images-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: OAuth2Auth\n  source: openapi/microsoft-azure-openai-v1-openapi.yml\n  flows:\n  -\
  \ flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n- name: azure_auth\n  source: openapi/microsoft-azure-openai-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscopes:\n- scope: https://cognitiveservices.azure.com/.default\n  description: Azure Cognitive Services data plane\n  flows:\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/_superseded/microsoft-azure-openai-audio-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-openai-chat-completions-api-openapi.yml\n  - openapi/microsoft-azure-openai-v1-openapi.yml\n- scope: user_impersonation\n  description: Impersonate user\n  flows:\n  - implicit\n  sources:\n  - openapi/_superseded/microsoft-azure-openai-chat-completions-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-openai-completions-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-openai-embeddings-api-openapi.yml\n  -\
  \ openapi/_superseded/microsoft-azure-openai-images-api-openapi.yml\n  - openapi/microsoft-azure-openai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-openai/scopes/microsoft-azure-openai-scopes.yml
summary_line: 2 scopes · clientCredentials/implicit
tags:
- Artificial Intelligence
- Embeddings
- GPT
- Generative AI
- LLM
- OpenAI
token_bound: false
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
