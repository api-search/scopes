---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Azure Document Intelligence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure AI Document Intelligence publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure AI Document Intelligence API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure AI Document Intelligence
provider_slug: azure-document-intelligence
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: OAuth2Auth
  source: openapi/azure-document-intelligence-openapi.json
scope_count: 1
scope_names:
- https://cognitiveservices.azure.com/.default
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: https://cognitiveservices.azure.com/.default
slug: azure-document-intelligence-scopes
source_filename: azure-document-intelligence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-document-intelligence-openapi.json\nschemes:\n- name: OAuth2Auth\n  source: openapi/azure-document-intelligence-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\nscopes:\n- scope: https://cognitiveservices.azure.com/.default\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-document-intelligence-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-document-intelligence/refs/heads/main/scopes/azure-document-intelligence-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- AI
- Document AI
- Azure
- IDP
- OCR
- Microsoft
- REST
token_urls:
- https://login.microsoftonline.com/common/oauth2/token
---
