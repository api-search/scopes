---
api_specs:
- filename: cdata-rest-api-openapi.yml
  format: yaml
  label: CData SQL API
  slug: sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-openapi.yml
- filename: cdata-rest-api-openapi.yml
  format: yaml
  label: CData Metadata API
  slug: metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-openapi.yml
- filename: cdata-rest-api-openapi.yml
  format: yaml
  label: CData Log API
  slug: log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-openapi.yml
- filename: cdata-rest-api-embedded-openapi.yml
  format: yaml
  label: CData Connection API
  slug: connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-embedded-openapi.yml
- filename: cdata-rest-api-embedded-openapi.yml
  format: yaml
  label: CData Job API
  slug: job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-embedded-openapi.yml
- filename: cdata-rest-api-embedded-openapi.yml
  format: yaml
  label: CData Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-embedded-openapi.yml
- filename: cdata-rest-api-openapi.yml
  format: yaml
  label: CData Audit API
  slug: audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-openapi.yml
- filename: cdata-odata-api-openapi.yml
  format: yaml
  label: CData OData API
  slug: odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-odata-api-openapi.yml
- filename: cdata-mcp-api-openapi.yml
  format: yaml
  label: CData Connect AI MCP Server
  slug: mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-mcp-api-openapi.yml
- filename: cdata-management-api-openapi.yml
  format: yaml
  label: CData Connect AI Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-management-api-openapi.yml
- filename: cdata-mcp-api-embedded-openapi.yml
  format: yaml
  label: CData Connect AI Embed MCP Server
  slug: mcp-embedded
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-mcp-api-embedded-openapi.yml
- filename: cdata-openapi-api-openapi.yml
  format: yaml
  label: CData Connect AI OpenAPI API
  slug: openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-openapi-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.cloud.cdata.com/en/API/Management-API.md
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Cdata Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CData publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CData API on a user''s behalf.


  Tokens are issued from https://cloud-login.cdata.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CData
provider_slug: cdata
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://cloud-login.cdata.com/oauth/token
  name: oauth2
  source: openapi/cdata-management-api-openapi.yml
scope_count: 4
scope_names:
- management:service-accounts:read
- management:service-accounts:write
- management:users:read
- management:users:write
scopes:
- description: Read access to service account resources.
  flows:
  - clientCredentials
  scope: management:service-accounts:read
- description: Write access to service account resources.
  flows:
  - clientCredentials
  scope: management:service-accounts:write
- description: Read access to user resources.
  flows:
  - clientCredentials
  scope: management:users:read
- description: Write access to user resources.
  flows:
  - clientCredentials
  scope: management:users:write
slug: cdata-scopes
source_filename: cdata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/cdata-management-api-openapi.yml\ndocs: https://docs.cloud.cdata.com/en/API/Management-API.md\nschemes:\n- name: oauth2\n  source: openapi/cdata-management-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cloud-login.cdata.com/oauth/token\nscopes:\n- scope: management:service-accounts:read\n  description: Read access to service account resources.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cdata-management-api-openapi.yml\n- scope: management:service-accounts:write\n  description: Write access to service account resources.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cdata-management-api-openapi.yml\n- scope: management:users:read\n  description: Read access to user resources.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cdata-management-api-openapi.yml\n- scope: management:users:write\n  description: Write access to user resources.\n  flows:\n  -\
  \ clientCredentials\n  sources:\n  - openapi/cdata-management-api-openapi.yml\n\n# --- SEARCHED enrichment, 2026-09-05 -------------------------------------------------\n# The four scopes above are the complete set the Management API declares. CData publishes\n# no separate scopes/permissions reference page: the Management API doc page and the\n# securitySchemes block in the spec are the only published statements of them, and they\n# agree. Nothing was added that the provider does not declare.\nscope_model:\n  granularity: resource + verb\n  pattern: 'management:<resource>:<read|write>'\n  resources: [users, service-accounts]\n  note: >-\n    Scopes cover the two Management API resource families. Roles and permissions are\n    themselves managed through those endpoints (POST /users/{id}/roles,\n    POST /service-accounts/{id}/permissions) and are governed by the parent resource's\n    write scope rather than by scopes of their own.\n  gap: >-\n    The Connect AI REST API (query, batch,\
  \ exec, metadata, log) and the OData and OpenAPI\n    surfaces declare only HTTP Basic — no OAuth scopes at all. A service-account bearer\n    token from cloud-login.cdata.com is accepted on those endpoints per the Authentication\n    page, but the contract publishes no scope that narrows what such a token may do there.\n    Authorization on the data plane is enforced through Connect AI roles, workspaces and\n    per-connection SELECT/INSERT/UPDATE/DELETE/EXECUTE permissions, which are not expressed\n    as OAuth scopes.\nmcp_scopes:\n  source: well-known/cdata-mcp-oauth-authorization-server.json\n  note: >-\n    The MCP authorization server is a separate issuer with its own scope set — openid,\n    profile, email, offline_access. These are OIDC identity scopes, not data-access scopes:\n    what an MCP session can reach is decided by the authenticated user's Connect AI\n    permissions, not by the scopes requested.\n  scopes: [openid, profile, email, offline_access]\nidentity_provider_scopes:\n\
  \  source: well-known/cdata-cloud-login-openid-configuration.json\n  note: >-\n    The Auth0-hosted identity provider at cloud-login.cdata.com advertises the standard OIDC\n    claim scopes (openid, profile, email, offline_access, name, given_name, family_name,\n    nickname, email_verified, picture, created_at, identities, phone, address). Recorded for\n    completeness; they govern the ID token, not API authorization.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/scopes/cdata-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Data
- Data Access
- Data Connectivity
- Databases
- NoSQL
- SQL
token_urls:
- https://cloud-login.cdata.com/oauth/token
---
