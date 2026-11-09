---
api_specs:
- filename: microsoft-azure-web-pubsub-asyncapi.yml
  format: yaml
  label: Azure Web PubSub Client and Upstream Events
  slug: azure-web-pubsub-client-and-upstream-events
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/microsoft-azure-web-pubsub/asyncapi/microsoft-azure-web-pubsub-asyncapi.yml
- filename: microsoft-azure-web-pubsub-hub-api-openapi.yml
  format: yaml
  label: Azure Web PubSub Hub API
  slug: microsoft-azure-web-pubsub-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-web-pubsub/openapi/microsoft-azure-web-pubsub-hub-api-openapi.yml
- filename: microsoft-azure-web-pubsub-permission-api-openapi.yml
  format: yaml
  label: Azure Web PubSub Permission API
  slug: microsoft-azure-web-pubsub-permission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-web-pubsub/openapi/microsoft-azure-web-pubsub-permission-api-openapi.yml
- filename: microsoft-azure-web-pubsub-general-api-openapi.yml
  format: yaml
  label: Azure Web PubSub General API
  slug: microsoft-azure-web-pubsub-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-web-pubsub/openapi/microsoft-azure-web-pubsub-general-api-openapi.yml
- filename: microsoft-azure-web-pubsub-webpubsub-api-openapi.yml
  format: yaml
  label: Azure Web PubSub Webpubsub API
  slug: microsoft-azure-web-pubsub-webpubsub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-web-pubsub/openapi/microsoft-azure-web-pubsub-webpubsub-api-openapi.yml
- filename: microsoft-azure-web-pubsub-client-token-api-openapi.yml
  format: yaml
  label: Azure Web PubSub Client Token API
  slug: microsoft-azure-web-pubsub-client-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-web-pubsub/openapi/microsoft-azure-web-pubsub-client-token-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Web Pubsub Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Web PubSub publishes 2 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Web PubSub API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Web PubSub
provider_slug: microsoft-azure-web-pubsub
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: OAuth2Auth
  source: openapi/microsoft-azure-web-pubsub-data-plane-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-web-pubsub-management-api-openapi.yml
scope_count: 2
scope_names:
- https://webpubsub.azure.com/.default
- user_impersonation
scopes:
- description: ''
  flows:
  - implicit
  scope: https://webpubsub.azure.com/.default
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-web-pubsub-scopes
source_filename: microsoft-azure-web-pubsub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-web-pubsub-data-plane-api-openapi.yml, openapi/microsoft-azure-web-pubsub-management-api-openapi.yml\nschemes:\n- name: OAuth2Auth\n  source: openapi/microsoft-azure-web-pubsub-data-plane-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: azure_auth\n  source: openapi/microsoft-azure-web-pubsub-management-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: https://webpubsub.azure.com/.default\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-web-pubsub-data-plane-api-openapi.yml\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-web-pubsub-management-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-web-pubsub/scopes/microsoft-azure-web-pubsub-scopes.yml
summary_line: 2 scopes · implicit
tags:
- Messaging
- Pub/Sub
- Real-Time
- Serverless
- WebSocket
token_bound: false
token_urls: []
---
