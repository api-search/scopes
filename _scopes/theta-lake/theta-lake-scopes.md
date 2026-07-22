---
api_specs:
- filename: theta-lake-openapi-original.yml
  format: yaml
  label: Theta Lake API
  slug: theta-lake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theta-lake/refs/heads/main/openapi/theta-lake-openapi-original.yml
authorization_urls: []
description: ''
docs: https://developer.thetalake.ai/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Theta Lake Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Theta Lake publishes 70 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Theta Lake API on a user''s behalf.


  Tokens are issued from https://developer.thetalake.ai/api/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Theta Lake
provider_slug: theta-lake
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.thetalake.ai/api/v1/token
  name: ClientCredentials
  source: openapi/theta-lake-openapi-original.yml
  type: oauth2
scope_count: 70
scope_names:
- audit_logs:read
- comments:read
- comments:create
- comments:update
- comments:delete
- cases:read
- cases:create
- cases:update
- cases:add_records
- cases:remove_records
- directory_groups:read
- directory_groups:create
- directory_groups:update
- directory_groups:delete
- exports:read
- identities:read
- identities:create
- identities:update
- identities:delete
- ingestion:read
- ingestion:update
- ingestion:upload
- integrations:read
- labels:read
- labels:create
- labels:update
- labels:delete
- labels:use
- legal_hold:read
- legal_hold:create
- legal_hold:update
- legal_hold:delete
- legal_matter:read
- legal_matter:create
- legal_matter:update
- legal_matter:delete
- org_units:read
- org_units:update
- reconciliation:read
- records:read
- retention_libraries:read
- retention_libraries:create
- retention_libraries:update
- retention_libraries:delete
- roles:read
- roles:create
- roles:update
- roles:delete
- search:read
- search:create
- search:export
- search:reset
- storage_accounts:read
- supervision_spaces:read
- supervision_spaces:create
- supervision_spaces:update
- supervision_spaces:delete
- user_groups:read
- user_groups:create
- user_groups:update
- user_groups:delete
- users:read
- users:create
- users:update
- users:delete
- users:disable
- workflows:read
- workflows:use
- workspace:read
- workspace:update
scopes:
- description: Read audit logs
  flows: []
  scope: audit_logs:read
- description: Read record comments
  flows: []
  scope: comments:read
- description: Create record comments
  flows: []
  scope: comments:create
- description: Update record comments
  flows: []
  scope: comments:update
- description: Delete record comments
  flows: []
  scope: comments:delete
- description: Read cases
  flows: []
  scope: cases:read
- description: Create cases
  flows: []
  scope: cases:create
- description: Update cases
  flows: []
  scope: cases:update
- description: Add records to a case
  flows: []
  scope: cases:add_records
- description: Remove records from a case
  flows: []
  scope: cases:remove_records
- description: Read directory groups
  flows: []
  scope: directory_groups:read
- description: Create directory groups
  flows: []
  scope: directory_groups:create
- description: Update directory groups
  flows: []
  scope: directory_groups:update
- description: Delete directory groups
  flows: []
  scope: directory_groups:delete
- description: Read exports
  flows: []
  scope: exports:read
- description: Read identities
  flows: []
  scope: identities:read
- description: Create identities
  flows: []
  scope: identities:create
- description: Update identities
  flows: []
  scope: identities:update
- description: Delete identities
  flows: []
  scope: identities:delete
- description: Read ingestion state and quota
  flows: []
  scope: ingestion:read
- description: Update ingestion state
  flows: []
  scope: ingestion:update
- description: Upload content for ingestion (ai/audio/chat/document/email/video)
  flows: []
  scope: ingestion:upload
- description: Read integrations
  flows: []
  scope: integrations:read
- description: Read labels
  flows: []
  scope: labels:read
- description: Create labels
  flows: []
  scope: labels:create
- description: Update labels
  flows: []
  scope: labels:update
- description: Delete labels
  flows: []
  scope: labels:delete
- description: Apply labels to records
  flows: []
  scope: labels:use
- description: Read legal holds
  flows: []
  scope: legal_hold:read
- description: Create legal holds
  flows: []
  scope: legal_hold:create
