---
api_specs:
- filename: microsoft-bot-framework-bot-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot API
  slug: microsoft-bot-framework-bot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-bot-api-openapi.yml
- filename: microsoft-bot-framework-botconnection-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot Connection API
  slug: microsoft-bot-framework-botconnection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-botconnection-api-openapi.yml
- filename: microsoft-bot-framework-bothostsettings-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot Host Settings API
  slug: microsoft-bot-framework-bothostsettings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-bothostsettings-api-openapi.yml
- filename: microsoft-bot-framework-channel-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Channel API
  slug: microsoft-bot-framework-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-channel-api-openapi.yml
- filename: microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework List Qn A Maker Endpoint Keys API
  slug: microsoft-bot-framework-listqnamakerendpointkeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml
- filename: microsoft-bot-framework-listserviceproviders-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework List Service Providers API
  slug: microsoft-bot-framework-listserviceproviders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-listserviceproviders-api-openapi.yml
- filename: microsoft-bot-framework-operationresults-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Operation Results API
  slug: microsoft-bot-framework-operationresults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-operationresults-api-openapi.yml
- filename: microsoft-bot-framework-operations-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Operations API
  slug: microsoft-bot-framework-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-operations-api-openapi.yml
- filename: microsoft-bot-framework-privatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Private Link Resources API
  slug: microsoft-bot-framework-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-privatelinkresources-api-openapi.yml
- filename: microsoft-bot-framework-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Private Endpoint Connections API
  slug: microsoft-bot-framework-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-private-endpoint-connections-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Bot Framework Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Bot Framework publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Bot Framework API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Bot Framework
provider_slug: microsoft-bot-framework
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-bot-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-botconnection-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-bothostsettings-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-channel-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-listserviceproviders-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-operationresults-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-operations-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-private-endpoint-connections-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-bot-framework-privatelinkresources-api-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-bot-framework-scopes
source_filename: microsoft-bot-framework-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/microsoft-bot-framework-bot-api-openapi.yml, openapi/microsoft-bot-framework-botconnection-api-openapi.yml,\n  openapi/microsoft-bot-framework-bothostsettings-api-openapi.yml, openapi/microsoft-bot-framework-channel-api-openapi.yml,\n  openapi/microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml, openapi/microsoft-bot-framework-listserviceproviders-api-openapi.yml,\n  openapi/microsoft-bot-framework-operationresults-api-openapi.yml, openapi/microsoft-bot-framework-operations-api-openapi.yml,\n  openapi/microsoft-bot-framework-private-endpoint-connections-api-openapi.yml, openapi/microsoft-bot-framework-privatelinkresources-api-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-bot-framework-bot-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n\
  \  source: openapi/microsoft-bot-framework-botconnection-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-bot-framework-bothostsettings-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-bot-framework-channel-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2\
  \ Flow\n- name: azure_auth\n  source: openapi/microsoft-bot-framework-listserviceproviders-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-bot-framework-operationresults-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-bot-framework-operations-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-bot-framework-private-endpoint-connections-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n\
  \  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-bot-framework-privatelinkresources-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-bot-framework-bot-api-openapi.yml\n  - openapi/microsoft-bot-framework-botconnection-api-openapi.yml\n  - openapi/microsoft-bot-framework-bothostsettings-api-openapi.yml\n  - openapi/microsoft-bot-framework-channel-api-openapi.yml\n  - openapi/microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml\n  - openapi/microsoft-bot-framework-listserviceproviders-api-openapi.yml\n  - openapi/microsoft-bot-framework-operationresults-api-openapi.yml\n  - openapi/microsoft-bot-framework-operations-api-openapi.yml\n  - openapi/microsoft-bot-framework-private-endpoint-connections-api-openapi.yml\n\
  \  - openapi/microsoft-bot-framework-privatelinkresources-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-bot-framework/scopes/microsoft-bot-framework-scopes.yml
summary_line: 1 scope · implicit
tags:
- Bots
- Conversational AI
- Messaging
- Bot Framework
- Direct Line
token_bound: false
token_urls: []
---
