---
api_specs:
- filename: microsoft-azure-cdn-management-openapi.json
  format: json
  label: Azure CDN Management API (Microsoft.Cdn)
  slug: microsoft-azure-cdn-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cdn/refs/heads/main/openapi/microsoft-azure-cdn-management-openapi.json
- filename: microsoft-azure-cdn-operations-api-openapi.yml
  format: yaml
  label: microsoft-azure-cdn Operations API
  slug: microsoft-azure-cdn-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cdn/refs/heads/main/openapi/microsoft-azure-cdn-operations-api-openapi.yml
- filename: microsoft-azure-cdn-profiles-api-openapi.yml
  format: yaml
  label: microsoft-azure-cdn Profiles API
  slug: microsoft-azure-cdn-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cdn/refs/heads/main/openapi/microsoft-azure-cdn-profiles-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles/networking
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Azure Cdn Scopes
name_suffix: OAuth Scopes
note: 'Two different things are called a "scope" on this API and conflating them is the usual integration mistake. (1) The OAUTH SCOPE is coarse: the contract declares exactly one, user_impersonation, and the real-world token request asks for https://management.azure.com/.default — neither expresses what the caller may do. (2) The AUTHORIZATION SCOPE is an Azure RBAC role assigned at an ARM resource scope, and that is what actually gates each of the 115 operations. Both are recorded below; the RBAC block is the one that matters.'
overview: 'Microsoft Azure Cdn publishes 2 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure Cdn API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure Cdn
provider_slug: microsoft-azure-cdn
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-cdn-management-openapi.json
scope_count: 2
scope_names:
- user_impersonation
- https://management.azure.com/.default
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
- description: The resource scope a service principal or managed identity requests for any Azure Resource Manager call, Microsoft.Cdn included. Documented by Microsoft, not declared in the contract.
  flows:
  - client_credentials
  scope: https://management.azure.com/.default
slug: microsoft-azure-cdn-scopes
source_filename: microsoft-azure-cdn-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  openapi/microsoft-azure-cdn-management-openapi.json,\n  https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles/networking\ndocs: https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles/networking\nprovider: microsoft-azure-cdn\nnote: >-\n  Two different things are called a \"scope\" on this API and conflating them is the usual integration\n  mistake. (1) The OAUTH SCOPE is coarse: the contract declares exactly one, user_impersonation, and\n  the real-world token request asks for https://management.azure.com/.default — neither expresses what\n  the caller may do. (2) The AUTHORIZATION SCOPE is an Azure RBAC role assigned at an ARM resource\n  scope, and that is what actually gates each of the 115 operations. Both are recorded below; the RBAC\n  block is the one that matters.\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-cdn-management-openapi.json\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  declared_in: contract\n  sources:\n  - openapi/microsoft-azure-cdn-management-openapi.json\n- scope: https://management.azure.com/.default\n  description: >-\n    The resource scope a service principal or managed identity requests for any Azure Resource Manager\n    call, Microsoft.Cdn included. Documented by Microsoft, not declared in the contract.\n  flows:\n  - client_credentials\n  declared_in: docs\nrbac_roles:\n- role: CDN Profile Contributor\n  id: ec156ff8-a8d1-4d15-830c-5b80698ca432\n  description: Can manage CDN profiles and their endpoints, but can't grant access to other users.\n  grants: [Microsoft.Cdn/*]\n- role: CDN Profile Reader\n  id: 8f96442b-4075-438f-813d-ad51ab4019af\n  description: Can view CDN\
  \ profiles and their endpoints, but can't make changes.\n  grants: [Microsoft.Cdn/*/read]\n- role: CDN Endpoint Contributor\n  id: 426e0c7f-0c7e-4658-b36f-ff54d6c29b45\n  description: Can manage CDN endpoints, but can't grant access to other users.\n  grants:\n  - Microsoft.Cdn/edgenodes/read\n  - Microsoft.Cdn/operationresults/*\n  - Microsoft.Cdn/profiles/endpoints/*\n- role: CDN Endpoint Reader\n  id: 871e35f6-b5c1-49cc-a043-bde969a0f2cd\n  description: Can view CDN endpoints, but can't make changes.\n  grants:\n  - Microsoft.Cdn/edgenodes/read\n  - Microsoft.Cdn/operationresults/*\n  - Microsoft.Cdn/profiles/endpoints/*/read\n  - Microsoft.Cdn/profiles/afdendpoints/validateCustomDomain/action\nassignable_scopes:\n- /subscriptions/{subscriptionId}\n- /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}\n- /subscriptions/{subscriptionId}/resourceGroups/{rg}/providers/Microsoft.Cdn/profiles/{profileName}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cdn/refs/heads/main/scopes/microsoft-azure-cdn-scopes.yml
summary_line: 2 scopes · implicit
tags:
- CDN
- Edge
- Caching
- Cloud Infrastructure
- Networking
- Web Performance
- Azure
- Content Delivery
- Web Application Firewall
token_urls: []
---
