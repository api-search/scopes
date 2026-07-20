---
api_specs:
- filename: powerbi.json
  format: json
  label: Power BI REST API
  slug: power-bi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/powerbi/data-plane/Microsoft.PowerBI/stable/v1.0/powerbi.json
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Power Bi Scopes
name_suffix: OAuth Scopes
note: Power BI authorizes via Microsoft Entra ID (Azure AD) OAuth 2.0. The curated OpenAPI declares only an http-bearer scheme, so no scopes are derivable from the spec; the scopes below are the documented Power BI Service delegated permissions requested against the resource https://analysis.windows.net/powerbi/api. Application permissions (client-credentials) use .default and are governed by tenant admin settings.
overview: 'Power BI publishes 17 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Power BI API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Power BI
provider_slug: power-bi
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    note: Uses the .default scope; requires tenant admin consent and Power BI service admin settings.
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: AzureADOAuth2
  type: oauth2
scope_count: 17
scope_names:
- https://analysis.windows.net/powerbi/api/.default
- Dataset.Read.All
- Dataset.ReadWrite.All
- Report.Read.All
- Report.ReadWrite.All
- Dashboard.Read.All
- Dashboard.ReadWrite.All
- Workspace.Read.All
- Workspace.ReadWrite.All
- Gateway.Read.All
- Gateway.ReadWrite.All
- Content.Create
- Tenant.Read.All
- Tenant.ReadWrite.All
- App.Read.All
- Capacity.Read.All
- Capacity.ReadWrite.All
scopes:
- description: Request all statically consented permissions (used by client-credentials / app-only flows).
  flows:
  - clientCredentials
  - authorizationCode
  scope: https://analysis.windows.net/powerbi/api/.default
- description: View all datasets.
  flows:
  - authorizationCode
  scope: Dataset.Read.All
- description: Read and write all datasets.
  flows:
  - authorizationCode
  scope: Dataset.ReadWrite.All
- description: View all reports.
  flows:
  - authorizationCode
  scope: Report.Read.All
- description: Read and write all reports (clone, rebind, export, delete).
  flows:
  - authorizationCode
  scope: Report.ReadWrite.All
- description: View all dashboards and tiles.
  flows:
  - authorizationCode
  scope: Dashboard.Read.All
- description: Read and write all dashboards.
  flows:
  - authorizationCode
  scope: Dashboard.ReadWrite.All
- description: View all workspaces (groups).
  flows:
  - authorizationCode
  scope: Workspace.Read.All
- description: Read and write all workspaces (create, delete, manage users).
  flows:
  - authorizationCode
  scope: Workspace.ReadWrite.All
- description: View all on-premises data gateways and their datasources.
  flows:
  - authorizationCode
  scope: Gateway.Read.All
- description: Read and write all gateways and datasources.
  flows:
  - authorizationCode
  scope: Gateway.ReadWrite.All
- description: Create content such as workspaces, datasets, and reports.
  flows:
  - authorizationCode
  scope: Content.Create
- description: View all content in the tenant (admin/read-only; requires Power BI admin).
  flows:
  - authorizationCode
  scope: Tenant.Read.All
- description: Read and write all content in the tenant (admin).
  flows:
  - authorizationCode
  scope: Tenant.ReadWrite.All
- description: View all Power BI apps.
  flows:
  - authorizationCode
  scope: App.Read.All
- description: View all capacities.
  flows:
  - authorizationCode
  scope: Capacity.Read.All
- description: Read and write all capacities.
  flows:
  - authorizationCode
  scope: Capacity.ReadWrite.All
slug: power-bi-scopes
source_filename: power-bi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: Microsoft Entra ID (Azure AD) Power BI Service delegated permissions reference\ndocs: https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app\nresource: https://analysis.windows.net/powerbi/api\nnote: >-\n  Power BI authorizes via Microsoft Entra ID (Azure AD) OAuth 2.0. The curated\n  OpenAPI declares only an http-bearer scheme, so no scopes are derivable from\n  the spec; the scopes below are the documented Power BI Service delegated\n  permissions requested against the resource\n  https://analysis.windows.net/powerbi/api. Application permissions\n  (client-credentials) use .default and are governed by tenant admin settings.\nschemes:\n  - name: AzureADOAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n        tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n      - flow: clientCredentials\n\
  \        tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n        note: Uses the .default scope; requires tenant admin consent and Power BI service admin settings.\nscopes:\n  - scope: https://analysis.windows.net/powerbi/api/.default\n    description: Request all statically consented permissions (used by client-credentials / app-only flows).\n    flows: [clientCredentials, authorizationCode]\n  - scope: Dataset.Read.All\n    description: View all datasets.\n    flows: [authorizationCode]\n  - scope: Dataset.ReadWrite.All\n    description: Read and write all datasets.\n    flows: [authorizationCode]\n  - scope: Report.Read.All\n    description: View all reports.\n    flows: [authorizationCode]\n  - scope: Report.ReadWrite.All\n    description: Read and write all reports (clone, rebind, export, delete).\n    flows: [authorizationCode]\n  - scope: Dashboard.Read.All\n    description: View all dashboards and tiles.\n    flows: [authorizationCode]\n  - scope: Dashboard.ReadWrite.All\n\
  \    description: Read and write all dashboards.\n    flows: [authorizationCode]\n  - scope: Workspace.Read.All\n    description: View all workspaces (groups).\n    flows: [authorizationCode]\n  - scope: Workspace.ReadWrite.All\n    description: Read and write all workspaces (create, delete, manage users).\n    flows: [authorizationCode]\n  - scope: Gateway.Read.All\n    description: View all on-premises data gateways and their datasources.\n    flows: [authorizationCode]\n  - scope: Gateway.ReadWrite.All\n    description: Read and write all gateways and datasources.\n    flows: [authorizationCode]\n  - scope: Content.Create\n    description: Create content such as workspaces, datasets, and reports.\n    flows: [authorizationCode]\n  - scope: Tenant.Read.All\n    description: View all content in the tenant (admin/read-only; requires Power BI admin).\n    flows: [authorizationCode]\n  - scope: Tenant.ReadWrite.All\n    description: Read and write all content in the tenant (admin).\n   \
  \ flows: [authorizationCode]\n  - scope: App.Read.All\n    description: View all Power BI apps.\n    flows: [authorizationCode]\n  - scope: Capacity.Read.All\n    description: View all capacities.\n    flows: [authorizationCode]\n  - scope: Capacity.ReadWrite.All\n    description: Read and write all capacities.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/scopes/power-bi-scopes.yml
summary_line: 17 scopes · authorizationCode/clientCredentials
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
