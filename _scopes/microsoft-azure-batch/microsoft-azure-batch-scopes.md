---
api_specs:
- filename: microsoft-azure-batch-batch-service-openapi.json
  format: json
  label: Azure Batch Service API
  slug: microsoft-azure-batch-batch-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/_original/microsoft-azure-batch-batch-service-openapi.json
- filename: microsoft-azure-batch-management-openapi.json
  format: json
  label: Azure Batch Management API
  slug: microsoft-azure-batch-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/_original/microsoft-azure-batch-management-openapi.json
- filename: microsoft-azure-batch-jobs-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Jobs API
  slug: microsoft-azure-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-jobs-api-openapi.yml
- filename: microsoft-azure-batch-pools-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Pools API
  slug: microsoft-azure-batch-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-pools-api-openapi.yml
- filename: microsoft-azure-batch-tasks-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Tasks API
  slug: microsoft-azure-batch-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-tasks-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: https://learn.microsoft.com/en-us/azure/batch/batch-aad-auth
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Azure Batch Scopes
name_suffix: OAuth Scopes
note: Azure Batch does NOT publish a granular OAuth scope surface. Both planes declare a single coarse scope and then delegate real authorization to Azure RBAC role assignments on the Batch account resource. An agent asking "which scope do I need for Jobs_DeleteJob" has no scope-level answer here — the answer is a role assignment. Recorded honestly rather than fabricating a per-operation scope map.
overview: 'Microsoft Azure Batch publishes 2 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure Batch API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure Batch
provider_slug: microsoft-azure-batch
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: implicit
  name: OAuth2Auth
  plane: data
  source: openapi/_original/microsoft-azure-batch-batch-service-openapi.json
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  plane: management
  source: openapi/_original/microsoft-azure-batch-management-openapi.json
scope_count: 2
scope_names:
- https://batch.core.windows.net//.default
- user_impersonation
scopes:
- description: Resource-wide .default scope for the Batch data plane. Grants whatever the calling identity's Azure RBAC role assignments on the Batch account already allow — it does not itself narrow access. Applied to all 72 data-plane operations.
  flows:
  - implicit
  - client_credentials
  scope: https://batch.core.windows.net//.default
- description: '"impersonate your user account" — the standard ARM delegated scope, applied to all 42 management-plane operations against management.azure.com.'
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-batch-scopes
source_filename: microsoft-azure-batch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/_original/microsoft-azure-batch-batch-service-openapi.json\ndocs: https://learn.microsoft.com/en-us/azure/batch/batch-aad-auth\nnote: >-\n  Azure Batch does NOT publish a granular OAuth scope surface. Both planes declare a\n  single coarse scope and then delegate real authorization to Azure RBAC role\n  assignments on the Batch account resource. An agent asking \"which scope do I need for\n  Jobs_DeleteJob\" has no scope-level answer here — the answer is a role assignment.\n  Recorded honestly rather than fabricating a per-operation scope map.\nscheme_count: 2\nschemes:\n  - name: OAuth2Auth\n    plane: data\n    source: openapi/_original/microsoft-azure-batch-batch-service-openapi.json\n    flows:\n      - flow: implicit\n        authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n  - name: azure_auth\n    plane: management\n    source: openapi/_original/microsoft-azure-batch-management-openapi.json\n\
  \    flows:\n      - flow: implicit\n        authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscope_count: 2\nscopes:\n  - scope: https://batch.core.windows.net//.default\n    plane: data\n    description: >-\n      Resource-wide .default scope for the Batch data plane. Grants whatever the calling\n      identity's Azure RBAC role assignments on the Batch account already allow — it does\n      not itself narrow access. Applied to all 72 data-plane operations.\n    flows:\n      - implicit\n      - client_credentials\n    applies_to: all data-plane operations\n    sources:\n      - openapi/_original/microsoft-azure-batch-batch-service-openapi.json\n  - scope: user_impersonation\n    plane: management\n    description: >-\n      \"impersonate your user account\" — the standard ARM delegated scope, applied to all\n      42 management-plane operations against management.azure.com.\n    flows:\n      - implicit\n    applies_to: all management-plane operations\n \
  \   sources:\n      - openapi/_original/microsoft-azure-batch-management-openapi.json\nauthorization_model:\n  mechanism: Azure RBAC\n  description: >-\n    Effective permission is decided by role assignment scope (subscription / resource\n    group / Batch account), not by token scope. Microsoft publishes Batch built-in roles\n    and the full Microsoft.Batch/* action list through the Azure role definitions surface.\n  docs: https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/scopes/microsoft-azure-batch-scopes.yml
summary_line: 2 scopes · implicit
tags:
- Batch
- Compute
- Job Scheduling
- High Performance Computing
- Cloud
- Microsoft
- Azure
- Parallel Processing
- Scheduling
- Infrastructure
token_urls: []
---
