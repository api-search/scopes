---
api_specs:
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Azure Databricks REST API
  slug: azure-databricks-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Clusters API
  slug: clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Jobs API
  slug: jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Workspace API
  slug: workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
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
provider_slug: azure-databricks
schemes:
- description: Azure Active Directory token for authenticating with Azure Databricks. Supports both user and service principal authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token
  name: AzureADToken
  source: openapi/azure-databricks-openapi.yml
scope_count: 1
scope_names:
- 2ff814a6-3304-4ab8-85cb-cd0e6f879c1d/.default
scopes:
- description: Access Azure Databricks workspace resources
  flows:
  - authorizationCode
  scope: 2ff814a6-3304-4ab8-85cb-cd0e6f879c1d/.default
slug: azure-databricks-scopes
source_filename: azure-databricks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-databricks-openapi.yml\nschemes:\n- name: AzureADToken\n  source: openapi/azure-databricks-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token\n  description: Azure Active Directory token for authenticating with Azure Databricks. Supports\n    both user and service principal authentication.\nscopes:\n- scope: 2ff814a6-3304-4ab8-85cb-cd0e6f879c1d/.default\n  description: Access Azure Databricks workspace resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/azure-databricks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/scopes/azure-databricks-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
token_urls:
- https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token
---
