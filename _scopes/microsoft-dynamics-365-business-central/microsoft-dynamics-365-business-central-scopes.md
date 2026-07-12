---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Dynamics 365 Business Central Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Dynamics 365 Business Central publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Dynamics 365 Business Central API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Dynamics 365 Business Central
provider_slug: microsoft-dynamics-365-business-central
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-dynamics-365-business-central-openapi.yml
scope_count: 1
scope_names:
- https://api.businesscentral.dynamics.com/.default
scopes:
- description: Business Central API access
  flows:
  - authorizationCode
  scope: https://api.businesscentral.dynamics.com/.default
slug: microsoft-dynamics-365-business-central-scopes
source_filename: microsoft-dynamics-365-business-central-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-dynamics-365-business-central-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-dynamics-365-business-central-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0\nscopes:\n- scope: https://api.businesscentral.dynamics.com/.default\n  description: Business Central API access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-dynamics-365-business-central-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/scopes/microsoft-dynamics-365-business-central-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- ERP
- Cloud ERP
- Finance
- Accounting
- Supply Chain
- Operations
- Small Business
- Mid-Market
- Microsoft Dynamics 365
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
