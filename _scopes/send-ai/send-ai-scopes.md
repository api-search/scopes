---
api_specs:
- filename: send-ai-openapi-generated.yml
  format: yaml
  label: Send AI API
  slug: send-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/send-ai/openapi/_ae-authored/send-ai-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Send Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Send AI publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Send AI API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Send AI
provider_slug: send-ai
schemes: []
scope_count: 6
scope_names:
- upload.read
- upload.create
- upload.edit
- upload.delete
- task.read
- task.edit
scopes:
- description: Fetch and list uploads
  flows: []
  scope: upload.read
- description: Create an upload
  flows: []
  scope: upload.create
- description: Make changes to an upload
  flows: []
  scope: upload.edit
- description: Delete an upload
  flows: []
  scope: upload.delete
- description: Fetch and list tasks
  flows: []
  scope: task.read
- description: Manipulate tasks (unlock, complete, discard, report)
  flows: []
  scope: task.edit
slug: send-ai-scopes
source_filename: send-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.send.ai/api/scopes\nscopes:\n  - name: upload.read\n    description: \"Fetch and list uploads\"\n  - name: upload.create\n    description: \"Create an upload\"\n  - name: upload.edit\n    description: \"Make changes to an upload\"\n  - name: upload.delete\n    description: \"Delete an upload\"\n  - name: task.read\n    description: \"Fetch and list tasks\"\n  - name: task.edit\n    description: \"Manipulate tasks (unlock, complete, discard, report)\"\n"
source_yaml_url: https://artifacts.apis.io/send-ai/scopes/send-ai-scopes.yml
summary_line: 6 scopes
tags:
- Company
- AI
- Document Processing
- EDI
- Supply Chain
- Integration
token_bound: false
token_urls: []
---
