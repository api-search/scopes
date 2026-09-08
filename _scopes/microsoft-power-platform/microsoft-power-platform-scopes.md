---
api_specs:
- filename: microsoft-power-platform-metadata-api-openapi.yml
  format: yaml
  label: Microsoft Power Platform Metadata API
  slug: microsoft-power-platform-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/microsoft-power-platform-metadata-api-openapi.yml
- filename: microsoft-power-platform-records-api-openapi.yml
  format: yaml
  label: Microsoft Power Platform Records API
  slug: microsoft-power-platform-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/microsoft-power-platform-records-api-openapi.yml
- filename: microsoft-power-platform-enterprise-policies-openapi.json
  format: json
  label: Power Platform Enterprise Policies (Azure Resource Manager)
  slug: microsoft-power-platform-enterprise-policies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/_original/microsoft-power-platform-enterprise-policies-openapi.json
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: https://learn.microsoft.com/en-us/power-platform/admin/programmability-permission-reference
flows:
- authorizationCode
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Power Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Power Platform publishes 5 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Power Platform API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Power Platform
provider_slug: microsoft-power-platform
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  provider: Microsoft Entra ID
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  provider: Microsoft Entra ID
  resource: https://management.azure.com
scope_count: 5
scope_names:
- https://{org}.api.crm.dynamics.com/.default
- https://{org}.api.crm.dynamics.com/user_impersonation
- https://api.powerplatform.com/.default
- mcp.tools
- user_impersonation
scopes:
- description: All permissions the calling principal has been granted on that Dataverse environment. Actual reach is decided by the security role on the user or application user, not by the scope.
  flows:
  - authorizationCode
  - clientCredentials
  scope: https://{org}.api.crm.dynamics.com/.default
- description: Delegated access to Dataverse on behalf of the signed-in user.
  flows:
  - authorizationCode
  scope: https://{org}.api.crm.dynamics.com/user_impersonation
- description: Tenant administration surface. Which namespaces the token can actually reach is governed by the Power Platform admin permission reference.
  flows:
  - authorizationCode
  - clientCredentials
  scope: https://api.powerplatform.com/.default
- description: Delegated permission that grants an MCP client access to the Dataverse MCP server. Granting it is not sufficient on its own - the client's application id must also be added to the environment's allowed MCP clients list in the Power Platform admin center.
  flows:
  - authorizationCode
  scope: mcp.tools
- description: Azure Resource Manager impersonation, declared in Microsoft's Swagger for the Microsoft.PowerPlatform provider. Governs enterprise policies, accounts and private link.
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-power-platform-scopes
source_filename: microsoft-power-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  Derived baseline from openapi/microsoft-power-platform-metadata-api-openapi.yml and\n  openapi/microsoft-power-platform-records-api-openapi.yml, then enriched from\n  https://learn.microsoft.com/en-us/power-platform/admin/programmability-authentication-v2,\n  https://learn.microsoft.com/en-us/power-platform/admin/programmability-permission-reference and\n  https://learn.microsoft.com/en-us/power-apps/maker/data-platform/data-platform-mcp-other-clients\n  (all HTTP 200, fetched 2026-09-06)\ndocs: https://learn.microsoft.com/en-us/power-platform/admin/programmability-permission-reference\nmodel: >-\n  Power Platform uses resource-scoped Entra ID permissions, not a fine-grained scope catalogue.\n  For machine-to-machine access you request the resource's /.default scope and the real\n  authorization decision is made by the Dataverse security role or Power Platform admin role\n  attached to the principal inside the environment.\
  \ That is why this list is short and the\n  permission reference, not this file, is where the granularity lives.\nschemes:\n- name: oauth2\n  provider: Microsoft Entra ID\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: azure_auth\n  provider: Microsoft Entra ID\n  resource: https://management.azure.com\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscopes:\n- scope: https://{org}.api.crm.dynamics.com/.default\n  resource: Microsoft Dataverse Web API\n  description: >-\n    All permissions the calling principal has been granted on that Dataverse environment. Actual\n    reach is decided by the security role on the user or application user, not by the scope.\n \
  \ flows: [authorizationCode, clientCredentials]\n- scope: https://{org}.api.crm.dynamics.com/user_impersonation\n  resource: Microsoft Dataverse Web API\n  description: Delegated access to Dataverse on behalf of the signed-in user.\n  flows: [authorizationCode]\n- scope: https://api.powerplatform.com/.default\n  resource: Power Platform API\n  description: >-\n    Tenant administration surface. Which namespaces the token can actually reach is governed by\n    the Power Platform admin permission reference.\n  flows: [authorizationCode, clientCredentials]\n- scope: mcp.tools\n  resource: Dynamics CRM (Dataverse MCP server)\n  description: >-\n    Delegated permission that grants an MCP client access to the Dataverse MCP server. Granting\n    it is not sufficient on its own - the client's application id must also be added to the\n    environment's allowed MCP clients list in the Power Platform admin center.\n  flows: [authorizationCode]\n- scope: user_impersonation\n  resource: https://management.azure.com\n\
  \  description: >-\n    Azure Resource Manager impersonation, declared in Microsoft's Swagger for the\n    Microsoft.PowerPlatform provider. Governs enterprise policies, accounts and private link.\n  flows: [implicit]\nconsent:\n  tenant_admin_required: true\n  note: >-\n    A tenant administrator must grant admin consent before a client can authenticate. Microsoft\n    publishes the consent URL form\n    https://login.microsoftonline.com/{tenant-id}/adminconsent?client_id={client-id} and, for its\n    own Dataverse CLI proxy, the app id 0c412cc3-0dd6-449b-987f-05b053db9457.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/scopes/microsoft-power-platform-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials/implicit
tags:
- Dataverse
- Low-Code
- Microsoft
- Power Apps
- Power Automate
- Power BI
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
