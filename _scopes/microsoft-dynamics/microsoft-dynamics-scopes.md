---
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
name: Microsoft Dynamics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Dynamics publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Dynamics API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schemes:
- description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-dynamics-business-central-openapi.yml
- description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-dynamics-dataverse-openapi.yml
- description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-dynamics-finance-operations-openapi.yml
scope_count: 3
scope_names:
- https://api.businesscentral.dynamics.com/.default
- https://myorg.operations.dynamics.com/.default
- https://org.crm.dynamics.com/.default
scopes:
- description: Access Business Central API
  flows:
  - authorizationCode
  scope: https://api.businesscentral.dynamics.com/.default
- description: Access Finance & Operations API
  flows:
  - clientCredentials
  scope: https://myorg.operations.dynamics.com/.default
- description: Access Dataverse API
  flows:
  - authorizationCode
  scope: https://org.crm.dynamics.com/.default
slug: microsoft-dynamics-scopes
source_filename: microsoft-dynamics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-dynamics-business-central-openapi.yml, openapi/microsoft-dynamics-dataverse-openapi.yml,\n  openapi/microsoft-dynamics-finance-operations-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-dynamics-business-central-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.\n- name: oauth2\n  source: openapi/microsoft-dynamics-dataverse-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.\n- name: oauth2\n  source: openapi/microsoft-dynamics-finance-operations-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.\nscopes:\n- scope: https://api.businesscentral.dynamics.com/.default\n  description: Access Business Central API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-dynamics-business-central-openapi.yml\n- scope: https://myorg.operations.dynamics.com/.default\n  description: Access Finance & Operations API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-dynamics-finance-operations-openapi.yml\n- scope: https://org.crm.dynamics.com/.default\n  description: Access Dataverse API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-dynamics-dataverse-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/scopes/microsoft-dynamics-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- CRM
- ERP
- Microsoft Dynamics
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
