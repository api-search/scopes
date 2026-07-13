---
api_specs:
- filename: azure-kubernetes-service-openapi.yml
  format: yaml
  label: Azure Kubernetes Service REST API
  slug: azure-kubernetes-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/openapi/azure-kubernetes-service-openapi.yml
- filename: azure-kubernetes-service-openapi.yml
  format: yaml
  label: Azure Kubernetes Service Managed Clusters API
  slug: azure-kubernetes-service-managed-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/openapi/azure-kubernetes-service-openapi.yml
- filename: azure-kubernetes-service-openapi.yml
  format: yaml
  label: Azure Kubernetes Service Agent Pools API
  slug: azure-kubernetes-service-agent-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/openapi/azure-kubernetes-service-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Kubernetes Service Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Kubernetes Service publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Kubernetes Service API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-kubernetes-service-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-kubernetes-service-scopes
source_filename: azure-kubernetes-service-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-kubernetes-service-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/azure-kubernetes-service-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: Impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-kubernetes-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/scopes/azure-kubernetes-service-scopes.yml
summary_line: 1 scope · implicit
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
token_urls: []
---
