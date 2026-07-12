---
authorization_urls: []
description: ''
docs: https://docs.cribl.io/cribl-as-code/api-auth/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Cribl Scopes
name_suffix: OAuth Scopes
note: Cribl uses the OAuth 2.0 client credentials flow only; clients do not request scopes. The scope attribute of the Bearer token reflects the IAM Permissions assigned to the API Credential (Organization Admin/Owner/User plus per-Workspace product permissions), and Cribl publishes only example scope strings rather than a complete scopes catalog (https://docs.cribl.io/cribl-as-code/api-auth/, https://docs.cribl.io/iam/permissions/).
overview: 'Cribl publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cribl API on a user''s behalf.


  Tokens are issued from https://login.cribl.cloud/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cribl
provider_slug: cribl
schemes:
- description: OAuth 2.0 client credentials flow for Cribl Cloud management plane authentication.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.cribl.cloud/oauth/token
  name: oauth2
  source: openapi/cribl-as-code-api-openapi.yml
- description: OAuth 2.0 client credentials flow for Cribl Cloud authentication. Tokens expire after 24 hours.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.cribl.cloud/oauth/token
  name: oauth2
  source: openapi/cribl-cloud-api-openapi.yml
scope_count: 6
scope_names:
- user:read:workergroups
- user:update:workergroups
- user:read:connections
- user:update:connections
- user:read:workspaces
- user:update:workspaces
scopes:
- description: Read Worker Group data in the Workspaces the API Credential's permissions cover.
  flows: []
  scope: user:read:workergroups
- description: Modify Worker Group configurations in the Workspaces the API Credential's permissions cover.
  flows: []
  scope: user:update:workergroups
- description: Read connection information in the Workspaces the API Credential's permissions cover.
  flows: []
  scope: user:read:connections
- description: Modify connection settings in the Workspaces the API Credential's permissions cover.
  flows: []
  scope: user:update:connections
- description: View Workspace data in the Cribl.Cloud Organization.
  flows: []
  scope: user:read:workspaces
- description: Change Workspace configurations in the Cribl.Cloud Organization.
  flows: []
  scope: user:update:workspaces
slug: cribl-scopes
source_filename: cribl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://docs.cribl.io/cribl-as-code/api-auth/\nnote: Cribl uses the OAuth 2.0 client credentials flow only; clients do not request\n  scopes. The scope attribute of the Bearer token reflects the IAM Permissions assigned\n  to the API Credential (Organization Admin/Owner/User plus per-Workspace product\n  permissions), and Cribl publishes only example scope strings rather than a complete\n  scopes catalog (https://docs.cribl.io/cribl-as-code/api-auth/, https://docs.cribl.io/iam/permissions/).\nsource: openapi/cribl-as-code-api-openapi.yml, openapi/cribl-cloud-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cribl-as-code-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.cribl.cloud/oauth/token\n  description: OAuth 2.0 client credentials flow for Cribl Cloud management plane authentication.\n- name: oauth2\n  source: openapi/cribl-cloud-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://login.cribl.cloud/oauth/token\n  description: OAuth 2.0 client credentials flow for Cribl Cloud authentication. Tokens expire\n    after 24 hours.\nscopes:\n- scope: user:read:workergroups\n  description: Read Worker Group data in the Workspaces the API Credential's permissions\n    cover.\n  sources:\n  - https://docs.cribl.io/cribl-as-code/api-auth/\n- scope: user:update:workergroups\n  description: Modify Worker Group configurations in the Workspaces the API Credential's\n    permissions cover.\n  sources:\n  - https://docs.cribl.io/cribl-as-code/api-auth/\n- scope: user:read:connections\n  description: Read connection information in the Workspaces the API Credential's\n    permissions cover.\n  sources:\n  - https://docs.cribl.io/cribl-as-code/api-auth/\n- scope: user:update:connections\n  description: Modify connection settings in the Workspaces the API Credential's\n    permissions cover.\n  sources:\n  - https://docs.cribl.io/cribl-as-code/api-auth/\n- scope:\
  \ user:read:workspaces\n  description: View Workspace data in the Cribl.Cloud Organization.\n  sources:\n  - https://docs.cribl.io/cribl-as-code/api-auth/\n- scope: user:update:workspaces\n  description: Change Workspace configurations in the Cribl.Cloud Organization.\n  sources:\n  - https://docs.cribl.io/cribl-as-code/api-auth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/scopes/cribl-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Configuration
- Data Lake
- Data Pipelines
- Data Routing
- Edge Computing
- Infrastructure as Code
- Observability
- Search
- Security Data
- Stream Processing
- Telemetry
token_urls:
- https://login.cribl.cloud/oauth/token
---
