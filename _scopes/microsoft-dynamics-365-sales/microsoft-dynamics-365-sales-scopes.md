---
api_specs:
- filename: microsoft-dynamics-365-sales-accounts-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Accounts API
  slug: microsoft-dynamics-365-sales-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-accounts-api-openapi.yml
- filename: microsoft-dynamics-365-sales-batch-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales $batch API
  slug: microsoft-dynamics-365-sales-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-batch-api-openapi.yml
- filename: microsoft-dynamics-365-sales-contacts-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Contacts API
  slug: microsoft-dynamics-365-sales-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-contacts-api-openapi.yml
- filename: microsoft-dynamics-365-sales-invoices-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Invoices API
  slug: microsoft-dynamics-365-sales-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-invoices-api-openapi.yml
- filename: microsoft-dynamics-365-sales-leads-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Leads API
  slug: microsoft-dynamics-365-sales-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-leads-api-openapi.yml
- filename: microsoft-dynamics-365-sales-opportunities-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Opportunities API
  slug: microsoft-dynamics-365-sales-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-opportunities-api-openapi.yml
- filename: microsoft-dynamics-365-sales-products-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Products API
  slug: microsoft-dynamics-365-sales-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-products-api-openapi.yml
- filename: microsoft-dynamics-365-sales-quotes-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Quotes API
  slug: microsoft-dynamics-365-sales-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-quotes-api-openapi.yml
- filename: microsoft-dynamics-365-sales-salesorders-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales SalesOrders API
  slug: microsoft-dynamics-365-sales-salesorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-salesorders-api-openapi.yml
- filename: microsoft-dynamics-365-sales-tasks-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Tasks API
  slug: microsoft-dynamics-365-sales-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-tasks-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: https://learn.microsoft.com/en-us/power-apps/developer/data-platform/authenticate-oauth
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Dynamics 365 Sales Scopes
name_suffix: OAuth Scopes
note: Dataverse does not publish a granular scope catalogue. There are exactly two token scopes, both resource-relative to the environment URL, and authorization is enforced downstream by the Dataverse security model (security roles, table and column privileges) rather than by scope strings. Anything finer-grained than the two scopes below is a security role, not an OAuth scope — see permission_model.
overview: 'Microsoft Dynamics 365 Sales publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Dynamics 365 Sales API on a user''s behalf.


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
  source: openapi/_original/microsoft-dynamics-365-sales-openapi.yml
scope_count: 2
scope_names:
- '{environment-url}/user_impersonation'
- '{environment-url}/.default'
scopes:
- description: Delegated — act on Dataverse as the signed-in user. Learn, verbatim — "use a '<environment-url>/user_impersonation' scope for a public client."
  flows:
  - authorizationCode
  scope: '{environment-url}/user_impersonation'
- description: Application / server-to-server — all statically consented permissions for the resource. Learn, verbatim — "For a confidential client, use a scope of '<environment-url>/.default'."
  flows:
  - clientCredentials
  scope: '{environment-url}/.default'
slug: microsoft-dynamics-365-sales-scopes
source_filename: microsoft-dynamics-365-sales-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/microsoft-dynamics-365-sales-openapi.yml\ndocs: https://learn.microsoft.com/en-us/power-apps/developer/data-platform/authenticate-oauth\ndocs_additional:\n- https://learn.microsoft.com/en-us/power-apps/developer/data-platform/walkthrough-register-app-azure-active-directory\n- https://learn.microsoft.com/en-us/power-platform/admin/manage-application-users\nnote: >-\n  Dataverse does not publish a granular scope catalogue. There are exactly two token scopes,\n  both resource-relative to the environment URL, and authorization is enforced downstream by\n  the Dataverse security model (security roles, table and column privileges) rather than by\n  scope strings. Anything finer-grained than the two scopes below is a security role, not an\n  OAuth scope — see permission_model.\n\nauthority: https://login.microsoftonline.com\nschemes:\n- name: oauth2\n  source: openapi/_original/microsoft-dynamics-365-sales-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n\nscopes:\n- scope: '{environment-url}/user_impersonation'\n  example: https://contoso.api.crm.dynamics.com/user_impersonation\n  description: >-\n    Delegated — act on Dataverse as the signed-in user. Learn, verbatim — \"use a\n    '<environment-url>/user_impersonation' scope for a public client.\"\n  client_type: public\n  flows: [authorizationCode]\n  entra_permission: Access Dynamics 365 as organization users\n  sources: [https://learn.microsoft.com/en-us/power-apps/developer/data-platform/authenticate-oauth]\n- scope: '{environment-url}/.default'\n  example: https://contoso.api.crm.dynamics.com/.default\n  description: >-\n \
  \   Application / server-to-server — all statically consented permissions for the resource.\n    Learn, verbatim — \"For a confidential client, use a scope of\n    '<environment-url>/.default'.\"\n  client_type: confidential\n  flows: [clientCredentials]\n  requires: >-\n    a Dataverse application user bound to the Entra app registration, assigned a custom\n    security role. Does not consume a paid licence.\n  sources: [https://learn.microsoft.com/en-us/power-apps/developer/data-platform/authenticate-oauth]\n\nresource_url_forms:\n- https://{org}.api.crm.dynamics.com\n- https://{org}.crm.dynamics.com\n- note: >-\n    Both forms appear in Microsoft's own samples on the same page — the .api. host in the\n    MSAL scope example and the bare host in the ServiceClient connection-string examples.\n    The region segment varies by datacenter (crm for North America, crm2 South America,\n    crm7 Japan and so on), so the scope string is tenant- and region-specific. Read the\n    exact value from\
  \ Power Apps -> Settings -> Developer resources.\n\npermission_model:\n  kind: role-based, enforced by Dataverse after the token is validated\n  layers:\n  - security roles (assigned to the user or application user)\n  - table (entity) privileges: create, read, write, delete, append, append-to, assign, share\n  - privilege depth: user, business unit, parent-child business unit, organization\n  - column-level security for individual fields\n  impersonation:\n    header: CallerObjectId\n    note: requires the caller to hold the impersonation privilege\n  docs: https://learn.microsoft.com/en-us/power-platform/admin/database-security\n  implication_for_agents: >-\n    A token scope tells you nothing about what an agent may do here. Two callers holding the\n    identical `.default` scope can have completely different effective access. Least\n    privilege is configured as a custom security role on the application user, not as a\n    narrower scope.\n\ncredentials_for_confidential_clients:\n\
  - client secret\n- X.509 certificate (.cer, .pem, .crt public key upload; thumbprint on the client)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/scopes/microsoft-dynamics-365-sales-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
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
