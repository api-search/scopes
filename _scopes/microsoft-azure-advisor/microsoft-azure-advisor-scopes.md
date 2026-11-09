---
api_specs:
- filename: microsoft-azure-advisor-operations-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Operations API
  slug: microsoft-azure-advisor-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-operations-api-openapi.yml
- filename: microsoft-azure-advisor-recommendations-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Recommendations API
  slug: microsoft-azure-advisor-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-recommendations-api-openapi.yml
- filename: microsoft-azure-advisor-advisorscoreentities-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Advisor Score Entities API
  slug: microsoft-azure-advisor-advisorscoreentities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-advisorscoreentities-api-openapi.yml
- filename: microsoft-azure-advisor-metadataentities-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Metadata Entities API
  slug: microsoft-azure-advisor-metadataentities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-metadataentities-api-openapi.yml
- filename: microsoft-azure-advisor-resiliencyreviews-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Resiliency Reviews API
  slug: microsoft-azure-advisor-resiliencyreviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-resiliencyreviews-api-openapi.yml
- filename: microsoft-azure-advisor-resourcerecommendationbases-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Resource Recommendation Bases API
  slug: microsoft-azure-advisor-resourcerecommendationbases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-resourcerecommendationbases-api-openapi.yml
- filename: microsoft-azure-advisor-subscriptions-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Subscriptions API
  slug: microsoft-azure-advisor-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-subscriptions-api-openapi.yml
- filename: microsoft-azure-advisor-suppressioncontracts-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Suppression Contracts API
  slug: microsoft-azure-advisor-suppressioncontracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-suppressioncontracts-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Advisor Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure Advisor publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure Advisor API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure Advisor
provider_slug: microsoft-azure-advisor
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-advisor-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-advisor-operations-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-advisor-recommendations-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-advisor-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-advisor-scopes
source_filename: microsoft-azure-advisor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-advisor-openapi.yml, openapi/microsoft-azure-advisor-operations-api-openapi.yml,\n  openapi/microsoft-azure-advisor-recommendations-api-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-advisor-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/microsoft-azure-advisor-operations-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/microsoft-azure-advisor-recommendations-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name:\
  \ azure_auth\n  source: openapi/microsoft-azure-advisor-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-advisor-openapi.yml\n  - openapi/microsoft-azure-advisor-operations-api-openapi.yml\n  - openapi/microsoft-azure-advisor-recommendations-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-advisor/scopes/microsoft-azure-advisor-scopes.yml
summary_line: 1 scope · implicit
tags:
- Advisor
- Best Practices
- Cost Optimization
- Microsoft Azure
- Optimization
- Recommendations
token_bound: false
token_urls: []
---
