---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Azure Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure Cloud publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure Cloud API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure Cloud
provider_slug: azure-cloud
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://management.azure.com/.default)
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/azure-cloud-openapi.yml
scope_count: 1
scope_names:
- https://management.azure.com/.default
scopes:
- description: Manage Azure resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: https://management.azure.com/.default
slug: azure-cloud-scopes
source_filename: azure-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-cloud-openapi.yml\nschemes:\n- name: entra\n  source: openapi/azure-cloud-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://management.azure.com/.default)\nscopes:\n- scope: https://management.azure.com/.default\n  description: Manage Azure resources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/azure-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-cloud/refs/heads/main/scopes/azure-cloud-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- AI
- Cloud Computing
- Databases
- IaaS
- Infrastructure
- Machine Learning
- Microsoft
- Networking
- PaaS
- Platform as a Service
- SaaS
- Storage
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
