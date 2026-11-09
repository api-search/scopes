---
api_specs:
- filename: animam-ai-corpus-api-openapi.yml
  format: yaml
  label: Animam.ai Corpus API
  slug: animam-ai-corpus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animam-ai/openapi/animam-ai-corpus-api-openapi.yml
- filename: animam-ai-segments-api-openapi.yml
  format: yaml
  label: Animam.ai Segments API
  slug: animam-ai-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animam-ai/openapi/animam-ai-segments-api-openapi.yml
- filename: animam-ai-tenants-api-openapi.yml
  format: yaml
  label: Animam.ai Tenants API
  slug: animam-ai-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animam-ai/openapi/animam-ai-tenants-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Animam Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Animam.ai publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Animam.ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Animam.ai
provider_slug: animam-ai
schemes: []
scope_count: 7
scope_names:
- corpus:read
- corpus:write
- segments:read
- segments:write
- settings:read
- settings:write
- stats:read
scopes:
- description: Read knowledge base entries
  flows: []
  scope: corpus:read
- description: Create / update / delete knowledge base entries
  flows: []
  scope: corpus:write
- description: Read segments
  flows: []
  scope: segments:read
- description: Create / update segments
  flows: []
  scope: segments:write
- description: Read tenant settings
  flows: []
  scope: settings:read
- description: Update tenant settings
  flows: []
  scope: settings:write
- description: Read analytics and usage data
  flows: []
  scope: stats:read
slug: animam-ai-scopes
source_filename: animam-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://api.animam.ai/openapi.json\nscopes:\n  - name: corpus:read\n    description: \"Read knowledge base entries\"\n  - name: corpus:write\n    description: \"Create / update / delete knowledge base entries\"\n  - name: segments:read\n    description: \"Read segments\"\n  - name: segments:write\n    description: \"Create / update segments\"\n  - name: settings:read\n    description: \"Read tenant settings\"\n  - name: settings:write\n    description: \"Update tenant settings\"\n  - name: stats:read\n    description: \"Read analytics and usage data\"\n"
source_yaml_url: https://artifacts.apis.io/animam-ai/scopes/animam-ai-scopes.yml
summary_line: 7 scopes
tags:
- Artificial Intelligence
- Automation
- Lead Generation
- Chatbots
- Software-as-a-Service
token_bound: false
token_urls: []
---
