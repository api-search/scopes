---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure Health Data Services publishes 2 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure Health Data Services API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure Health Data Services
provider_slug: azure-health
schemes:
- description: The Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: AadToken
  source: openapi/health-data-ai-deid-2024-11-15.json
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/healthcare-apis-2024-03-31.json
scope_count: 2
scope_names:
- https://deid.azure.com/.default
- user_impersonation
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: https://deid.azure.com/.default
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-health-scopes
source_filename: azure-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/health-data-ai-deid-2024-11-15.json, openapi/healthcare-apis-2024-03-31.json\nschemes:\n- name: AadToken\n  source: openapi/health-data-ai-deid-2024-11-15.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n  description: The Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/healthcare-apis-2024-03-31.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: https://deid.azure.com/.default\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/health-data-ai-deid-2024-11-15.json\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/healthcare-apis-2024-03-31.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/scopes/azure-health-scopes.yml
summary_line: 2 scopes · authorizationCode/implicit
tags:
- Healthcare
- FHIR
- DICOM
- MedTech
- IoMT
- Health Data
- HIPAA
- HITRUST
- Cloud
- Azure
- Microsoft
token_urls:
- https://login.microsoftonline.com/common/oauth2/token
---
