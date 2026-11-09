---
api_specs:
- filename: microsoft-azure-stream-analytics-clusters-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Clusters API
  slug: microsoft-azure-stream-analytics-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-clusters-api-openapi.yml
- filename: microsoft-azure-stream-analytics-functions-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Functions API
  slug: microsoft-azure-stream-analytics-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-functions-api-openapi.yml
- filename: microsoft-azure-stream-analytics-inputs-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Inputs API
  slug: microsoft-azure-stream-analytics-inputs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-inputs-api-openapi.yml
- filename: microsoft-azure-stream-analytics-outputs-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Outputs API
  slug: microsoft-azure-stream-analytics-outputs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-outputs-api-openapi.yml
- filename: microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics StreamingJobs API
  slug: microsoft-azure-stream-analytics-streamingjobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml
- filename: microsoft-azure-stream-analytics-transformations-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Transformations API
  slug: microsoft-azure-stream-analytics-transformations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-transformations-api-openapi.yml
- filename: microsoft-azure-stream-analytics-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Subscriptions API
  slug: microsoft-azure-stream-analytics-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-subscriptions-api-openapi.yml
- filename: microsoft-azure-stream-analytics-operations-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Operations API
  slug: microsoft-azure-stream-analytics-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-operations-api-openapi.yml
- filename: microsoft-azure-stream-analytics-private-endpoints-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Private Endpoints API
  slug: microsoft-azure-stream-analytics-private-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-private-endpoints-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Stream Analytics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Stream Analytics publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Stream Analytics API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Stream Analytics
provider_slug: microsoft-azure-stream-analytics
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-stream-analytics-clusters-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-stream-analytics-functions-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-stream-analytics-inputs-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-stream-analytics-outputs-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-stream-analytics-privateendpoints-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-stream-analytics-subscriptions-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-stream-analytics-transformations-api-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-stream-analytics-scopes
source_filename: microsoft-azure-stream-analytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-stream-analytics-clusters-api-openapi.yml, openapi/microsoft-azure-stream-analytics-functions-api-openapi.yml,\n  openapi/microsoft-azure-stream-analytics-inputs-api-openapi.yml, openapi/microsoft-azure-stream-analytics-outputs-api-openapi.yml,\n  openapi/microsoft-azure-stream-analytics-privateendpoints-api-openapi.yml, openapi/microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml,\n  openapi/microsoft-azure-stream-analytics-subscriptions-api-openapi.yml, openapi/microsoft-azure-stream-analytics-transformations-api-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-stream-analytics-clusters-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-stream-analytics-functions-api-openapi.yml\n  flows:\n\
  \  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-stream-analytics-inputs-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-stream-analytics-outputs-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-stream-analytics-privateendpoints-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-stream-analytics-subscriptions-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-stream-analytics-transformations-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-stream-analytics-clusters-api-openapi.yml\n  - openapi/microsoft-azure-stream-analytics-functions-api-openapi.yml\n  - openapi/microsoft-azure-stream-analytics-inputs-api-openapi.yml\n\
  \  - openapi/microsoft-azure-stream-analytics-outputs-api-openapi.yml\n  - openapi/microsoft-azure-stream-analytics-privateendpoints-api-openapi.yml\n  - openapi/microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml\n  - openapi/microsoft-azure-stream-analytics-subscriptions-api-openapi.yml\n  - openapi/microsoft-azure-stream-analytics-transformations-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-stream-analytics/scopes/microsoft-azure-stream-analytics-scopes.yml
summary_line: 1 scope · implicit
tags:
- Stream Processing
- Real-Time Analytics
- IoT
- Event Processing
- Microsoft Azure
- Streaming
token_bound: false
token_urls: []
---