- description: Update legal holds
  flows: []
  scope: legal_hold:update
- description: Delete legal holds
  flows: []
  scope: legal_hold:delete
- description: Read legal matters
  flows: []
  scope: legal_matter:read
- description: Create legal matters
  flows: []
  scope: legal_matter:create
- description: Update legal matters
  flows: []
  scope: legal_matter:update
- description: Delete legal matters
  flows: []
  scope: legal_matter:delete
- description: Read organizational units
  flows: []
  scope: org_units:read
- description: Update organizational units
  flows: []
  scope: org_units:update
- description: Read reconciliation data
  flows: []
  scope: reconciliation:read
- description: Read records
  flows: []
  scope: records:read
- description: Read retention libraries
  flows: []
  scope: retention_libraries:read
- description: Create retention libraries
  flows: []
  scope: retention_libraries:create
- description: Update retention libraries
  flows: []
  scope: retention_libraries:update
- description: Delete retention libraries
  flows: []
  scope: retention_libraries:delete
- description: Read roles
  flows: []
  scope: roles:read
- description: Create roles
  flows: []
  scope: roles:create
- description: Update roles
  flows: []
  scope: roles:update
- description: Delete roles
  flows: []
  scope: roles:delete
- description: Read/run searches
  flows: []
  scope: search:read
- description: Create saved searches
  flows: []
  scope: search:create
- description: Export search results
  flows: []
  scope: search:export
- description: Reset and re-enter a saved search
  flows: []
  scope: search:reset
- description: Read storage accounts
  flows: []
  scope: storage_accounts:read
- description: Read supervision spaces
  flows: []
  scope: supervision_spaces:read
- description: Create supervision spaces
  flows: []
  scope: supervision_spaces:create
- description: Update supervision spaces
  flows: []
  scope: supervision_spaces:update
- description: Delete supervision spaces
  flows: []
  scope: supervision_spaces:delete
- description: Read user groups
  flows: []
  scope: user_groups:read
- description: Create user groups
  flows: []
  scope: user_groups:create
- description: Update user groups
  flows: []
  scope: user_groups:update
- description: Delete user groups
  flows: []
  scope: user_groups:delete
- description: Read users
  flows: []
  scope: users:read
- description: Create users
  flows: []
  scope: users:create
- description: Update users
  flows: []
  scope: users:update
- description: Delete users
  flows: []
  scope: users:delete
- description: Disable/enable users
  flows: []
  scope: users:disable
- description: Read workflows
  flows: []
  scope: workflows:read
- description: Run/queue workflows
  flows: []
  scope: workflows:use
- description: Read workspace
  flows: []
  scope: workspace:read
- description: Update workspace
  flows: []
  scope: workspace:update
