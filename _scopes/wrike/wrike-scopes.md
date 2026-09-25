---
api_specs:
- filename: wrike-access-roles-api-openapi.yml
  format: yaml
  label: Wrike Access Roles API
  slug: wrike-access-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-access-roles-api-openapi.yml
- filename: wrike-accounts-api-openapi.yml
  format: yaml
  label: Wrike Accounts API
  slug: wrike-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-accounts-api-openapi.yml
- filename: wrike-colors-api-openapi.yml
  format: yaml
  label: Wrike Colors API
  slug: wrike-colors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-colors-api-openapi.yml
- filename: wrike-comments-api-openapi.yml
  format: yaml
  label: Wrike Comments API
  slug: wrike-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-comments-api-openapi.yml
- filename: wrike-contacts-api-openapi.yml
  format: yaml
  label: Wrike Contacts API
  slug: wrike-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-contacts-api-openapi.yml
- filename: wrike-custom-fields-api-openapi.yml
  format: yaml
  label: Wrike Custom Fields API
  slug: wrike-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-custom-fields-api-openapi.yml
- filename: wrike-folders-and-projects-api-openapi.yml
  format: yaml
  label: Wrike Folders And Projects API
  slug: wrike-folders-and-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-folders-and-projects-api-openapi.yml
- filename: wrike-groups-api-openapi.yml
  format: yaml
  label: Wrike Groups API
  slug: wrike-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-groups-api-openapi.yml
- filename: wrike-tasks-api-openapi.yml
  format: yaml
  label: Wrike Tasks API
  slug: wrike-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-tasks-api-openapi.yml
- filename: wrike-time-logs-api-openapi.yml
  format: yaml
  label: Wrike Time Logs API
  slug: wrike-time-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-time-logs-api-openapi.yml
- filename: wrike-users-api-openapi.yml
  format: yaml
  label: Wrike Users API
  slug: wrike-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-users-api-openapi.yml
- filename: wrike-webhooks-api-openapi.yml
  format: yaml
  label: Wrike Webhooks API
  slug: wrike-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-webhooks-api-openapi.yml
- filename: wrike-workflows-api-openapi.yml
  format: yaml
  label: Wrike Workflows API
  slug: wrike-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-workflows-api-openapi.yml
authorization_urls:
- https://www.wrike.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wrike Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wrike publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wrike API on a user''s behalf.


  Tokens are issued from https://www.wrike.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wrike
provider_slug: wrike
schemes:
- description: OAuth 2.0 authorization code flow
  flows:
  - authorizationUrl: https://www.wrike.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.wrike.com/oauth2/token
  name: oauth2
  source: openapi/wrike-openapi.yml
scope_count: 6
scope_names:
- Default
- amReadOnlyAccessRole
- amReadOnlyWorkflow
- amReadWriteWorkflow
- wsReadOnly
- wsReadWrite
scopes:
- description: Default access scope
  flows:
  - authorizationCode
  scope: Default
- description: Read-only access to access roles
  flows:
  - authorizationCode
  scope: amReadOnlyAccessRole
- description: Read-only access to workflows
  flows:
  - authorizationCode
  scope: amReadOnlyWorkflow
- description: Read-write access to workflows
  flows:
  - authorizationCode
  scope: amReadWriteWorkflow
- description: Read-only workspace access
  flows:
  - authorizationCode
  scope: wsReadOnly
- description: Read-write workspace access
  flows:
  - authorizationCode
  scope: wsReadWrite
slug: wrike-scopes
source_filename: wrike-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wrike-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/wrike-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wrike.com/oauth2/authorize\n    tokenUrl: https://www.wrike.com/oauth2/token\n  description: OAuth 2.0 authorization code flow\nscopes:\n- scope: Default\n  description: Default access scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wrike-openapi.yml\n- scope: amReadOnlyAccessRole\n  description: Read-only access to access roles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wrike-openapi.yml\n- scope: amReadOnlyWorkflow\n  description: Read-only access to workflows\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wrike-openapi.yml\n- scope: amReadWriteWorkflow\n  description: Read-write access to workflows\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wrike-openapi.yml\n- scope: wsReadOnly\n  description: Read-only workspace\
  \ access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wrike-openapi.yml\n- scope: wsReadWrite\n  description: Read-write workspace access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wrike-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/scopes/wrike-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Work Management
- Project Management
- Collaboration
- Productivity
- Workflow Automation
- Task Management
token_urls:
- https://www.wrike.com/oauth2/token
---
