---
api_specs:
- filename: microsoft-azure-communication-services-callautomation-api-openapi.yml
  format: yaml
  label: Azure Communication Services Call Automation API
  slug: microsoft-azure-communication-services-callautomation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-callautomation-api-openapi.yml
- filename: microsoft-azure-communication-services-chat-api-openapi.yml
  format: yaml
  label: Azure Communication Services Chat API
  slug: microsoft-azure-communication-services-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-chat-api-openapi.yml
- filename: microsoft-azure-communication-services-email-api-openapi.yml
  format: yaml
  label: Azure Communication Services Email API
  slug: microsoft-azure-communication-services-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-email-api-openapi.yml
- filename: microsoft-azure-communication-services-identity-api-openapi.yml
  format: yaml
  label: Azure Communication Services Identity API
  slug: microsoft-azure-communication-services-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-identity-api-openapi.yml
- filename: microsoft-azure-communication-services-jobrouter-api-openapi.yml
  format: yaml
  label: Azure Communication Services Job Router API
  slug: microsoft-azure-communication-services-jobrouter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml
- filename: microsoft-azure-communication-services-messages-api-openapi.yml
  format: yaml
  label: Azure Communication Services Advanced Messaging API
  slug: microsoft-azure-communication-services-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-messages-api-openapi.yml
- filename: microsoft-azure-communication-services-phonenumbers-api-openapi.yml
  format: yaml
  label: Azure Communication Services Phone Numbers API
  slug: microsoft-azure-communication-services-phonenumbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml
- filename: microsoft-azure-communication-services-rooms-api-openapi.yml
  format: yaml
  label: Azure Communication Services Rooms API
  slug: microsoft-azure-communication-services-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-rooms-api-openapi.yml
- filename: microsoft-azure-communication-services-siprouting-api-openapi.yml
  format: yaml
  label: Azure Communication Services SIP Routing API
  slug: microsoft-azure-communication-services-siprouting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml
- filename: microsoft-azure-communication-services-sms-api-openapi.yml
  format: yaml
  label: Azure Communication Services SMS API
  slug: microsoft-azure-communication-services-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-sms-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Communication Services Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Azure Communication Services publishes 2 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Azure Communication Services API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Azure Communication Services
provider_slug: microsoft-azure-communication-services
schemes:
- description: The Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: AadOauth2Auth
  source: openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml
- description: The Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: AadOauth2Auth
  source: openapi/microsoft-azure-communication-services-messages-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-communication-services-sms-api-openapi.yml
scope_count: 2
scope_names:
- https://communication.azure.com/.default
- user_impersonation
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: https://communication.azure.com/.default
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-communication-services-scopes
source_filename: microsoft-azure-communication-services-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml, openapi/microsoft-azure-communication-services-messages-api-openapi.yml,\n  openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml, openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml,\n  openapi/microsoft-azure-communication-services-sms-api-openapi.yml\nschemes:\n- name: AadOauth2Auth\n  source: openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n  description: The Azure Active Directory OAuth2 Flow\n- name: AadOauth2Auth\n  source: openapi/microsoft-azure-communication-services-messages-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n\
  \    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n  description: The Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-communication-services-sms-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: https://communication.azure.com/.default\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-messages-api-openapi.yml\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-sms-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-communication-services/scopes/microsoft-azure-communication-services-scopes.yml
summary_line: 2 scopes · authorizationCode/implicit
tags:
- Microsoft Azure
- CPaaS
- Calling
- Chat
- Communications
- Contact Center
- Email
- Identity
- Messaging
- Phone Numbers
- Rooms
- Routing
- SIP
- SMS
- Telephony
- Tokens
- Video
- Voice
- WhatsApp
token_bound: false
token_urls:
- https://login.microsoftonline.com/common/oauth2/token
---
