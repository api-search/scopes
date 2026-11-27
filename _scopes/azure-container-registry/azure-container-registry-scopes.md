---
api_specs:
- filename: azure-container-registry-registries-api-openapi.yml
  format: yaml
  label: Azure Container Registry Registries API
  slug: azure-container-registry-registries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-registries-api-openapi.yml
- filename: azure-container-registry-replications-api-openapi.yml
  format: yaml
  label: Azure Container Registry Replications API
  slug: azure-container-registry-replications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-replications-api-openapi.yml
- filename: azure-container-registry-webhooks-api-openapi.yml
  format: yaml
  label: Azure Container Registry Webhooks API
  slug: azure-container-registry-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-webhooks-api-openapi.yml
- filename: azure-container-registry-blobs-api-openapi.yml
  format: yaml
  label: Azure Container Registry Blobs API
  slug: microsoft-azure-container-registry-blobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-blobs-api-openapi.yml
- filename: azure-container-registry-manifests-api-openapi.yml
  format: yaml
  label: Azure Container Registry Manifests API
  slug: microsoft-azure-container-registry-manifests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-manifests-api-openapi.yml
- filename: azure-container-registry-acr-api-openapi.yml
  format: yaml
  label: Azure Container Registry Acr API
  slug: azure-container-registry-acr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-acr-api-openapi.yml
- filename: azure-container-registry-azure-container-registry-api-openapi.yml
  format: yaml
  label: Azure Container Registry Azure Container Registry API
  slug: azure-container-registry-azure-container-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-azure-container-registry-api-openapi.yml
- filename: azure-container-registry-cacherules-api-openapi.yml
  format: yaml
  label: Azure Container Registry Cache Rules API
  slug: azure-container-registry-cacherules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-cacherules-api-openapi.yml
- filename: azure-container-registry-connectedregistries-api-openapi.yml
  format: yaml
  label: Azure Container Registry Connected Registries API
  slug: azure-container-registry-connectedregistries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-connectedregistries-api-openapi.yml
- filename: azure-container-registry-credentialsets-api-openapi.yml
  format: yaml
  label: Azure Container Registry Credential Sets API
  slug: azure-container-registry-credentialsets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-credentialsets-api-openapi.yml
- filename: azure-container-registry-oauth2-api-openapi.yml
  format: yaml
  label: Azure Container Registry Oauth2 API
  slug: azure-container-registry-oauth2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-oauth2-api-openapi.yml
- filename: azure-container-registry-operations-api-openapi.yml
  format: yaml
  label: Azure Container Registry Operations API
  slug: azure-container-registry-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-operations-api-openapi.yml
- filename: azure-container-registry-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Container Registry Private Link Resources API
  slug: azure-container-registry-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-privatelinkresources-api-openapi.yml
- filename: azure-container-registry-runs-api-openapi.yml
  format: yaml
  label: Azure Container Registry Runs API
  slug: azure-container-registry-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-runs-api-openapi.yml
- filename: azure-container-registry-scopemaps-api-openapi.yml
  format: yaml
  label: Azure Container Registry Scope Maps API
  slug: azure-container-registry-scopemaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-scopemaps-api-openapi.yml
- filename: azure-container-registry-tasks-api-openapi.yml
  format: yaml
  label: Azure Container Registry Tasks API
  slug: azure-container-registry-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-tasks-api-openapi.yml
- filename: azure-container-registry-tokens-api-openapi.yml
  format: yaml
  label: Azure Container Registry Tokens API
  slug: azure-container-registry-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-tokens-api-openapi.yml
- filename: azure-container-registry-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Container Registry Private Endpoint Connections API
  slug: azure-container-registry-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-registry/openapi/azure-container-registry-private-endpoint-connections-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Container Registry Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Container Registry publishes 2 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Container Registry API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: OAuth2Auth
  source: openapi/azure-container-registry-data-plane-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-container-registry-management-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-container-registry-operation-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/azure-container-registry-registries-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/azure-container-registry-replications-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/azure-container-registry-webhooks-api-openapi.yml
scope_count: 2
scope_names:
- https://containerregistry.azure.net/.default
- user_impersonation
scopes:
- description: ''
  flows:
  - implicit
  scope: https://containerregistry.azure.net/.default
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-container-registry-scopes
source_filename: azure-container-registry-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/azure-container-registry-data-plane-api-openapi.yml, openapi/azure-container-registry-management-api-openapi.yml,\n  openapi/azure-container-registry-operation-api-openapi.yml, openapi/_superseded/azure-container-registry-registries-api-openapi.yml,\n  openapi/_superseded/azure-container-registry-replications-api-openapi.yml, openapi/_superseded/azure-container-registry-webhooks-api-openapi.yml\nschemes:\n- name: OAuth2Auth\n  source: openapi/azure-container-registry-data-plane-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: azure_auth\n  source: openapi/azure-container-registry-management-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-container-registry-operation-api-openapi.yml\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/_superseded/azure-container-registry-registries-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/_superseded/azure-container-registry-replications-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/_superseded/azure-container-registry-webhooks-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: https://containerregistry.azure.net/.default\n\
  \  flows:\n  - implicit\n  sources:\n  - openapi/azure-container-registry-data-plane-api-openapi.yml\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-container-registry-management-api-openapi.yml\n  - openapi/azure-container-registry-operation-api-openapi.yml\n  - openapi/_superseded/azure-container-registry-registries-api-openapi.yml\n  - openapi/_superseded/azure-container-registry-replications-api-openapi.yml\n  - openapi/_superseded/azure-container-registry-webhooks-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/azure-container-registry/scopes/azure-container-registry-scopes.yml
summary_line: 2 scopes · implicit
tags:
- Microsoft Azure
- Container Images
- Containers
- Docker
- Registry
token_bound: false
token_urls: []
---
