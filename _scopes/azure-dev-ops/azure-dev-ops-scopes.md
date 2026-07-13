---
api_specs:
- filename: azure-dev-ops-openapi.yaml
  format: yaml
  label: Azure DevOps REST API
  slug: azure-devops-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/openapi/azure-dev-ops-openapi.yaml
- filename: azure-dev-ops-openapi.yaml
  format: yaml
  label: Azure DevOps Pipelines API
  slug: azure-devops-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/openapi/azure-dev-ops-openapi.yaml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Dev Ops Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure DevOps publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure DevOps API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-dev-ops-openapi.yaml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-dev-ops-scopes
source_filename: azure-dev-ops-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-dev-ops-openapi.yaml\nschemes:\n- name: azure_auth\n  source: openapi/azure-dev-ops-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-dev-ops-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/scopes/azure-dev-ops-scopes.yml
summary_line: 1 scope · implicit
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
token_urls: []
---
