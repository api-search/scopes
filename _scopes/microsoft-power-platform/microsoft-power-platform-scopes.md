---
api_specs:
- filename: microsoft-power-platform-openapi.yml
  format: yaml
  label: Microsoft Dataverse Web API
  slug: dataverse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/microsoft-power-platform-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Power Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Power Platform publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Power Platform API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Power Platform
provider_slug: microsoft-power-platform
schemes:
- description: Microsoft Entra ID OAuth 2.0. Use the resource/scope corresponding to the Dataverse environment, e.g. https://{org}.api.crm.dynamics.com/.default for client credentials.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-power-platform-openapi.yml
scope_count: 1
scope_names:
- https://{org}.api.crm.dynamics.com/.default
scopes:
- description: Full Dataverse access scoped to the environment
  flows:
  - authorizationCode
  scope: https://{org}.api.crm.dynamics.com/.default
slug: microsoft-power-platform-scopes
source_filename: microsoft-power-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-power-platform-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-power-platform-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0. Use the resource/scope corresponding to the Dataverse\n    environment, e.g. https://{org}.api.crm.dynamics.com/.default for client credentials.\nscopes:\n- scope: https://{org}.api.crm.dynamics.com/.default\n  description: Full Dataverse access scoped to the environment\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-power-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/scopes/microsoft-power-platform-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Dataverse
- Low-Code
- Microsoft
- Power Apps
- Power Automate
- Power BI
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
