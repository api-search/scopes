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
name: Microsoft Azure Signalr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure SignalR Service publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure SignalR Service API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure SignalR Service
provider_slug: microsoft-azure-signalr
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-signalr-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-signalr-scopes
source_filename: microsoft-azure-signalr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-signalr-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-signalr-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: Impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-signalr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-signalr/refs/heads/main/scopes/microsoft-azure-signalr-scopes.yml
summary_line: 1 scope · implicit
tags:
- Real-Time
- WebSockets
- SignalR
- Messaging
- Push
token_urls: []
---
