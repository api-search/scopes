---
api_specs:
- filename: resource-manager
  format: yaml
  label: Azure Event Hubs REST API
  slug: azure-event-hubs-rest-api
  spec_type: OpenAPI
  url: https://github.com/Azure/azure-rest-api-specs/tree/main/specification/eventhub/resource-manager
- filename: data-plane
  format: yaml
  label: Azure Event Hubs Data Plane API
  slug: azure-event-hubs-data-plane-api
  spec_type: OpenAPI
  url: https://github.com/Azure/azure-rest-api-specs/tree/main/specification/eventhub/data-plane
- filename: azure-event-hubs-messaging-asyncapi.yml
  format: yaml
  label: Azure Event Hubs Messaging API
  slug: azure-event-hubs-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/asyncapi/azure-event-hubs-messaging-asyncapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Event Hubs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Event Hubs publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Event Hubs API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Event Hubs
provider_slug: microsoft-azure-event-hubs
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-event-hubs-management-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-event-hubs-scopes
source_filename: microsoft-azure-event-hubs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-event-hubs-management-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/azure-event-hubs-management-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: Impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-event-hubs-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/scopes/microsoft-azure-event-hubs-scopes.yml
summary_line: 1 scope · implicit
tags:
- Big Data
- Event Streaming
- IoT
- Message Ingestion
- Real-Time Processing
token_urls: []
---
