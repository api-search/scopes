---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Tasks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Tasks publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Tasks API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Tasks
provider_slug: google-tasks
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/tasks.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/tasks
- https://www.googleapis.com/auth/tasks.readonly
scopes:
- description: Create, edit, organize, and delete all your tasks
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/tasks
- description: View your tasks
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/tasks.readonly
slug: google-tasks-scopes
source_filename: google-tasks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tasks.yml\nschemes:\n- name: oauth2\n  source: openapi/tasks.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/tasks\n  description: Create, edit, organize, and delete all your tasks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tasks.yml\n- scope: https://www.googleapis.com/auth/tasks.readonly\n  description: View your tasks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tasks.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-tasks/refs/heads/main/scopes/google-tasks-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Google
- Productivity
- Task Management
- Tasks
- Todo
- Workspace
token_urls:
- https://oauth2.googleapis.com/token
---
