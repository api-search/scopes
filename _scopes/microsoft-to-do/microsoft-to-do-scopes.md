---
api_specs:
- filename: microsoft-to-do-linkedresources-api-openapi.yml
  format: yaml
  label: Microsoft to Do LinkedResources API
  slug: microsoft-to-do-linkedresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-linkedresources-api-openapi.yml
- filename: microsoft-to-do-tasklists-api-openapi.yml
  format: yaml
  label: Microsoft to Do TaskLists API
  slug: microsoft-to-do-tasklists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-tasklists-api-openapi.yml
- filename: microsoft-to-do-tasks-api-openapi.yml
  format: yaml
  label: Microsoft to Do Tasks API
  slug: microsoft-to-do-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-tasks-api-openapi.yml
- filename: microsoft-to-do-me-todo-api-openapi.yml
  format: yaml
  label: Microsoft To Do Me.todo API
  slug: microsoft-to-do-me-todo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-me-todo-api-openapi.yml
- filename: microsoft-to-do-users-todo-api-openapi.yml
  format: yaml
  label: Microsoft To Do Users.todo API
  slug: microsoft-to-do-users-todo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-users-todo-api-openapi.yml
- filename: microsoft-to-do-checklist-items-api-openapi.yml
  format: yaml
  label: Microsoft To Do Checklist Items API
  slug: microsoft-to-do-checklist-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-checklist-items-api-openapi.yml
authorization_urls: []
description: ''
docs: https://learn.microsoft.com/en-us/graph/permissions-reference
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft To Do Scopes
name_suffix: OAuth Scopes
note: Microsoft Graph permissions governing todo, todoTaskList and todoTask resources (Microsoft identity platform OAuth 2.0). The Graph OpenAPI declares no securitySchemes; the scopes come from the permissions reference.
overview: 'Microsoft To Do publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft To Do API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft To Do
provider_slug: microsoft-to-do
schemes: []
scope_count: 6
scope_names:
- Tasks.Read
- Tasks.ReadWrite
- Tasks.Read.Shared
- Tasks.ReadWrite.Shared
- Tasks.Read.All
- Tasks.ReadWrite.All
scopes:
- description: ''
  flows: []
  scope: Tasks.Read
- description: ''
  flows: []
  scope: Tasks.ReadWrite
- description: ''
  flows: []
  scope: Tasks.Read.Shared
- description: ''
  flows: []
  scope: Tasks.ReadWrite.Shared
- description: ''
  flows: []
  scope: Tasks.Read.All
- description: ''
  flows: []
  scope: Tasks.ReadWrite.All
slug: microsoft-to-do-scopes
source_filename: microsoft-to-do-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'name: Microsoft To Do OAuth scopes

  generated: ''2026-11-04''

  method: searched

  source: https://learn.microsoft.com/en-us/graph/permissions-reference

  docs: https://learn.microsoft.com/en-us/graph/permissions-reference

  note: Microsoft Graph permissions governing todo, todoTaskList and todoTask resources (Microsoft identity platform OAuth 2.0). The Graph OpenAPI declares no securitySchemes; the scopes come from the permissions reference.

  scopes:

  - {name: Tasks.Read, type: delegated}

  - {name: Tasks.ReadWrite, type: delegated}

  - {name: Tasks.Read.Shared, type: delegated}

  - {name: Tasks.ReadWrite.Shared, type: delegated}

  - {name: Tasks.Read.All, type: application}

  - {name: Tasks.ReadWrite.All, type: application}

  '
source_yaml_url: https://artifacts.apis.io/microsoft-to-do/scopes/microsoft-to-do-scopes.yml
summary_line: 6 scopes
tags:
- Microsoft
- Microsoft 365
- Productivity
- Task
- Task Management
- Microsoft Graph
token_bound: false
token_urls: []
---
