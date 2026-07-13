---
api_specs:
- filename: synapse.json
  format: json
  label: Azure Synapse REST API
  slug: azure-synapse-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/synapse/resource-manager/Microsoft.Synapse/stable/2021-06-01/synapse.json
- filename: azure-synapse-openapi.yaml
  format: yaml
  label: Azure Synapse Pipeline API
  slug: azure-synapse-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/openapi/azure-synapse-openapi.yaml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Synapse Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Synapse Analytics publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Synapse Analytics API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Synapse Analytics
provider_slug: azure-synapse
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-synapse-openapi.yaml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-synapse-scopes
source_filename: azure-synapse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-synapse-openapi.yaml\nschemes:\n- name: azure_auth\n  source: openapi/azure-synapse-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscopes:\n- scope: user_impersonation\n  description: Impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-synapse-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/scopes/azure-synapse-scopes.yml
summary_line: 1 scope · implicit
tags:
- Analytics
- Apache Spark
- Big Data
- Data Warehouse
- ETL
- SQL
token_urls: []
---
