---
api_specs:
- filename: azure-cosmos-db-openapi.yml
  format: yaml
  label: Azure Cosmos DB Data Plane REST API
  slug: data-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Azure Cosmos Db Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Cosmos DB publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Cosmos DB API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Cosmos DB
provider_slug: azure-cosmos-db
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/azure-cosmos-db-openapi.yml
scope_count: 1
scope_names:
- https://cosmos.azure.com/.default
scopes:
- description: Cosmos DB data plane access
  flows:
  - clientCredentials
  scope: https://cosmos.azure.com/.default
slug: azure-cosmos-db-scopes
source_filename: azure-cosmos-db-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-cosmos-db-openapi.yml\nschemes:\n- name: entra\n  source: openapi/azure-cosmos-db-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\nscopes:\n- scope: https://cosmos.azure.com/.default\n  description: Cosmos DB data plane access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-cosmos-db-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/scopes/azure-cosmos-db-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Database
- NoSQL
- Document Database
- Vector Database
- Globally Distributed
- Cloud
- Azure
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
