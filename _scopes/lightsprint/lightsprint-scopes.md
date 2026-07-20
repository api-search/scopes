---
authorization_urls:
- https://lightsprint.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lightsprint Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lightsprint publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lightsprint API on a user''s behalf.


  Tokens are issued from https://lightsprint.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lightsprint
provider_slug: lightsprint
schemes:
- flows:
  - authorizationUrl: https://lightsprint.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://lightsprint.ai/oauth/token
  name: LightsprintOAuth2Api
  source: https://github.com/SprintsAI/n8n-nodes-lightsprint/blob/main/credentials/LightsprintOAuth2Api.credentials.ts
scope_count: 7
scope_names:
- tasks:read
- tasks:write
- kanban:read
- comments:write
- agents:write
- plans:read
- plans:write
scopes:
- description: Read tasks on the workspace board.
  flows:
  - authorizationCode
  scope: tasks:read
- description: Create, update, delete, and claim tasks.
  flows:
  - authorizationCode
  scope: tasks:write
- description: Read the kanban board structure — stacks, sections, and task ordering.
  flows:
  - authorizationCode
  scope: kanban:read
- description: Create, update, and delete comments on tasks.
  flows:
  - authorizationCode
  scope: comments:write
- description: Launch and stop cloud coding agents against a task.
  flows:
  - authorizationCode
  scope: agents:write
- description: Read generated plans (Plan Mode output).
  flows:
  - authorizationCode
  scope: plans:read
- description: Create and modify plans.
  flows:
  - authorizationCode
  scope: plans:write
slug: lightsprint-scopes
source_filename: lightsprint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/SprintsAI/n8n-nodes-lightsprint/blob/main/credentials/LightsprintOAuth2Api.credentials.ts\nnotes: >-\n  Scope strings are recorded verbatim from the default `scope` value in the\n  provider's published OAuth 2.0 credential definition. Lightsprint publishes no\n  scopes/permissions reference page, so the descriptions below are honest readings of\n  each scope's resource:action shape mapped to the API operations the n8n node calls\n  under that scope — they are not quoted provider prose.\ndocs: null\nschemes:\n- name: LightsprintOAuth2Api\n  source: https://github.com/SprintsAI/n8n-nodes-lightsprint/blob/main/credentials/LightsprintOAuth2Api.credentials.ts\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lightsprint.ai/oauth/authorize\n    tokenUrl: https://lightsprint.ai/oauth/token\nscopes:\n- scope: tasks:read\n  description: Read tasks on the workspace board.\n  flows: [authorizationCode]\n\
  \  observed_operations:\n  - 'GET /api/repos/{repoId}/tasks'\n  - 'GET /api/tasks/{taskId}'\n- scope: tasks:write\n  description: Create, update, delete, and claim tasks.\n  flows: [authorizationCode]\n  observed_operations:\n  - 'POST /api/repos/{repoId}/tasks'\n  - 'PATCH /api/tasks/{taskId}'\n  - 'DELETE /api/tasks/{taskId}'\n  - 'POST /api/tasks/{taskId}/claim'\n- scope: kanban:read\n  description: Read the kanban board structure — stacks, sections, and task ordering.\n  flows: [authorizationCode]\n  observed_operations: []\n- scope: comments:write\n  description: Create, update, and delete comments on tasks.\n  flows: [authorizationCode]\n  observed_operations:\n  - 'POST /api/tasks/{taskId}/comments'\n  - 'PATCH /api/comments/{commentId}'\n  - 'DELETE /api/comments/{commentId}'\n- scope: agents:write\n  description: Launch and stop cloud coding agents against a task.\n  flows: [authorizationCode]\n  observed_operations:\n  - 'POST /api/tasks/{taskId}/cloud-agents/{provider}'\n  -\
  \ 'DELETE /api/tasks/{taskId}/cloud-agents/{provider}'\n- scope: plans:read\n  description: Read generated plans (Plan Mode output).\n  flows: [authorizationCode]\n  observed_operations: []\n- scope: plans:write\n  description: Create and modify plans.\n  flows: [authorizationCode]\n  observed_operations: []\nobservations:\n- The published default scope set is granted as a single space-delimited string; no\n  incremental or per-operation scope negotiation is documented.\n- 'There is no `comments:read` scope in the default set even though the node reads\n  comments via GET /api/tasks/{taskId}/comments — reads there appear to be covered by\n  tasks:read.'\ngaps:\n- No public scopes/permissions reference page exists on lightsprint.ai; scopes are only\n  discoverable from the published n8n credential source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightsprint/refs/heads/main/scopes/lightsprint-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Developer Tools
- Artificial Intelligence
- Agents
- Software Development
- Project Management
- Code Generation
- Team Collaboration
token_urls:
- https://lightsprint.ai/oauth/token
---
