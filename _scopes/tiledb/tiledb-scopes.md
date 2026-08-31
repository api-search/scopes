---
api_specs:
- filename: tiledb-cloud-v1-openapi.yaml
  format: yaml
  label: TileDB Storage Platform API (v1)
  slug: tiledb-storage-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-cloud-v1-openapi.yaml
- filename: tiledb-cloud-v2-openapi.yaml
  format: yaml
  label: TileDB Storage Platform API (v2)
  slug: tiledb-storage-platform-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-cloud-v2-openapi.yaml
authorization_urls:
- https://oauth2.tiledb.com/oauth2/authorize
description: ''
docs: https://documentation.cloud.tiledb.com/academy/accounts/individual/profile/api-tokens/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tiledb Scopes
name_suffix: OAuth Scopes
note: Two distinct scope surfaces. (1) The OAuth 2.0 authorization-code flow declared in securityDefinitions carries three coarse scopes (read/write/admin); note that the spec comments the OAuth2 requirement out of the global security block because it broke the generated Python client, so in practice callers use the X-TILEDB-REST-API-KEY header or HTTP Basic. (2) REST API tokens minted at POST /v1/token carry the finer TokenScope enum below, which the console exposes as the token 'Scope' field. Tokens default to all permissions ('*') and to a 30-minute expiry when none is given.
overview: 'TileDB publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TileDB API on a user''s behalf.


  Tokens are issued from https://oauth2.tiledb.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TileDB
provider_slug: tiledb
schemes:
- flows:
  - authorizationUrl: https://oauth2.tiledb.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://oauth2.tiledb.com/oauth2/token
  name: OAuth2
  source: openapi/tiledb-cloud-v1-openapi.yaml
- flows:
  - authorizationUrl: https://oauth2.tiledb.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://oauth2.tiledb.com/oauth2/token
  name: OAuth2
  source: openapi/tiledb-cloud-v2-openapi.yaml
scope_count: 3
scope_names:
- admin
- read
- write
scopes:
- description: Grants read and write access to administrative information
  flows:
  - authorizationCode
  scope: admin
- description: Grants read access
  flows:
  - authorizationCode
  scope: read
- description: Grants write access
  flows:
  - authorizationCode
  scope: write
slug: tiledb-scopes
source_filename: tiledb-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://documentation.cloud.tiledb.com/academy/accounts/individual/profile/api-tokens/ + openapi/tiledb-cloud-v1-openapi.yaml\n  (definitions.TokenScope)\nschemes:\n- name: OAuth2\n  source: openapi/tiledb-cloud-v1-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth2.tiledb.com/oauth2/authorize\n    tokenUrl: https://oauth2.tiledb.com/oauth2/token\n- name: OAuth2\n  source: openapi/tiledb-cloud-v2-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth2.tiledb.com/oauth2/authorize\n    tokenUrl: https://oauth2.tiledb.com/oauth2/token\nscopes:\n- scope: admin\n  description: Grants read and write access to administrative information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tiledb-cloud-v1-openapi.yaml\n  - openapi/tiledb-cloud-v2-openapi.yaml\n- scope: read\n  description: Grants read access\n  flows:\n  - authorizationCode\n  sources:\n \
  \ - openapi/tiledb-cloud-v1-openapi.yaml\n  - openapi/tiledb-cloud-v2-openapi.yaml\n- scope: write\n  description: Grants write access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tiledb-cloud-v1-openapi.yaml\n  - openapi/tiledb-cloud-v2-openapi.yaml\ndocs: https://documentation.cloud.tiledb.com/academy/accounts/individual/profile/api-tokens/\nnote: Two distinct scope surfaces. (1) The OAuth 2.0 authorization-code flow declared in securityDefinitions carries\n  three coarse scopes (read/write/admin); note that the spec comments the OAuth2 requirement out of the global security\n  block because it broke the generated Python client, so in practice callers use the X-TILEDB-REST-API-KEY header\n  or HTTP Basic. (2) REST API tokens minted at POST /v1/token carry the finer TokenScope enum below, which the console\n  exposes as the token 'Scope' field. Tokens default to all permissions ('*') and to a 30-minute expiry when none\n  is given.\napi_token_scopes:\n  mint_operation: createToken\
  \ (POST /v1/token)\n  list_operation: getTokenScopes (GET /v1/tokens/scopes)\n  revoke_operation: revokeToken (DELETE /v1/tokens/{token})\n  default: '*'\n  default_expiry: 30 minutes when no expires value is supplied\n  source: openapi/tiledb-cloud-v1-openapi.yaml definitions.TokenScope\n  scopes:\n  - scope: '*'\n    description: All permissions. The default when no scope is supplied on a token request.\n  - scope: password_reset\n    description: Limited to the password-reset flow (POST /v1/user/password_reset).\n  - scope: confirm_email\n    description: Limited to the email-confirmation flow (POST /v1/user/confirm_email).\n  - scope: user:read\n    description: Read the authenticated user profile and user-scoped listings.\n  - scope: user:read-write\n    description: Read and modify the authenticated user profile.\n  - scope: user:admin\n    description: Administrative access to user records.\n  - scope: array:read\n    description: Read arrays, array schemas, metadata and array activity.\n\
  \  - scope: array:read-write\n    description: Read and write arrays, including register/deregister and metadata writes.\n  - scope: array:admin\n    description: Administrative access to arrays, including delete and sharing.\n  - scope: organization:read\n    description: Read organization profile and membership.\n  - scope: organization:read-write\n    description: Read and modify organization profile and membership.\n  - scope: organization:admin\n    description: Administrative access to an organization, including billing and deletion.\n  - scope: group:read\n    description: Read groups and group contents.\n  - scope: group:read-write\n    description: Read and modify groups and group contents.\n  - scope: group:admin\n    description: Administrative access to groups, including delete and sharing.\nrelated_permission_enums:\n  note: Not token scopes — the per-asset action enums the sharing/permission endpoints accept.\n  ArrayActions:\n  - read\n  - write\n  - edit\n  - read_array_logs\n\
  \  - read_array_info\n  - read_array_schema\n  GroupActions:\n  - read\n  - write\n  - edit\n  UDFActions:\n  - fetch_udf\n  - share_udf\n  TaskGraphActions:\n  - fetch_task_graph\n  - share_task_graph\n  NamespaceActions:\n  - read\n  - write\n  - create\n  - delete\n  - edit\n  - read_array_logs\n  - read_job_logs\n  - read_object_logs\n  - run_job\n  - delete_organization\n  - edit_organization\n  - edit_billing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/scopes/tiledb-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Database
- Multimodal Data
- Life Sciences
- Genomics
- Single Cell
- Biomedical Imaging
- Vector Search
- Data Management
- Cloud Storage
- Analytics
- Machine-Learning
token_urls:
- https://oauth2.tiledb.com/oauth2/token
---
