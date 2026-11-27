---
api_specs:
- filename: azure-log-analytics-tables-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Tables API
  slug: azure-log-analytics-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-tables-api-openapi.yml
- filename: azure-log-analytics-workspaces-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Workspaces API
  slug: azure-log-analytics-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-workspaces-api-openapi.yml
- filename: azure-log-analytics-availableservicetiers-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Available Service Tiers API
  slug: azure-log-analytics-availableservicetiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-availableservicetiers-api-openapi.yml
- filename: azure-log-analytics-clusters-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Clusters API
  slug: azure-log-analytics-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-clusters-api-openapi.yml
- filename: azure-log-analytics-deletedworkspaces-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Deleted Workspaces API
  slug: azure-log-analytics-deletedworkspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-deletedworkspaces-api-openapi.yml
- filename: azure-log-analytics-intelligencepacks-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Intelligence Packs API
  slug: azure-log-analytics-intelligencepacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-intelligencepacks-api-openapi.yml
- filename: azure-log-analytics-linkedservices-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Linked Services API
  slug: azure-log-analytics-linkedservices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-linkedservices-api-openapi.yml
- filename: azure-log-analytics-linkedstorageaccounts-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Linked Storage Accounts API
  slug: azure-log-analytics-linkedstorageaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-linkedstorageaccounts-api-openapi.yml
- filename: azure-log-analytics-networksecurityperimeterconfigurations-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Network Security Perimeter Configurations API
  slug: azure-log-analytics-networksecurityperimeterconfigurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-networksecurityperimeterconfigurations-api-openapi.yml
- filename: azure-log-analytics-operations-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Operations API
  slug: azure-log-analytics-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-operations-api-openapi.yml
- filename: azure-log-analytics-storageinsights-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Storage Insights API
  slug: azure-log-analytics-storageinsights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-storageinsights-api-openapi.yml
- filename: azure-log-analytics-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Subscriptions API
  slug: azure-log-analytics-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-subscriptions-api-openapi.yml
- filename: azure-log-analytics-summaryrules-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Summary Rules API
  slug: azure-log-analytics-summaryrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-summaryrules-api-openapi.yml
- filename: azure-log-analytics-async-operations-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Async Operations API
  slug: azure-log-analytics-async-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-async-operations-api-openapi.yml
- filename: azure-log-analytics-data-export-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Data Export API
  slug: azure-log-analytics-data-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-data-export-api-openapi.yml
- filename: azure-log-analytics-data-sources-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Data Sources API
  slug: azure-log-analytics-data-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-data-sources-api-openapi.yml
- filename: azure-log-analytics-saved-searches-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Saved Searches API
  slug: azure-log-analytics-saved-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-saved-searches-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Log Analytics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Log Analytics publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Log Analytics API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Log Analytics
provider_slug: azure-log-analytics
schemes:
- description: Azure Active Directory OAuth2 implicit flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: oauth2
  source: openapi/azure-log-analytics-management-api.yaml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-log-analytics-scopes
source_filename: azure-log-analytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-log-analytics-management-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/azure-log-analytics-management-api.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 implicit flow.\nscopes:\n- scope: user_impersonation\n  description: Impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-log-analytics-management-api.yaml\n"
source_yaml_url: https://artifacts.apis.io/azure-log-analytics/scopes/azure-log-analytics-scopes.yml
summary_line: 1 scope · implicit
tags:
- Analytics
- Microsoft Azure
- Cloud
- Logging
- Monitoring
token_bound: false
token_urls: []
---
