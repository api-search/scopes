---
api_specs:
- filename: azure-storage-account-blobcontainers-api-openapi.yml
  format: yaml
  label: Azure Storage Account BlobContainers API
  slug: azure-storage-account-blobcontainers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-blobcontainers-api-openapi.yml
- filename: azure-storage-account-blobservice-api-openapi.yml
  format: yaml
  label: Azure Storage Account BlobService API
  slug: azure-storage-account-blobservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-blobservice-api-openapi.yml
- filename: azure-storage-account-locationusage-api-openapi.yml
  format: yaml
  label: Azure Storage Account LocationUsage API
  slug: azure-storage-account-locationusage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-locationusage-api-openapi.yml
- filename: azure-storage-account-managementpolicies-api-openapi.yml
  format: yaml
  label: Azure Storage Account ManagementPolicies API
  slug: azure-storage-account-managementpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-managementpolicies-api-openapi.yml
- filename: azure-storage-account-operations-api-openapi.yml
  format: yaml
  label: Azure Storage Account Operations API
  slug: azure-storage-account-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-operations-api-openapi.yml
- filename: azure-storage-account-privateendpointconnections-api-openapi.yml
  format: yaml
  label: Azure Storage Account PrivateEndpointConnections API
  slug: azure-storage-account-privateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-privateendpointconnections-api-openapi.yml
- filename: azure-storage-account-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Storage Account PrivateLinkResources API
  slug: azure-storage-account-privatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-privatelinkresources-api-openapi.yml
- filename: azure-storage-account-skus-api-openapi.yml
  format: yaml
  label: Azure Storage Account Skus API
  slug: azure-storage-account-skus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-skus-api-openapi.yml
- filename: azure-storage-account-storageaccounts-api-openapi.yml
  format: yaml
  label: Azure Storage Account StorageAccounts API
  slug: azure-storage-account-storageaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-storageaccounts-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Storage Account Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Storage Account publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Storage Account API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-storage-account-blob-openapi.yaml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-storage-account-management-openapi.yaml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-storage-account-scopes
source_filename: azure-storage-account-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-storage-account-blob-openapi.yaml, openapi/azure-storage-account-management-openapi.yaml\nschemes:\n- name: azure_auth\n  source: openapi/azure-storage-account-blob-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/azure-storage-account-management-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-storage-account-blob-openapi.yaml\n  - openapi/azure-storage-account-management-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/scopes/azure-storage-account-scopes.yml
summary_line: 1 scope · implicit
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
token_urls: []
---
