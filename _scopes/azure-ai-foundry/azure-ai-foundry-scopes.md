---
api_specs:
- filename: azure-ai-foundry-openapi.yml
  format: yaml
  label: Azure AI Foundry REST API
  slug: foundry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Azure Ai Foundry Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure AI Foundry publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure AI Foundry API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure AI Foundry
provider_slug: azure-ai-foundry
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://ai.azure.com/.default)
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/azure-ai-foundry-openapi.yml
scope_count: 1
scope_names:
- https://ai.azure.com/.default
scopes:
- description: Default Foundry inference scope
  flows:
  - clientCredentials
  scope: https://ai.azure.com/.default
slug: azure-ai-foundry-scopes
source_filename: azure-ai-foundry-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-ai-foundry-openapi.yml\nschemes:\n- name: entra\n  source: openapi/azure-ai-foundry-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://ai.azure.com/.default)\nscopes:\n- scope: https://ai.azure.com/.default\n  description: Default Foundry inference scope\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-ai-foundry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/scopes/azure-ai-foundry-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Artificial Intelligence
- Generative AI
- AI Agents
- Foundation Models
- Machine Learning
- Cloud
- Azure
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
