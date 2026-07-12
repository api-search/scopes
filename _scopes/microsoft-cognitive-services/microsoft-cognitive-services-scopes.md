---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Cognitive Services Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Cognitive Services publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Cognitive Services API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Cognitive Services
provider_slug: microsoft-cognitive-services
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: azure_auth
  source: openapi/microsoft-cognitive-services-openapi.yml
scope_count: 1
scope_names:
- https://cognitiveservices.azure.com/.default
scopes:
- description: Cognitive Services access
  flows:
  - clientCredentials
  scope: https://cognitiveservices.azure.com/.default
slug: microsoft-cognitive-services-scopes
source_filename: microsoft-cognitive-services-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-cognitive-services-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-cognitive-services-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\nscopes:\n- scope: https://cognitiveservices.azure.com/.default\n  description: Cognitive Services access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-cognitive-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-cognitive-services/refs/heads/main/scopes/microsoft-cognitive-services-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Azure AI
- Computer Vision
- Speech
- NLP
- OpenAI
- Machine Learning
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
