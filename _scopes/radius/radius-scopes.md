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
name: Radius Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Radius publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Radius API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Radius
provider_slug: radius
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/radius-applications-core-openapi.json
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/radius-applications-dapr-openapi.json
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/radius-applications-datastores-openapi.json
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/radius-applications-messaging-openapi.json
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/radius-ucp-openapi.json
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: radius-scopes
source_filename: radius-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/radius-applications-core-openapi.json, openapi/radius-applications-dapr-openapi.json,\n  openapi/radius-applications-datastores-openapi.json, openapi/radius-applications-messaging-openapi.json,\n  openapi/radius-ucp-openapi.json\nschemes:\n- name: azure_auth\n  source: openapi/radius-applications-core-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/radius-applications-dapr-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/radius-applications-datastores-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure\
  \ Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/radius-applications-messaging-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/radius-ucp-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/radius-applications-core-openapi.json\n  - openapi/radius-applications-dapr-openapi.json\n  - openapi/radius-applications-datastores-openapi.json\n  - openapi/radius-applications-messaging-openapi.json\n  - openapi/radius-ucp-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/scopes/radius-scopes.yml
summary_line: 1 scope · implicit
tags:
- Application Platform
- Cloud Native
- Infrastructure
- Multi Cloud
token_urls: []
---
