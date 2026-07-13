---
api_specs:
- filename: azure-file-storage-openapi.yml
  format: yaml
  label: Azure Files FileREST API
  slug: filerest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-file-storage/refs/heads/main/openapi/azure-file-storage-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Azure File Storage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Files publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Files API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Files
provider_slug: azure-file-storage
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/azure-file-storage-openapi.yml
scope_count: 1
scope_names:
- https://storage.azure.com/.default
scopes:
- description: Azure Storage data plane access
  flows:
  - clientCredentials
  scope: https://storage.azure.com/.default
slug: azure-file-storage-scopes
source_filename: azure-file-storage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-file-storage-openapi.yml\nschemes:\n- name: entra\n  source: openapi/azure-file-storage-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\nscopes:\n- scope: https://storage.azure.com/.default\n  description: Azure Storage data plane access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-file-storage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-file-storage/refs/heads/main/scopes/azure-file-storage-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Storage
- File Storage
- File Shares
- SMB
- NFS
- Cloud
- Azure
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
