---
api_specs:
- filename: acceldata-alerts-api-openapi.yml
  format: yaml
  label: Acceldata Alerts API
  slug: acceldata-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-alerts-api-openapi.yml
- filename: acceldata-data-quality-rules-api-openapi.yml
  format: yaml
  label: Acceldata Data Quality Rules API
  slug: acceldata-data-quality-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-data-quality-rules-api-openapi.yml
- filename: acceldata-datasets-api-openapi.yml
  format: yaml
  label: Acceldata Datasets API
  slug: acceldata-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-datasets-api-openapi.yml
- filename: acceldata-lineage-api-openapi.yml
  format: yaml
  label: Acceldata Lineage API
  slug: acceldata-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-lineage-api-openapi.yml
- filename: acceldata-pipeline-jobs-api-openapi.yml
  format: yaml
  label: Acceldata Pipeline Jobs API
  slug: acceldata-pipeline-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-pipeline-jobs-api-openapi.yml
- filename: acceldata-roles-api-openapi.yml
  format: yaml
  label: Acceldata Roles API
  slug: acceldata-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-roles-api-openapi.yml
- filename: acceldata-users-api-openapi.yml
  format: yaml
  label: Acceldata Users API
  slug: acceldata-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-users-api-openapi.yml
- filename: acceldata-catalog-api-openapi.json
  format: json
  label: Acceldata Catalog API
  slug: acceldata-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/_original/acceldata-catalog-api-openapi.json
- filename: acceldata-administration-api-openapi.json
  format: json
  label: Acceldata Administration API
  slug: acceldata-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/_original/acceldata-administration-api-openapi.json
- filename: acceldata-tags-api-openapi.json
  format: json
  label: Acceldata Tag Services API
  slug: acceldata-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/_original/acceldata-tags-api-openapi.json
