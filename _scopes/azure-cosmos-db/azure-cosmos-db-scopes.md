---
api_specs:
- filename: azure-cosmos-db-datatransfer-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Data Transfer API
  slug: azure-cosmos-db-datatransfer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-datatransfer-api-openapi.yml
- filename: azure-cosmos-db-fleets-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Fleets API
  slug: azure-cosmos-db-fleets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-fleets-api-openapi.yml
- filename: azure-cosmos-db-graphapicompute-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Graph API Compute API
  slug: azure-cosmos-db-graphapicompute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-graphapicompute-api-openapi.yml
- filename: azure-cosmos-db-materializedviewsbuilder-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Materialized Views Builder API
  slug: azure-cosmos-db-materializedviewsbuilder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-materializedviewsbuilder-api-openapi.yml
- filename: azure-cosmos-db-notebookworkspacesresource-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Notebook Workspaces Resource API
  slug: azure-cosmos-db-notebookworkspacesresource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-notebookworkspacesresource-api-openapi.yml
- filename: azure-cosmos-db-operations-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Operations API
  slug: azure-cosmos-db-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-operations-api-openapi.yml
- filename: azure-cosmos-db-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Private Link Resources API
  slug: azure-cosmos-db-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-privatelinkresources-api-openapi.yml
- filename: azure-cosmos-db-providers-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Providers API
  slug: azure-cosmos-db-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-providers-api-openapi.yml
- filename: azure-cosmos-db-sqldedicatedgateway-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Sql Dedicated Gateway API
  slug: azure-cosmos-db-sqldedicatedgateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-sqldedicatedgateway-api-openapi.yml
- filename: azure-cosmos-db-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Subscriptions API
  slug: azure-cosmos-db-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-subscriptions-api-openapi.yml
- filename: azure-cosmos-db-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Private Endpoint Connections API
  slug: azure-cosmos-db-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-private-endpoint-connections-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Cosmos DB Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Cosmos DB publishes 2 OAuth 2.0 scopes via the clientCredentials and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Cosmos DB API on a user''s behalf.


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
  source: openapi/_superseded/azure-cosmos-db-collections-api-openapi.yml
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/azure-cosmos-db-databases-api-openapi.yml
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/azure-cosmos-db-documents-api-openapi.yml
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/azure-cosmos-db-offers-api-openapi.yml
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/azure-cosmos-db-permissions-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-cosmos-db-resource-provider-openapi.yml
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/azure-cosmos-db-stored-procedures-api-openapi.yml
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/azure-cosmos-db-triggers-api-openapi.yml
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/azure-cosmos-db-user-defined-functions-api-openapi.yml
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/_superseded/azure-cosmos-db-users-api-openapi.yml
scope_count: 2
scope_names:
- https://cosmos.azure.com/.default
- user_impersonation
scopes:
- description: Cosmos DB data plane access
  flows:
  - clientCredentials
  scope: https://cosmos.azure.com/.default
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-cosmos-db-scopes
source_filename: azure-cosmos-db-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/azure-cosmos-db-collections-api-openapi.yml, openapi/_superseded/azure-cosmos-db-databases-api-openapi.yml,\n  openapi/_superseded/azure-cosmos-db-documents-api-openapi.yml, openapi/_superseded/azure-cosmos-db-offers-api-openapi.yml,\n  openapi/_superseded/azure-cosmos-db-permissions-api-openapi.yml, openapi/azure-cosmos-db-resource-provider-openapi.yml,\n  openapi/_superseded/azure-cosmos-db-stored-procedures-api-openapi.yml, openapi/_superseded/azure-cosmos-db-triggers-api-openapi.yml,\n  openapi/_superseded/azure-cosmos-db-user-defined-functions-api-openapi.yml, openapi/_superseded/azure-cosmos-db-users-api-openapi.yml\nschemes:\n- name: entra\n  source: openapi/_superseded/azure-cosmos-db-collections-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n- name: entra\n\
  \  source: openapi/_superseded/azure-cosmos-db-databases-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n- name: entra\n  source: openapi/_superseded/azure-cosmos-db-documents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n- name: entra\n  source: openapi/_superseded/azure-cosmos-db-offers-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n- name: entra\n  source: openapi/_superseded/azure-cosmos-db-permissions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth\
  \ 2.0 bearer token\n- name: azure_auth\n  source: openapi/azure-cosmos-db-resource-provider-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: entra\n  source: openapi/_superseded/azure-cosmos-db-stored-procedures-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n- name: entra\n  source: openapi/_superseded/azure-cosmos-db-triggers-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n- name: entra\n  source: openapi/_superseded/azure-cosmos-db-user-defined-functions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n\
  \  description: Microsoft Entra ID OAuth 2.0 bearer token\n- name: entra\n  source: openapi/_superseded/azure-cosmos-db-users-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\nscopes:\n- scope: https://cosmos.azure.com/.default\n  description: Cosmos DB data plane access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/_superseded/azure-cosmos-db-collections-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-databases-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-documents-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-offers-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-permissions-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-stored-procedures-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-triggers-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-user-defined-functions-api-openapi.yml\n\
  \  - openapi/_superseded/azure-cosmos-db-users-api-openapi.yml\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-cosmos-db-resource-provider-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/azure-cosmos-db/scopes/azure-cosmos-db-scopes.yml
summary_line: 2 scopes · clientCredentials/implicit
tags:
- Database
- NoSQL
- Document Database
- Vector Search
- Globally Distributed
- Cloud
- Microsoft Azure
token_bound: false
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
