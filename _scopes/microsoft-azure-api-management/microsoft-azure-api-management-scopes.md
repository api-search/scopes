---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Api Management Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure API Management publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure API Management API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-api-management-rest-api-openapi.yaml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-api-management-scopes
source_filename: microsoft-azure-api-management-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-api-management-rest-api-openapi.yaml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-api-management-rest-api-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-api-management-rest-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/scopes/microsoft-azure-api-management-scopes.yml
summary_line: 1 scope · implicit
tags:
- A2A
- AI Gateway
- API Center
- API Gateway
- API Management
- Enterprise
- MCP
- Microsoft Azure
token_urls: []
---
