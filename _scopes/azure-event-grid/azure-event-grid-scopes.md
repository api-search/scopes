---
api_specs:
- filename: azure-event-grid-openapi.yml
  format: yaml
  label: Azure Event Grid Publisher API
  slug: publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-event-grid/refs/heads/main/openapi/azure-event-grid-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Azure Event Grid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Event Grid publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Event Grid API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Event Grid
provider_slug: azure-event-grid
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  source: openapi/azure-event-grid-openapi.yml
scope_count: 1
scope_names:
- https://eventgrid.azure.net/.default
scopes:
- description: Publish/receive Event Grid events
  flows:
  - clientCredentials
  scope: https://eventgrid.azure.net/.default
slug: azure-event-grid-scopes
source_filename: azure-event-grid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-event-grid-openapi.yml\nschemes:\n- name: entra\n  source: openapi/azure-event-grid-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\nscopes:\n- scope: https://eventgrid.azure.net/.default\n  description: Publish/receive Event Grid events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-event-grid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-event-grid/refs/heads/main/scopes/azure-event-grid-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Eventing
- Event Driven
- Pub Sub
- Messaging
- Webhooks
- CloudEvents
- Cloud
- Azure
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
