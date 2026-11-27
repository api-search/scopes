---
api_specs:
- filename: azure-service-bus-namespaces-api-openapi.yml
  format: yaml
  label: Azure Service Bus Namespaces API
  slug: azure-service-bus-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-namespaces-api-openapi.yml
- filename: azure-service-bus-queues-api-openapi.yml
  format: yaml
  label: Azure Service Bus Queues API
  slug: azure-service-bus-queues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-queues-api-openapi.yml
- filename: azure-service-bus-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Service Bus Subscriptions API
  slug: azure-service-bus-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-subscriptions-api-openapi.yml
- filename: azure-service-bus-topics-api-openapi.yml
  format: yaml
  label: Azure Service Bus Topics API
  slug: azure-service-bus-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-topics-api-openapi.yml
- filename: azure-service-bus-armdisasterrecoveries-api-openapi.yml
  format: yaml
  label: Azure Service Bus Arm Disaster Recoveries API
  slug: azure-service-bus-armdisasterrecoveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-armdisasterrecoveries-api-openapi.yml
- filename: azure-service-bus-disasterrecoveryconfigs-api-openapi.yml
  format: yaml
  label: Azure Service Bus Disaster Recovery Configs API
  slug: azure-service-bus-disasterrecoveryconfigs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-disasterrecoveryconfigs-api-openapi.yml
- filename: azure-service-bus-migrationconfigs-api-openapi.yml
  format: yaml
  label: Azure Service Bus Migration Configs API
  slug: azure-service-bus-migrationconfigs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-migrationconfigs-api-openapi.yml
- filename: azure-service-bus-namespaces-authorizationrule-api-openapi.yml
  format: yaml
  label: Azure Service Bus Namespaces AuthorizationRule API
  slug: azure-service-bus-namespaces-authorizationrule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-namespaces-authorizationrule-api-openapi.yml
- filename: azure-service-bus-networksecurityperimeterconfigurations-api-openapi.yml
  format: yaml
  label: Azure Service Bus Network Security Perimeter Configurations API
  slug: azure-service-bus-networksecurityperimeterconfigurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-networksecurityperimeterconfigurations-api-openapi.yml
- filename: azure-service-bus-operations-api-openapi.yml
  format: yaml
  label: Azure Service Bus Operations API
  slug: azure-service-bus-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-operations-api-openapi.yml
- filename: azure-service-bus-rules-api-openapi.yml
  format: yaml
  label: Azure Service Bus Rules API
  slug: azure-service-bus-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-rules-api-openapi.yml
- filename: azure-service-bus-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Service Bus Private Endpoint Connections API
  slug: azure-service-bus-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-private-endpoint-connections-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Service Bus Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Service Bus publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Service Bus API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Service Bus
provider_slug: azure-service-bus
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/azure-service-bus-data-plane-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/azure-service-bus-namespaces-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/azure-service-bus-queues-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/azure-service-bus-resource-manager-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/azure-service-bus-subscriptions-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/azure-service-bus-topics-api-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-service-bus-scopes
source_filename: azure-service-bus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/azure-service-bus-data-plane-openapi.yml, openapi/_superseded/azure-service-bus-namespaces-api-openapi.yml,\n  openapi/_superseded/azure-service-bus-queues-api-openapi.yml, openapi/_superseded/azure-service-bus-resource-manager-openapi.yml,\n  openapi/_superseded/azure-service-bus-subscriptions-api-openapi.yml, openapi/_superseded/azure-service-bus-topics-api-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/_superseded/azure-service-bus-data-plane-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/_superseded/azure-service-bus-namespaces-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: azure_auth\n  source: openapi/_superseded/azure-service-bus-queues-api-openapi.yml\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: azure_auth\n  source: openapi/_superseded/azure-service-bus-resource-manager-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/_superseded/azure-service-bus-subscriptions-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: azure_auth\n  source: openapi/_superseded/azure-service-bus-topics-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/_superseded/azure-service-bus-data-plane-openapi.yml\n  - openapi/_superseded/azure-service-bus-namespaces-api-openapi.yml\n\
  \  - openapi/_superseded/azure-service-bus-queues-api-openapi.yml\n  - openapi/_superseded/azure-service-bus-resource-manager-openapi.yml\n  - openapi/_superseded/azure-service-bus-subscriptions-api-openapi.yml\n  - openapi/_superseded/azure-service-bus-topics-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/azure-service-bus/scopes/azure-service-bus-scopes.yml
summary_line: 1 scope · implicit
tags:
- Microsoft Azure
- Cloud
- Enterprise
- Message Broker
- Messaging
- Pub/Sub
- Queues
- Real-Time
token_bound: false
token_urls: []
---
