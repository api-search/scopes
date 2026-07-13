---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Power Apps REST API
  slug: power-apps-rest-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/connectors/powerappsforappmakers/
- filename: openapi
  format: yaml
  label: Microsoft Dataverse Web API
  slug: microsoft-dataverse-web-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/openapi
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Power Apps Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Power Apps publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Power Apps API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Power Apps
provider_slug: power-apps
schemes:
- description: 'Authentication uses Microsoft Entra ID (Azure AD) OAuth 2.0. Acquire a

    bearer token with the audience set to the Dataverse organization URL,

    for example https://{organization}.crm.dynamics.com/.default.'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: OAuth2
  source: openapi/power-apps-openapi.yml
scope_count: 2
scope_names:
- https://{organization}.crm.dynamics.com/.default
- https://{organization}.crm.dynamics.com/user_impersonation
scopes:
- description: Application access to Dataverse
  flows:
  - clientCredentials
  scope: https://{organization}.crm.dynamics.com/.default
- description: Access Dataverse as the signed-in user
  flows:
  - authorizationCode
  scope: https://{organization}.crm.dynamics.com/user_impersonation
slug: power-apps-scopes
source_filename: power-apps-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/power-apps-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/power-apps-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: |-\n    Authentication uses Microsoft Entra ID (Azure AD) OAuth 2.0. Acquire a\n    bearer token with the audience set to the Dataverse organization URL,\n    for example https://{organization}.crm.dynamics.com/.default.\nscopes:\n- scope: https://{organization}.crm.dynamics.com/.default\n  description: Application access to Dataverse\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/power-apps-openapi.yml\n- scope: https://{organization}.crm.dynamics.com/user_impersonation\n  description: Access Dataverse as\
  \ the signed-in user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/power-apps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-apps/refs/heads/main/scopes/power-apps-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- App Development
- Business Applications
- Cloud Platform
- Low-Code
- Microsoft
- No-Code
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
