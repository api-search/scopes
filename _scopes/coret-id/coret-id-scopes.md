---
authorization_urls: []
description: ''
docs: https://coret.id/api/v1/SKILL.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: coret.id Scopes
name_suffix: OAuth Scopes
note: Scopes are attached to each API key; old dashboard keys do not gain new scopes automatically. There is no folders:* scope — folders use maps:* and share:write. OAuth connectors request the full scope set.
overview: 'coret.id publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the coret.id API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: coret.id
provider_slug: coret-id
schemes: []
scope_count: 10
scope_names:
- maps:read
- maps:write
- nodes:read
- nodes:write
- workspace:read
- share:write
- pad:read
- pad:write
- book:read
- book:write
scopes:
- description: Read maps
  flows: []
  scope: maps:read
- description: Create
  flows: []
  scope: maps:write
- description: Read nodes in a mind map
  flows: []
  scope: nodes:read
- description: Write nodes
  flows: []
  scope: nodes:write
- description: Read workspace information
  flows: []
  scope: workspace:read
- description: Create
  flows: []
  scope: share:write
- description: 'Read Pad boards: tasks, worklog, blockers and change feed'
  flows: []
  scope: pad:read
- description: Claim tasks
  flows: []
  scope: pad:write
- description: Read Books and their pages
  flows: []
  scope: book:read
- description: Create Books and add/update pages via Markdown
  flows: []
  scope: book:write
slug: coret-id-scopes
source_filename: coret-id-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'generated: ''2026-11-04''

  method: searched

  source: https://coret.id/api/v1/SKILL.md

  docs: https://coret.id/api/v1/SKILL.md

  note: Scopes are attached to each API key; old dashboard keys do not gain new scopes automatically. There is no folders:* scope — folders use maps:* and share:write. OAuth connectors request the full scope set.

  scopes:

  - {name: ''maps:read'', description: Read maps, folders, connectors, Spidol drawings, sketch, video presets, version history and export}

  - {name: ''maps:write'', description: Create, update, delete maps and folders, move maps between folders, write drawings, sketch and video presets}

  - {name: ''nodes:read'', description: Read nodes in a mind map}

  - {name: ''nodes:write'', description: Write nodes, connectors and node image uploads}

  - {name: ''workspace:read'', description: Read workspace information}

  - {name: ''share:write'', description: Create, list and revoke share links, and manage folder access}

  - {name: ''pad:read'', description: ''Read Pad boards: tasks, worklog, blockers and change feed''}

  - {name: ''pad:write'', description: Claim tasks, report, heartbeat, complete, block and create tasks}

  - {name: ''book:read'', description: Read Books and their pages}

  - {name: ''book:write'', description: Create Books and add/update pages via Markdown}

  '
source_yaml_url: https://artifacts.apis.io/coret-id/scopes/coret-id-scopes.yml
summary_line: 10 scopes
tags:
- Company
- Mind Mapping
- Collaboration
- Productivity
- AI Agents
- MCP
- Indonesia
token_bound: false
token_urls: []
---
