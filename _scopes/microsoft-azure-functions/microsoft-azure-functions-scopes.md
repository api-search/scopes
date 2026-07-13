---
api_specs:
- filename: azure-functions-management-api.json
  format: json
  label: Azure Functions Management API
  slug: azure-functions-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/openapi/azure-functions-management-api.json
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Functions Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure Functions publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure Functions API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-functions-management-api.json
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-functions-scopes
source_filename: microsoft-azure-functions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-functions-management-api.json\nschemes:\n- name: azure_auth\n  source: openapi/azure-functions-management-api.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-functions-management-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/scopes/microsoft-azure-functions-scopes.yml
summary_line: 1 scope · implicit
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
token_urls: []
---
