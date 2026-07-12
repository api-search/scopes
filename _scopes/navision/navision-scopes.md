---
authorization_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Navision Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Dynamics NAV publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Dynamics NAV API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schemes:
- description: OAuth 2.0 authentication via Microsoft Entra ID
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/admin-center-api.yml
- description: OAuth 2.0 authentication via Microsoft Entra ID
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/automation-api.yml
- description: OAuth 2.0 authentication via Microsoft Entra ID
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/business-central-api-v2.yml
scope_count: 1
scope_names:
- https://api.businesscentral.dynamics.com/.default
scopes:
- description: Access Business Central Admin APIs
  flows:
  - authorizationCode
  - clientCredentials
  scope: https://api.businesscentral.dynamics.com/.default
slug: navision-scopes
source_filename: navision-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/admin-center-api.yml, openapi/automation-api.yml, openapi/business-central-api-v2.yml\nschemes:\n- name: oauth2\n  source: openapi/admin-center-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: OAuth 2.0 authentication via Microsoft Entra ID\n- name: oauth2\n  source: openapi/automation-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: OAuth 2.0 authentication\
  \ via Microsoft Entra ID\n- name: oauth2\n  source: openapi/business-central-api-v2.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: OAuth 2.0 authentication via Microsoft Entra ID\nscopes:\n- scope: https://api.businesscentral.dynamics.com/.default\n  description: Access Business Central Admin APIs\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/admin-center-api.yml\n  - openapi/automation-api.yml\n  - openapi/business-central-api-v2.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/scopes/navision-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
token_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
