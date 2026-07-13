---
api_specs:
- filename: azure-quantum-data-plane-openapi.json
  format: json
  label: Azure Quantum Workspace Data-Plane API
  slug: azure-quantum-workspace-data-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-quantum/refs/heads/main/openapi/azure-quantum-data-plane-openapi.json
- filename: azure-quantum-resource-manager-openapi.json
  format: json
  label: Azure Quantum Resource Manager API
  slug: azure-quantum-resource-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-quantum/refs/heads/main/openapi/azure-quantum-resource-manager-openapi.json
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Quantum Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure Quantum publishes 2 OAuth 2.0 scopes via the clientCredentials and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure Quantum API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure Quantum
provider_slug: microsoft-quantum
schemes:
- description: Azure Entra OAuth2 Authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: AzureEntraAuth
  source: openapi/azure-quantum-data-plane-openapi.json
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-quantum-resource-manager-openapi.json
scope_count: 2
scope_names:
- https://quantum.microsoft.com/.default
- user_impersonation
scopes:
- description: ''
  flows:
  - clientCredentials
  scope: https://quantum.microsoft.com/.default
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-quantum-scopes
source_filename: microsoft-quantum-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-quantum-data-plane-openapi.json, openapi/azure-quantum-resource-manager-openapi.json\nschemes:\n- name: AzureEntraAuth\n  source: openapi/azure-quantum-data-plane-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Azure Entra OAuth2 Authentication\n- name: azure_auth\n  source: openapi/azure-quantum-resource-manager-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: https://quantum.microsoft.com/.default\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-quantum-data-plane-openapi.json\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-quantum-resource-manager-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-quantum/refs/heads/main/scopes/microsoft-quantum-scopes.yml
summary_line: 2 scopes · clientCredentials/implicit
tags:
- Quantum
- Quantum Computing
- Azure
- Microsoft
- Q#
- QDK
- Resource Estimation
- IonQ
- Quantinuum
- Pasqal
- Rigetti
- Hybrid Quantum
- Fault Tolerance
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
