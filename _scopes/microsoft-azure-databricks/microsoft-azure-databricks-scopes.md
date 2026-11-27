---
api_specs:
- filename: microsoft-azure-databricks-accessconnector-api-openapi.yml
  format: yaml
  label: Azure Databricks Access Connector API
  slug: microsoft-azure-databricks-accessconnector-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-accessconnector-api-openapi.yml
- filename: microsoft-azure-databricks-delete-api-openapi.yml
  format: yaml
  label: Azure Databricks DELETE API
  slug: microsoft-azure-databricks-delete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-delete-api-openapi.yml
- filename: microsoft-azure-databricks-operations-api-openapi.yml
  format: yaml
  label: Azure Databricks Operations API
  slug: microsoft-azure-databricks-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-operations-api-openapi.yml
- filename: microsoft-azure-databricks-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Databricks Private Link Resources API
  slug: microsoft-azure-databricks-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-privatelinkresources-api-openapi.yml
- filename: microsoft-azure-databricks-put-api-openapi.yml
  format: yaml
  label: Azure Databricks PUT API
  slug: microsoft-azure-databricks-put-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-put-api-openapi.yml
- filename: microsoft-azure-databricks-vnetpeering-api-openapi.yml
  format: yaml
  label: Azure Databricks V Net Peering API
  slug: microsoft-azure-databricks-vnetpeering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-vnetpeering-api-openapi.yml
- filename: microsoft-azure-databricks-workspaces-api-openapi.yml
  format: yaml
  label: Azure Databricks Workspaces API
  slug: microsoft-azure-databricks-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-workspaces-api-openapi.yml
- filename: microsoft-azure-databricks-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Databricks Private Endpoint Connections API
  slug: microsoft-azure-databricks-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-private-endpoint-connections-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Azure Databricks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Databricks publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Databricks API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Databricks
provider_slug: microsoft-azure-databricks
schemes:
- description: Azure Active Directory token for authenticating with Azure Databricks. Supports both user and service principal authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token
  name: AzureADToken
  source: openapi/_superseded/microsoft-azure-databricks-clusters-api-openapi.yml
- description: Azure Active Directory token for authenticating with Azure Databricks. Supports both user and service principal authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token
  name: AzureADToken
  source: openapi/_superseded/microsoft-azure-databricks-jobs-api-openapi.yml
- description: Azure Active Directory token for authenticating with Azure Databricks. Supports both user and service principal authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token
  name: AzureADToken
  source: openapi/_superseded/microsoft-azure-databricks-workspace-api-openapi.yml
scope_count: 1
scope_names:
- 2ff814a6-3304-4ab8-85cb-cd0e6f879c1d/.default
scopes:
- description: Access Azure Databricks workspace resources
  flows:
  - authorizationCode
  scope: 2ff814a6-3304-4ab8-85cb-cd0e6f879c1d/.default
slug: microsoft-azure-databricks-scopes
source_filename: microsoft-azure-databricks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-databricks-clusters-api-openapi.yml, openapi/_superseded/microsoft-azure-databricks-jobs-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-databricks-workspace-api-openapi.yml\nschemes:\n- name: AzureADToken\n  source: openapi/_superseded/microsoft-azure-databricks-clusters-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token\n  description: Azure Active Directory token for authenticating with Azure Databricks. Supports\n    both user and service principal authentication.\n- name: AzureADToken\n  source: openapi/_superseded/microsoft-azure-databricks-jobs-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token\n\
  \  description: Azure Active Directory token for authenticating with Azure Databricks. Supports\n    both user and service principal authentication.\n- name: AzureADToken\n  source: openapi/_superseded/microsoft-azure-databricks-workspace-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token\n  description: Azure Active Directory token for authenticating with Azure Databricks. Supports\n    both user and service principal authentication.\nscopes:\n- scope: 2ff814a6-3304-4ab8-85cb-cd0e6f879c1d/.default\n  description: Access Azure Databricks workspace resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/_superseded/microsoft-azure-databricks-clusters-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-databricks-jobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-databricks-workspace-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-databricks/scopes/microsoft-azure-databricks-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
token_bound: false
token_urls:
- https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token
---
