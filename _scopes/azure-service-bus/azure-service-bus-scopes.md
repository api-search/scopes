---
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
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-service-bus-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: azure-service-bus-scopes
source_filename: azure-service-bus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-service-bus-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/azure-service-bus-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscopes:\n- scope: user_impersonation\n  description: Impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-service-bus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-service-bus/refs/heads/main/scopes/azure-service-bus-scopes.yml
summary_line: 1 scope · implicit
tags:
- Azure
- Cloud
- Enterprise
- Message Broker
- Messaging
- Pub/Sub
- Queues
token_urls: []
---