authorization_urls: []
description: ''
docs: https://docs.acceldata.io/documentation/roles-and-permissions
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Acceldata Scopes
name_suffix: OAuth Scopes
note: 'Acceldata does NOT authorize its platform APIs with OAuth 2.0 scopes. Authentication is a static accessKey/secretKey header pair, and authorization is an RBAC permission model attached to the calling identity. The permissions below are not invented: every one is named verbatim in a published operation description ("Requires MODIFY_USERS permission", "Authorization: requires ASSET_VIEW and ASSET_METADATA_VIEW"), and the count is the number of published operations that name it. Roles are assembled from these permissions in the ADOC UI at Control Center > Access Management. derive-oauth-scopes.py was run first and correctly reported 0 oauth2 schemes; this file is the searched replacement that records the authorization model that actually exists.'
overview: 'Acceldata uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Acceldata
provider_slug: acceldata
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: acceldata-scopes
source_filename: acceldata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: openapi/_original/*.json operation descriptions + https://docs.acceldata.io/documentation/roles-and-permissions\ndocs: https://docs.acceldata.io/documentation/roles-and-permissions\nmodel: rbac-permissions\nnote: >-\n  Acceldata does NOT authorize its platform APIs with OAuth 2.0 scopes. Authentication is a\n  static accessKey/secretKey header pair, and authorization is an RBAC permission model\n  attached to the calling identity. The permissions below are not invented: every one is\n  named verbatim in a published operation description (\"Requires MODIFY_USERS permission\",\n  \"Authorization: requires ASSET_VIEW and ASSET_METADATA_VIEW\"), and the count is the number\n  of published operations that name it. Roles are assembled from these permissions in the\n  ADOC UI at Control Center > Access Management.\n  derive-oauth-scopes.py was run first and correctly reported 0 oauth2 schemes; this file\n  is the searched replacement\
  \ that records the authorization model that actually exists.\nrole_model:\n  tiers:\n  - name: Tenant Roles\n    scope: platform-wide\n    examples:\n    - tenant_admin\n    - viewer\n    - owner\n    categories:\n    - Administration (User Management, API Keys, Billing, Account Configuration)\n    - Alerts\n    - Compute\n    - Pipeline\n    - Data Products\n    - Reliability\n  - name: Domain Roles\n    scope: per-domain / per-resource\n    examples:\n    - asset_viewer\n    - report_admin\n    - domain_editor\n    categories:\n    - Asset Management\n    - Domain Management\n    - Report Management\n  actions:\n  - Create\n  - Modify\n  - View\n  scim_managed: >-\n    Users and groups provisioned through SCIM are synced from the identity provider and\n    cannot be modified, renamed or deleted through the Administration API (403).\npermissions:\n- name: ASSET_VIEW\n  domain: catalog\n  action: view\n  operations: 91\n  description: Read assets, their metadata, schema, samples, relationships\
  \ and lineage.\n- name: ASSET_METADATA_VIEW\n  domain: catalog\n  action: view\n  operations: 1\n  description: Read the metadata document attached to an asset. Required alongside ASSET_VIEW on getAssetMetadata.\n- name: ASSET_CONFIGURATION_MODIFY\n  domain: catalog\n  action: modify\n  operations: 4\n  description: Change asset-level configuration such as incremental strategies and sampling settings.\n- name: POLICY_VIEW\n  domain: reliability\n  action: view\n  operations: 39\n  description: Read data quality, reconciliation, data drift, schema drift, freshness and anomaly policies.\n- name: POLICY_MODIFY\n  domain: reliability\n  action: modify\n  operations: 26\n  description: Update, enable, disable, schedule or delete an existing policy.\n- name: POLICY_CREATE\n  domain: reliability\n  action: create\n  operations: 5\n  description: Create a new reliability policy of any supported type.\n- name: POLICY_EXECUTE\n  domain: reliability\n  action: execute\n  operations: 4\n  description:\
  \ Trigger a policy execution and cancel an in-flight run.\n- name: POLICY_GROUP_VIEW\n  domain: reliability\n  action: view\n  operations: 1\n  description: Read policy groups / rulesets.\n- name: TAGS_VIEW\n  domain: governance\n  action: view\n  operations: 3\n  description: Read tag keys, tag values and tag associations.\n- name: TAGS_CREATE\n  domain: governance\n  action: create\n  operations: 2\n  description: Create a tag key (GOVERNED or USER) and its initial values.\n- name: TAGS_MODIFY\n  domain: governance\n  action: modify\n  operations: 2\n  description: Attach, detach or edit tags on catalog entities.\n- name: USER_DEFINED_FUNCTION_VIEW\n  domain: governance\n  action: view\n  operations: 2\n  description: Read user-defined functions and templates (UDF/UDT).\n- name: USER_DEFINED_FUNCTION_CREATE\n  domain: governance\n  action: create\n  operations: 1\n  description: Create a user-defined function or template.\n- name: USER_DEFINED_FUNCTION_MODIFY\n  domain: governance\n\
  \  action: modify\n  operations: 2\n  description: Update or delete a user-defined function or template.\n- name: VIEW_USERS\n  domain: administration\n  action: view\n  operations: 3\n  description: List and read users in the tenant.\n- name: MODIFY_USERS\n  domain: administration\n  action: modify\n  operations: 4\n  description: Update or remove users. Blocked (403) for SCIM-managed users.\n- name: VIEW_USER_GROUPS\n  domain: administration\n  action: view\n  operations: 5\n  description: List and read user groups.\n- name: MODIFY_USER_GROUPS\n  domain: administration\n  action: modify\n  operations: 4\n  description: Create, rename, delete groups and change group membership. Blocked for SCIM-managed groups.\n- name: CREATE_USER_GROUPS\n  domain: administration\n  action: create\n  operations: 1\n  description: Create a new user group.\n- name: VIEW_SERVICE_USERS\n  domain: administration\n  action: view\n  operations: 2\n  description: List and read service (machine) users.\n- name:\
  \ CREATE_SERVICE_USERS\n  domain: administration\n  action: create\n  operations: 1\n  description: Create a service user.\n- name: MODIFY_SERVICE_USERS\n  domain: administration\n  action: modify\n  operations: 5\n  description: Update, disable or delete a service user and its role mappings.\n- name: VIEW_API_KEYS\n  domain: administration\n  action: view\n  operations: 1\n  description: List issued API keys and their metadata.\n- name: MODIFY_API_KEYS\n  domain: administration\n  action: modify\n  operations: 3\n  description: Issue and revoke API keys.\n- name: VIEW_ROLE\n  domain: administration\n  action: view\n  operations: 6\n  description: Read tenant and domain role definitions and their permission sets.\noauth_scopes:\n- scope: mcp\n  issuer: https://documentation.acceldata.io\n  applies_to: https://documentation.acceldata.io/mcp/rpc\n  source: https://documentation.acceldata.io/.well-known/oauth-authorization-server\n  note: >-\n    The only OAuth scope Acceldata publishes anywhere.\
  \ It protects the documentation MCP\n    endpoint, not the ADOC platform APIs, and the endpoint currently answers anonymously.\nsummary:\n  oauth2_scopes_on_platform_api: 0\n  rbac_permissions: 25\n  permission_named_operations: 140\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/scopes/acceldata-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
token_urls: []
---
