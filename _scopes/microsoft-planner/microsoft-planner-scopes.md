---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Planner Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Planner publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Planner API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schemes:
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-planner-openapi.yml
scope_count: 6
scope_names:
- Group.Read.All
- Group.ReadWrite.All
- Tasks.Read
- Tasks.Read.All
- Tasks.ReadWrite
- Tasks.ReadWrite.All
scopes:
- description: Read all groups
  flows:
  - authorizationCode
  scope: Group.Read.All
- description: Read and write all groups
  flows:
  - authorizationCode
  scope: Group.ReadWrite.All
- description: Read user Planner tasks
  flows:
  - authorizationCode
  scope: Tasks.Read
- description: Read all Planner tasks (admin)
  flows:
  - authorizationCode
  scope: Tasks.Read.All
- description: Read and write user Planner tasks
  flows:
  - authorizationCode
  scope: Tasks.ReadWrite
- description: Read and write all Planner tasks (admin)
  flows:
  - authorizationCode
  scope: Tasks.ReadWrite.All
slug: microsoft-planner-scopes
source_filename: microsoft-planner-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-planner-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-planner-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization with Microsoft identity platform\nscopes:\n- scope: Group.Read.All\n  description: Read all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-planner-openapi.yml\n- scope: Group.ReadWrite.All\n  description: Read and write all groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-planner-openapi.yml\n- scope: Tasks.Read\n  description: Read user Planner tasks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-planner-openapi.yml\n- scope: Tasks.Read.All\n  description: Read all Planner tasks (admin)\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/microsoft-planner-openapi.yml\n- scope: Tasks.ReadWrite\n  description: Read and write user Planner tasks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-planner-openapi.yml\n- scope: Tasks.ReadWrite.All\n  description: Read and write all Planner tasks (admin)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-planner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/scopes/microsoft-planner-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
