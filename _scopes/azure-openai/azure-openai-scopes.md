---
api_specs:
- filename: azure-openai-asyncapi.yml
  format: yaml
  label: Azure OpenAI Inference REST API
  slug: inference-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-openai/refs/heads/main/asyncapi/azure-openai-asyncapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Azure Openai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure OpenAI Service publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure OpenAI Service API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure OpenAI Service
provider_slug: azure-openai
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/azure-openai-openapi.yml
scope_count: 1
scope_names:
- https://cognitiveservices.azure.com/.default
scopes:
- description: Azure Cognitive Services data plane
  flows:
  - clientCredentials
  scope: https://cognitiveservices.azure.com/.default
slug: azure-openai-scopes
source_filename: azure-openai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-openai-openapi.yml\nschemes:\n- name: entra\n  source: openapi/azure-openai-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\nscopes:\n- scope: https://cognitiveservices.azure.com/.default\n  description: Azure Cognitive Services data plane\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-openai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-openai/refs/heads/main/scopes/azure-openai-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- AI
- LLM
- Generative AI
- Azure
- OpenAI
- Foundation Models
- Chat Completions
- Embeddings
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
