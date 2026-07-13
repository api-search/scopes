---
api_specs:
- filename: microsoft-azure-batch-openapi.yml
  format: yaml
  label: Azure Batch REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Batch Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'microsoft-azure-batch publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the microsoft-azure-batch API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: microsoft-azure-batch
provider_slug: microsoft-azure-batch
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-batch-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Impersonate user
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-batch-scopes
source_filename: microsoft-azure-batch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-batch-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-batch-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscopes:\n- scope: user_impersonation\n  description: Impersonate user\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-batch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/scopes/microsoft-azure-batch-scopes.yml
summary_line: 1 scope · implicit
tags: []
token_urls: []
---
