---
api_specs:
- filename: microsoft-skype-deliveryreports-api-openapi.yml
  format: yaml
  label: Microsoft Skype Delivery Reports API
  slug: microsoft-skype-deliveryreports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-deliveryreports-api-openapi.yml
- filename: microsoft-skype-messages-api-openapi.yml
  format: yaml
  label: Microsoft Skype Messages API
  slug: microsoft-skype-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-messages-api-openapi.yml
- filename: microsoft-skype-optoutsadd-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Add API
  slug: microsoft-skype-optoutsadd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutsadd-api-openapi.yml
- filename: microsoft-skype-optoutscheck-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Check API
  slug: microsoft-skype-optoutscheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutscheck-api-openapi.yml
- filename: microsoft-skype-optoutsremove-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Remove API
  slug: microsoft-skype-optoutsremove-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutsremove-api-openapi.yml
- filename: microsoft-skype-participants-api-openapi.yml
  format: yaml
  label: Microsoft Skype Participants API
  slug: microsoft-skype-participants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-participants-api-openapi.yml
- filename: microsoft-skype-sms-api-openapi.yml
  format: yaml
  label: Microsoft Skype Sms API
  slug: microsoft-skype-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-sms-api-openapi.yml
- filename: microsoft-skype-threads-api-openapi.yml
  format: yaml
  label: Microsoft Skype Threads API
  slug: microsoft-skype-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-threads-api-openapi.yml
- filename: microsoft-skype-typingnotifications-api-openapi.yml
  format: yaml
  label: Microsoft Skype Typing Notifications API
  slug: microsoft-skype-typingnotifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-typingnotifications-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Skype Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Skype publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Skype API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Skype
provider_slug: microsoft-skype
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-skype-sms-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-skype-scopes
source_filename: microsoft-skype-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/microsoft-skype-sms-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-skype-sms-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-skype-sms-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-skype/scopes/microsoft-skype-scopes.yml
summary_line: 1 scope · implicit
tags:
- Communications
- Messaging
- Microsoft
- Video
- Voice
token_bound: false
token_urls: []
---
