---
api_specs:
- filename: azure-health-collection-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Collection API
  slug: azure-health-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-collection-api-openapi.yml
- filename: azure-health-deid-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Deid API
  slug: azure-health-deid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-deid-api-openapi.yml
- filename: azure-health-dicomservices-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services DicomServices API
  slug: azure-health-dicomservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-dicomservices-api-openapi.yml
- filename: azure-health-fhirservices-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services FhirServices API
  slug: azure-health-fhirservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-fhirservices-api-openapi.yml
- filename: azure-health-iotconnectors-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services IotConnectors API
  slug: azure-health-iotconnectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-iotconnectors-api-openapi.yml
- filename: azure-health-jobs-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Jobs API
  slug: azure-health-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-jobs-api-openapi.yml
- filename: azure-health-privateendpointconnections-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services PrivateEndpointConnections API
  slug: azure-health-privateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-privateendpointconnections-api-openapi.yml
- filename: azure-health-privatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services PrivateLinkResources API
  slug: azure-health-privatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-privatelinkresources-api-openapi.yml
- filename: azure-health-proxy-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Proxy API
  slug: azure-health-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-proxy-api-openapi.yml
- filename: azure-health-resource-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Resource API
  slug: azure-health-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-resource-api-openapi.yml
- filename: azure-health-workspaceprivateendpointconnections-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services WorkspacePrivateEndpointConnections API
  slug: azure-health-workspaceprivateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-workspaceprivateendpointconnections-api-openapi.yml
- filename: azure-health-workspaceprivatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services WorkspacePrivateLinkResources API
  slug: azure-health-workspaceprivatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-workspaceprivatelinkresources-api-openapi.yml
- filename: azure-health-workspaces-api-openapi.yml
  format: yaml
  label: Microsoft Azure Health Data Services Workspaces API
  slug: azure-health-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-health/refs/heads/main/openapi/azure-health-workspaces-api-openapi.yml
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
