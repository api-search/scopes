---
api_specs:
- filename: blob.json
  format: json
  label: Azure Blob Storage API
  slug: azure-blob-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/storage/data-plane/Microsoft.BlobStorage/stable/2021-12-02/blob.json
- filename: azure-storage-account-management-openapi.yaml
  format: yaml
  label: Azure Queue Storage API
  slug: azure-queue-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-management-openapi.yaml
- filename: azure-storage-account-management-openapi.yaml
  format: yaml
  label: Azure Table Storage API
  slug: azure-table-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-management-openapi.yaml
- filename: azure-storage-account-management-openapi.yaml
  format: yaml
  label: Azure File Storage API
  slug: azure-file-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/openapi/azure-storage-account-management-openapi.yaml
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
