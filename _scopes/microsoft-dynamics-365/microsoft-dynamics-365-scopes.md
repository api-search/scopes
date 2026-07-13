---
api_specs:
- filename: $metadata
  format: yaml
  label: Dynamics 365 Sales API
  slug: dynamics-365-sales-api
  spec_type: OpenAPI
  url: https://[org].api.crm.dynamics.com/api/data/v9.2/$metadata
- filename: $metadata
  format: yaml
  label: Dynamics 365 Customer Service API
  slug: dynamics-365-customer-service-api
  spec_type: OpenAPI
  url: https://[org].api.crm.dynamics.com/api/data/v9.2/$metadata
- filename: openapi
  format: yaml
  label: Dynamics 365 Business Central API
  slug: dynamics-365-business-central-api
  spec_type: OpenAPI
  url: https://docs.microsoft.com/dynamics365/business-central/dev-itpro/api-reference/v2.0/openapi
- filename: microsoft-dynamics-365-dataverse-web-api-openapi.yml
  format: yaml
  label: Microsoft Dataverse Web API
  slug: microsoft-dataverse-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365/refs/heads/main/openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Dynamics 365 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Dynamics 365 publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Dynamics 365 API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Dynamics 365
provider_slug: microsoft-dynamics-365
schemes:
- description: OAuth 2.0 authentication using Microsoft Entra ID (Azure Active Directory). Applications must be registered in Microsoft Entra ID and granted the appropriate Dynamics 365 permissions.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml
scope_count: 1
scope_names:
- https://{org}.api.crm.dynamics.com/.default
scopes:
- description: Full access to Dataverse Web API.
  flows:
  - authorizationCode
  scope: https://{org}.api.crm.dynamics.com/.default
slug: microsoft-dynamics-365-scopes
source_filename: microsoft-dynamics-365-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: OAuth 2.0 authentication using Microsoft Entra ID (Azure Active Directory). Applications\n    must be registered in Microsoft Entra ID and granted the appropriate Dynamics 365 permissions.\nscopes:\n- scope: https://{org}.api.crm.dynamics.com/.default\n  description: Full access to Dataverse Web API.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365/refs/heads/main/scopes/microsoft-dynamics-365-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Business Applications
- Cloud
- CRM
- Enterprise
- ERP
- Microsoft
token_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
