---
api_specs:
- filename: azure-log-analytics-query-api.yaml
  format: yaml
  label: Azure Log Analytics Query API
  slug: azure-log-analytics-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/openapi/azure-log-analytics-query-api.yaml
- filename: azure-log-analytics-management-api.yaml
  format: yaml
  label: Azure Log Analytics Management API
  slug: azure-log-analytics-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/openapi/azure-log-analytics-management-api.yaml
- filename: azure-log-analytics-ingestion-api.yaml
  format: yaml
  label: Azure Log Analytics Ingestion API
  slug: azure-log-analytics-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/openapi/azure-log-analytics-ingestion-api.yaml
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/scopes/azure-log-analytics-scopes.yml
summary_line: 1 scope · implicit
tags:
- Analytics
- Azure
- Cloud
- Logging
- Monitoring
token_urls: []
---
