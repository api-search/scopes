---
api_specs:
- filename: datastax-access-list-api-openapi.yml
  format: yaml
  label: DataStax Access List API
  slug: datastax-access-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-access-list-api-openapi.yml
- filename: datastax-authentication-api-openapi.yml
  format: yaml
  label: DataStax Authentication API
  slug: datastax-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-authentication-api-openapi.yml
- filename: datastax-clone-api-openapi.yml
  format: yaml
  label: DataStax Clone API
  slug: datastax-clone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-clone-api-openapi.yml
- filename: datastax-customer-keys-api-openapi.yml
  format: yaml
  label: DataStax Customer Keys API
  slug: datastax-customer-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-customer-keys-api-openapi.yml
- filename: datastax-database-operations-api-openapi.yml
  format: yaml
  label: DataStax Database Operations API
  slug: datastax-database-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-database-operations-api-openapi.yml
- filename: datastax-devops-access-list-api-openapi.yml
  format: yaml
  label: DataStax DevOps Access List API
  slug: datastax-devops-access-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-devops-access-list-api-openapi.yml
- filename: datastax-enterprise-operations-api-openapi.yml
  format: yaml
  label: DataStax Enterprise Operations API
  slug: datastax-enterprise-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-enterprise-operations-api-openapi.yml
- filename: datastax-migrations-api-openapi.yml
  format: yaml
  label: DataStax Migrations API
  slug: datastax-migrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-migrations-api-openapi.yml
- filename: datastax-organization-operations-api-openapi.yml
  format: yaml
  label: DataStax Organization Operations API
  slug: datastax-organization-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-organization-operations-api-openapi.yml
- filename: datastax-pcu-api-openapi.yml
  format: yaml
  label: DataStax PCU API
  slug: datastax-pcu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-pcu-api-openapi.yml
- filename: datastax-private-link-api-openapi.yml
  format: yaml
  label: DataStax Private Link API
  slug: datastax-private-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-private-link-api-openapi.yml
- filename: datastax-regions-api-openapi.yml
  format: yaml
  label: DataStax Regions API
  slug: datastax-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-regions-api-openapi.yml
- filename: datastax-roles-api-openapi.yml
  format: yaml
  label: DataStax Roles API
  slug: datastax-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-roles-api-openapi.yml
- filename: datastax-scim-api-openapi.yml
  format: yaml
  label: DataStax SCIM API
  slug: datastax-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-scim-api-openapi.yml
- filename: datastax-token-api-openapi.yml
  format: yaml
  label: DataStax Token API
  slug: datastax-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-token-api-openapi.yml
- filename: datastax-users-api-openapi.yml
  format: yaml
  label: DataStax Users API
  slug: datastax-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-users-api-openapi.yml
- filename: datastax-vpc-peering-api-openapi.yml
  format: yaml
  label: DataStax VPC Peering API
  slug: datastax-vpc-peering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-vpc-peering-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.datastax.com/en/astra-db-serverless/administration/manage-application-tokens.html
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Datastax Scopes
name_suffix: OAuth Scopes
note: Astra application tokens carry permission scopes (not OAuth2). These scope strings are declared on the BearerAuth security requirement in the DevOps API OpenAPI. Astra also supports fine-grained custom roles; this list captures the built-in permission scopes present in the spec.
overview: 'DataStax publishes 15 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the DataStax API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DataStax
provider_slug: datastax
schemes:
- name: BearerAuth
  source: openapi/datastax-devops-openapi.json
  type: http-bearer
scope_count: 15
scope_names:
- org-admin
- org-db-create
- org-db-terminate
- org-db-view
- org-db-expand
- org-db-suspend
- org-db-addpeering
- org-db-readpeering
- db-keyspace-create
- db-cql
- accesslist-write
- accesslist-read
- db-manage-privateendpoint
- db-manage-telemetry
- db-manage-backupconfiguration
scopes:
- description: Full administrative access to the organization.
  flows: []
  scope: org-admin
- description: Create databases in the organization.
  flows: []
  scope: org-db-create
- description: Terminate databases in the organization.
  flows: []
  scope: org-db-terminate
- description: View databases and their details.
  flows: []
  scope: org-db-view
- description: Resize / expand databases (add capacity or regions).
  flows: []
  scope: org-db-expand
- description: Suspend / park databases.
  flows: []
  scope: org-db-suspend
- description: Add VPC peering / private-link connections.
  flows: []
  scope: org-db-addpeering
- description: Read VPC peering / private-link configuration.
  flows: []
  scope: org-db-readpeering
- description: Create keyspaces within a database.
  flows: []
  scope: db-keyspace-create
- description: Execute CQL against a database.
  flows: []
  scope: db-cql
- description: Create and modify database access lists (IP allowlists).
  flows: []
  scope: accesslist-write
- description: Read database access lists.
  flows: []
  scope: accesslist-read
- description: Manage private endpoints for a database.
  flows: []
  scope: db-manage-privateendpoint
- description: Configure telemetry / metrics export for a database.
  flows: []
  scope: db-manage-telemetry
- description: Manage backup configuration for a database.
  flows: []
  scope: db-manage-backupconfiguration
slug: datastax-scopes
source_filename: datastax-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/datastax-devops-openapi.json\ndocs: https://docs.datastax.com/en/astra-db-serverless/administration/manage-application-tokens.html\nnote: Astra application tokens carry permission scopes (not OAuth2). These scope strings are declared\n  on the BearerAuth security requirement in the DevOps API OpenAPI. Astra also supports fine-grained custom\n  roles; this list captures the built-in permission scopes present in the spec.\nschemes:\n- name: BearerAuth\n  type: http-bearer\n  source: openapi/datastax-devops-openapi.json\nscopes:\n- scope: org-admin\n  description: Full administrative access to the organization.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: org-db-create\n  description: Create databases in the organization.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: org-db-terminate\n  description: Terminate databases in the organization.\n\
  \  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: org-db-view\n  description: View databases and their details.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: org-db-expand\n  description: Resize / expand databases (add capacity or regions).\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: org-db-suspend\n  description: Suspend / park databases.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: org-db-addpeering\n  description: Add VPC peering / private-link connections.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: org-db-readpeering\n  description: Read VPC peering / private-link configuration.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: db-keyspace-create\n  description: Create keyspaces within a database.\n  schemes:\n \
  \ - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: db-cql\n  description: Execute CQL against a database.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: accesslist-write\n  description: Create and modify database access lists (IP allowlists).\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: accesslist-read\n  description: Read database access lists.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: db-manage-privateendpoint\n  description: Manage private endpoints for a database.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: db-manage-telemetry\n  description: Configure telemetry / metrics export for a database.\n  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n- scope: db-manage-backupconfiguration\n  description: Manage backup configuration for a database.\n\
  \  schemes:\n  - BearerAuth\n  sources:\n  - openapi/datastax-devops-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/scopes/datastax-scopes.yml
summary_line: 15 scopes
tags:
- Company
- Enterprise
- Database
- Vector Database
- Cassandra
- Artificial Intelligence
- RAG
- Serverless
- Streaming
- Developer Tools
token_urls: []
---
