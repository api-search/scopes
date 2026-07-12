---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Reclaim Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Reclaim.ai publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Reclaim.ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Reclaim.ai
provider_slug: reclaim-ai
schemes:
- flows: []
  name: Authorization
  source: openapi/reclaim-ai-openapi.yml
scope_count: 3
scope_names:
- ROLE_API
- isAnonymous()
- isAuthenticated()
scopes:
- description: ''
  flows: []
  scope: ROLE_API
- description: ''
  flows: []
  scope: isAnonymous()
- description: ''
  flows: []
  scope: isAuthenticated()
slug: reclaim-ai-scopes
source_filename: reclaim-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reclaim-ai-openapi.yml\nschemes:\n- name: Authorization\n  source: openapi/reclaim-ai-openapi.yml\n  flows: []\nscopes:\n- scope: ROLE_API\n  sources:\n  - openapi/reclaim-ai-openapi.yml\n- scope: isAnonymous()\n  sources:\n  - openapi/reclaim-ai-openapi.yml\n- scope: isAuthenticated()\n  sources:\n  - openapi/reclaim-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reclaim-ai/refs/heads/main/scopes/reclaim-ai-scopes.yml
summary_line: 3 scopes
tags:
- AI
- Scheduling
- Calendar
- Productivity
- Tasks
- Habits
- Time Management
- Meetings
- Focus Time
token_urls: []
---