slug: theta-lake-scopes
source_filename: theta-lake-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/theta-lake-openapi-original.yml\ndocs: https://developer.thetalake.ai/\nnotes: >-\n  The OpenAPI oauth2 clientCredentials flow declares an empty scopes map, but every operation\n  documents a REQUIRED PERMISSION (e.g. `users:read`) in its description, and the /token/context\n  response returns the granted permissions[] for an access token. These permissions are the\n  effective OAuth2/JWT scope surface, harvested from the operation descriptions across the spec.\nschemes:\n- name: ClientCredentials\n  type: oauth2\n  source: openapi/theta-lake-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.thetalake.ai/api/v1/token\nscope_convention: \"<resource>:<action>  (action in read|create|update|delete|use|upload|export|reset|disable)\"\nscopes:\n- {scope: 'audit_logs:read', description: Read audit logs}\n- {scope: 'comments:read', description: Read record comments}\n- {scope: 'comments:create',\
  \ description: Create record comments}\n- {scope: 'comments:update', description: Update record comments}\n- {scope: 'comments:delete', description: Delete record comments}\n- {scope: 'cases:read', description: Read cases}\n- {scope: 'cases:create', description: Create cases}\n- {scope: 'cases:update', description: Update cases}\n- {scope: 'cases:add_records', description: Add records to a case}\n- {scope: 'cases:remove_records', description: Remove records from a case}\n- {scope: 'directory_groups:read', description: Read directory groups}\n- {scope: 'directory_groups:create', description: Create directory groups}\n- {scope: 'directory_groups:update', description: Update directory groups}\n- {scope: 'directory_groups:delete', description: Delete directory groups}\n- {scope: 'exports:read', description: Read exports}\n- {scope: 'identities:read', description: Read identities}\n- {scope: 'identities:create', description: Create identities}\n- {scope: 'identities:update', description: Update\
  \ identities}\n- {scope: 'identities:delete', description: Delete identities}\n- {scope: 'ingestion:read', description: Read ingestion state and quota}\n- {scope: 'ingestion:update', description: Update ingestion state}\n- {scope: 'ingestion:upload', description: Upload content for ingestion (ai/audio/chat/document/email/video)}\n- {scope: 'integrations:read', description: Read integrations}\n- {scope: 'labels:read', description: Read labels}\n- {scope: 'labels:create', description: Create labels}\n- {scope: 'labels:update', description: Update labels}\n- {scope: 'labels:delete', description: Delete labels}\n- {scope: 'labels:use', description: Apply labels to records}\n- {scope: 'legal_hold:read', description: Read legal holds}\n- {scope: 'legal_hold:create', description: Create legal holds}\n- {scope: 'legal_hold:update', description: Update legal holds}\n- {scope: 'legal_hold:delete', description: Delete legal holds}\n- {scope: 'legal_matter:read', description: Read legal matters}\n\
  - {scope: 'legal_matter:create', description: Create legal matters}\n- {scope: 'legal_matter:update', description: Update legal matters}\n- {scope: 'legal_matter:delete', description: Delete legal matters}\n- {scope: 'org_units:read', description: Read organizational units}\n- {scope: 'org_units:update', description: Update organizational units}\n- {scope: 'reconciliation:read', description: Read reconciliation data}\n- {scope: 'records:read', description: Read records}\n- {scope: 'retention_libraries:read', description: Read retention libraries}\n- {scope: 'retention_libraries:create', description: Create retention libraries}\n- {scope: 'retention_libraries:update', description: Update retention libraries}\n- {scope: 'retention_libraries:delete', description: Delete retention libraries}\n- {scope: 'roles:read', description: Read roles}\n- {scope: 'roles:create', description: Create roles}\n- {scope: 'roles:update', description: Update roles}\n- {scope: 'roles:delete', description: Delete\
  \ roles}\n- {scope: 'search:read', description: Read/run searches}\n- {scope: 'search:create', description: Create saved searches}\n- {scope: 'search:export', description: Export search results}\n- {scope: 'search:reset', description: Reset and re-enter a saved search}\n- {scope: 'storage_accounts:read', description: Read storage accounts}\n- {scope: 'supervision_spaces:read', description: Read supervision spaces}\n- {scope: 'supervision_spaces:create', description: Create supervision spaces}\n- {scope: 'supervision_spaces:update', description: Update supervision spaces}\n- {scope: 'supervision_spaces:delete', description: Delete supervision spaces}\n- {scope: 'user_groups:read', description: Read user groups}\n- {scope: 'user_groups:create', description: Create user groups}\n- {scope: 'user_groups:update', description: Update user groups}\n- {scope: 'user_groups:delete', description: Delete user groups}\n- {scope: 'users:read', description: Read users}\n- {scope: 'users:create', description:\
  \ Create users}\n- {scope: 'users:update', description: Update users}\n- {scope: 'users:delete', description: Delete users}\n- {scope: 'users:disable', description: Disable/enable users}\n- {scope: 'workflows:read', description: Read workflows}\n- {scope: 'workflows:use', description: Run/queue workflows}\n- {scope: 'workspace:read', description: Read workspace}\n- {scope: 'workspace:update', description: Update workspace}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theta-lake/refs/heads/main/scopes/theta-lake-scopes.yml
summary_line: 70 scopes · clientCredentials
tags:
- Communications Governance
- Compliance
- Archiving
- Security
- Supervision
- eDiscovery
- Legal Hold
- Records Management
- Unified Communications
- AI Governance
- Regulatory Compliance
token_urls:
- https://developer.thetalake.ai/api/v1/token
---
