---
api_specs:
- filename: microsoft-azure-sql-database-databases-api-openapi.yml
  format: yaml
  label: Azure SQL Database Databases API
  slug: microsoft-azure-sql-database-databases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-databases-api-openapi.yml
- filename: microsoft-azure-sql-database-elasticpools-api-openapi.yml
  format: yaml
  label: Azure SQL Database ElasticPools API
  slug: microsoft-azure-sql-database-elasticpools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml
- filename: microsoft-azure-sql-database-failovergroups-api-openapi.yml
  format: yaml
  label: Azure SQL Database FailoverGroups API
  slug: microsoft-azure-sql-database-failovergroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml
- filename: microsoft-azure-sql-database-servers-api-openapi.yml
  format: yaml
  label: Azure SQL Database Servers API
  slug: microsoft-azure-sql-database-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-servers-api-openapi.yml
- filename: microsoft-azure-sql-database-firewall-rules-api-openapi.yml
  format: yaml
  label: Azure SQL Database Firewall Rules API
  slug: microsoft-azure-sql-database-firewall-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Sql Database Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure SQL Database publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure SQL Database API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure SQL Database
provider_slug: microsoft-azure-sql-database
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-sql-database-databases-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-sql-database-servers-api-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-sql-database-scopes
source_filename: microsoft-azure-sql-database-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-sql-database-databases-api-openapi.yml, openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml,\n  openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml, openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml,\n  openapi/microsoft-azure-sql-database-servers-api-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-sql-database-databases-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/microsoft-azure-sql-database-servers-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-sql-database-databases-api-openapi.yml\n  - openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml\n  - openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml\n\
  \  - openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml\n  - openapi/microsoft-azure-sql-database-servers-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-sql-database/scopes/microsoft-azure-sql-database-scopes.yml
summary_line: 1 scope · implicit
tags:
- Database
- SQL
- Relational Database
- Microsoft Azure
- Microsoft
- Cloud Database
- Managed Database
- SQL Server
token_bound: false
token_urls: []
---
