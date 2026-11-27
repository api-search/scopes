---
api_specs:
- filename: azure-devops-health-availabilitystatuses-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Availability Statuses API
  slug: azure-devops-health-availabilitystatuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-availabilitystatuses-api-openapi.yml
- filename: azure-devops-health-childavailabilitystatuses-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Child Availability Statuses API
  slug: azure-devops-health-childavailabilitystatuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml
- filename: azure-devops-health-childresources-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Child Resources API
  slug: azure-devops-health-childresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-childresources-api-openapi.yml
- filename: azure-devops-health-emergingissues-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Emerging Issues API
  slug: azure-devops-health-emergingissues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-emergingissues-api-openapi.yml
- filename: azure-devops-health-event-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Event API
  slug: azure-devops-health-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-event-api-openapi.yml
- filename: azure-devops-health-eventimpactedresources-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Event Impacted Resources API
  slug: azure-devops-health-eventimpactedresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-eventimpactedresources-api-openapi.yml
- filename: azure-devops-health-events-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Events API
  slug: azure-devops-health-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-events-api-openapi.yml
- filename: azure-devops-health-metadata-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Metadata API
  slug: azure-devops-health-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-metadata-api-openapi.yml
- filename: azure-devops-health-operations-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Operations API
  slug: azure-devops-health-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-operations-api-openapi.yml
- filename: azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Security Advisory Impacted Resources API
  slug: azure-devops-health-securityadvisoryimpactedresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Resource Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Resource Health publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Resource Health API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Resource Health
provider_slug: azure-devops-health
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-availabilitystatuses-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-childresources-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-emergingissues-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-event-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-eventimpactedresources-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-events-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-metadata-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-operations-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-devops-health-scopes
source_filename: azure-devops-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/azure-devops-health-availabilitystatuses-api-openapi.yml, openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml,\n  openapi/azure-devops-health-childresources-api-openapi.yml, openapi/azure-devops-health-emergingissues-api-openapi.yml,\n  openapi/azure-devops-health-event-api-openapi.yml, openapi/azure-devops-health-eventimpactedresources-api-openapi.yml,\n  openapi/azure-devops-health-events-api-openapi.yml, openapi/azure-devops-health-metadata-api-openapi.yml,\n  openapi/azure-devops-health-operations-api-openapi.yml, openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/azure-devops-health-availabilitystatuses-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-devops-health-childresources-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-devops-health-emergingissues-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-devops-health-event-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-devops-health-eventimpactedresources-api-openapi.yml\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-devops-health-events-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-devops-health-metadata-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-devops-health-operations-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-devops-health-availabilitystatuses-api-openapi.yml\n  - openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml\n  - openapi/azure-devops-health-childresources-api-openapi.yml\n  - openapi/azure-devops-health-emergingissues-api-openapi.yml\n  - openapi/azure-devops-health-event-api-openapi.yml\n  - openapi/azure-devops-health-eventimpactedresources-api-openapi.yml\n  - openapi/azure-devops-health-events-api-openapi.yml\n  - openapi/azure-devops-health-metadata-api-openapi.yml\n  - openapi/azure-devops-health-operations-api-openapi.yml\n  - openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/azure-devops-health/scopes/azure-devops-health-scopes.yml
summary_line: 1 scope · implicit
tags:
- Continuous Integration
- Developer Tools
- Public APIs
- Microsoft Azure
- Microsoft
- Monitoring
- Service Health
token_bound: false
token_urls: []
---
