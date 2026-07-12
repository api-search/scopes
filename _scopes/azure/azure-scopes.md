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
name: Azure Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure
provider_slug: azure
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-management-openapi.yaml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-scopes
source_filename: azure-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-management-openapi.yaml\nschemes:\n- name: azure_auth\n  source: openapi/azure-management-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscopes:\n- scope: user_impersonation\n  description: Impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-management-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/scopes/azure-scopes.yml
summary_line: 1 scope · implicit
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Platform as a Service
- Storage
token_urls: []
---
