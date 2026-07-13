---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Power Apps API
  slug: power-apps-api
  spec_type: OpenAPI
  url: https://docs.microsoft.com/en-us/connectors/powerappsforappmakers/
- filename: openapi
  format: yaml
  label: Dataverse API (Common Data Service)
  slug: dataverse-api-common-data-service
  spec_type: OpenAPI
  url: https://docs.microsoft.com/en-us/power-apps/developer/data-platform/webapi/openapi
authorization_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Power Apps Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Power Apps publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Power Apps API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Power Apps
provider_slug: microsoft-power-apps
schemes:
- description: OAuth 2.0 authentication using Microsoft Entra ID (formerly Azure Active Directory). Applications must be registered in Microsoft Entra ID and granted appropriate Dataverse permissions.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-power-apps-dataverse-web-api-openapi.yml
scope_count: 2
scope_names:
- https://{organization}.crm.dynamics.com/.default
- https://{organization}.crm.dynamics.com/user_impersonation
scopes:
- description: Full access to Dataverse environment
  flows:
  - authorizationCode
  scope: https://{organization}.crm.dynamics.com/.default
- description: Access Dataverse as the signed-in user
  flows:
  - authorizationCode
  scope: https://{organization}.crm.dynamics.com/user_impersonation
slug: microsoft-power-apps-scopes
source_filename: microsoft-power-apps-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-power-apps-dataverse-web-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-power-apps-dataverse-web-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: OAuth 2.0 authentication using Microsoft Entra ID (formerly Azure Active Directory).\n    Applications must be registered in Microsoft Entra ID and granted appropriate Dataverse\n    permissions.\nscopes:\n- scope: https://{organization}.crm.dynamics.com/.default\n  description: Full access to Dataverse environment\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-power-apps-dataverse-web-api-openapi.yml\n- scope: https://{organization}.crm.dynamics.com/user_impersonation\n  description: Access Dataverse as the signed-in user\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/microsoft-power-apps-dataverse-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-apps/refs/heads/main/scopes/microsoft-power-apps-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Business Applications
- Cloud
- Enterprise
- Low-Code
- Microsoft
- No-Code
- Power Platform
- SaaS
token_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
