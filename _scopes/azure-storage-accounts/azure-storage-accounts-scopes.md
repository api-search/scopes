---
api_specs:
- filename: azure-storage-accounts-blobcontainers-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts BlobContainers API
  slug: azure-storage-accounts-blobcontainers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-blobcontainers-api-openapi.yml
- filename: azure-storage-accounts-blobservice-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts BlobService API
  slug: azure-storage-accounts-blobservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-blobservice-api-openapi.yml
- filename: azure-storage-accounts-locationusage-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts LocationUsage API
  slug: azure-storage-accounts-locationusage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-locationusage-api-openapi.yml
- filename: azure-storage-accounts-managementpolicies-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts ManagementPolicies API
  slug: azure-storage-accounts-managementpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-managementpolicies-api-openapi.yml
- filename: azure-storage-accounts-operations-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts Operations API
  slug: azure-storage-accounts-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-operations-api-openapi.yml
- filename: azure-storage-accounts-privateendpointconnections-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts PrivateEndpointConnections API
  slug: azure-storage-accounts-privateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-privateendpointconnections-api-openapi.yml
- filename: azure-storage-accounts-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts PrivateLinkResources API
  slug: azure-storage-accounts-privatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-privatelinkresources-api-openapi.yml
- filename: azure-storage-accounts-skus-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts Skus API
  slug: azure-storage-accounts-skus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-skus-api-openapi.yml
- filename: azure-storage-accounts-storageaccounts-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts StorageAccounts API
  slug: azure-storage-accounts-storageaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-storageaccounts-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Storage Accounts Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Storage Accounts publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Storage Accounts API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-storage-accounts-blob-openapi.yaml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-storage-accounts-management-openapi.yaml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-storage-accounts-scopes
source_filename: azure-storage-accounts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-storage-accounts-blob-openapi.yaml, openapi/azure-storage-accounts-management-openapi.yaml\nschemes:\n- name: azure_auth\n  source: openapi/azure-storage-accounts-blob-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/azure-storage-accounts-management-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-storage-accounts-blob-openapi.yaml\n  - openapi/azure-storage-accounts-management-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/scopes/azure-storage-accounts-scopes.yml
summary_line: 1 scope · implicit
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
token_urls: []
---
