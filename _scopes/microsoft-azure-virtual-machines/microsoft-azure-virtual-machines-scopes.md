---
api_specs:
- filename: virtualMachines.json
  format: json
  label: Azure Virtual Machines REST API
  slug: azure-virtual-machines-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/compute/resource-manager/Microsoft.Compute/ComputeRP/stable/2023-09-01/virtualMachines.json
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Virtual Machines Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Virtual Machines publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Virtual Machines API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Virtual Machines
provider_slug: microsoft-azure-virtual-machines
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: OAuth2Auth
  source: openapi/azure-virtual-machines-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-virtual-machines-scopes
source_filename: microsoft-azure-virtual-machines-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-virtual-machines-openapi.yml\nschemes:\n- name: OAuth2Auth\n  source: openapi/azure-virtual-machines-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-virtual-machines-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-virtual-machines/refs/heads/main/scopes/microsoft-azure-virtual-machines-scopes.yml
summary_line: 1 scope · implicit
tags:
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
token_urls: []
---
