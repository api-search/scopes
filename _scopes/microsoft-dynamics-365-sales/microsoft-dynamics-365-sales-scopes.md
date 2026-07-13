---
api_specs:
- filename: microsoft-dynamics-365-sales-openapi.yml
  format: yaml
  label: Microsoft Dataverse Web API (Dynamics 365 Sales)
  slug: dataverse-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-openapi.yml
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
name: Microsoft Dynamics 365 Sales Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Dynamics 365 Sales publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Dynamics 365 Sales API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Dynamics 365 Sales
provider_slug: microsoft-dynamics-365-sales
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-dynamics-365-sales-openapi.yml
scope_count: 1
scope_names:
- https://{org}.api.crm.dynamics.com/.default
scopes:
- description: Dataverse environment access
  flows:
  - authorizationCode
  - clientCredentials
  scope: https://{org}.api.crm.dynamics.com/.default
slug: microsoft-dynamics-365-sales-scopes
source_filename: microsoft-dynamics-365-sales-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-dynamics-365-sales-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-dynamics-365-sales-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\nscopes:\n- scope: https://{org}.api.crm.dynamics.com/.default\n  description: Dataverse environment access\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/microsoft-dynamics-365-sales-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/scopes/microsoft-dynamics-365-sales-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- CRM
- Sales
- Customer Relationship Management
- Dynamics 365
- Microsoft
- Dataverse
- OData
- Sales Automation
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
