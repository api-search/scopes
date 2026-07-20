---
api_specs:
- filename: microsoft-power-automate-management-api.yaml
  format: yaml
  label: Power Automate Management API
  slug: power-automate-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/openapi/microsoft-power-automate-management-api.yaml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: https://learn.microsoft.com/en-us/power-automate/web-api#authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Power Automate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Power Automate publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Power Automate API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Power Automate
provider_slug: microsoft-power-automate
schemes:
- description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: oauth2
  source: openapi/microsoft-power-automate-management-api.yaml
scope_count: 1
scope_names:
- https://service.flow.microsoft.com/.default
scopes:
- description: Access Power Automate Management API
  flows:
  - authorizationCode
  scope: https://service.flow.microsoft.com/.default
slug: microsoft-power-automate-scopes
source_filename: microsoft-power-automate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/microsoft-power-automate-management-api.yaml\ndocs: https://learn.microsoft.com/en-us/power-automate/web-api#authentication\nnotes: >-\n  The Power Automate Management API is accessed with the resource-level\n  \".default\" scope of the Power Automate service application\n  (https://service.flow.microsoft.com/.default). Effective permissions are\n  governed by the caller's Microsoft Entra ID roles and Power Platform\n  environment access, not by fine-grained per-operation OAuth scopes.\nschemes:\n- name: oauth2\n  source: openapi/microsoft-power-automate-management-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.\nscopes:\n- scope: https://service.flow.microsoft.com/.default\n  description: Access Power\
  \ Automate Management API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-power-automate-management-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/scopes/microsoft-power-automate-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Automation
- Business Process
- Integration
- Low-Code
- Microsoft
- Power Platform
- RPA
- Workflow
token_urls:
- https://login.microsoftonline.com/common/oauth2/token
---
