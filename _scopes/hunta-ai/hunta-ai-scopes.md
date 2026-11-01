---
api_specs:
- filename: hunta-ai-admin-api-openapi.yml
  format: yaml
  label: hunta-ai Admin API
  slug: hunta-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-admin-api-openapi.yml
- filename: hunta-ai-candidates-api-openapi.yml
  format: yaml
  label: hunta-ai Candidates API
  slug: hunta-ai-candidates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-candidates-api-openapi.yml
- filename: hunta-ai-errata-api-openapi.yml
  format: yaml
  label: hunta-ai Errata API
  slug: hunta-ai-errata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-errata-api-openapi.yml
- filename: hunta-ai-export-api-openapi.yml
  format: yaml
  label: hunta-ai Export API
  slug: hunta-ai-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-export-api-openapi.yml
- filename: hunta-ai-facts-api-openapi.yml
  format: yaml
  label: hunta-ai Facts API
  slug: hunta-ai-facts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-facts-api-openapi.yml
- filename: hunta-ai-memories-api-openapi.yml
  format: yaml
  label: hunta-ai Memories API
  slug: hunta-ai-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-memories-api-openapi.yml
- filename: hunta-ai-metrics-api-openapi.yml
  format: yaml
  label: hunta-ai Metrics API
  slug: hunta-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-metrics-api-openapi.yml
- filename: hunta-ai-reckon-api-openapi.yml
  format: yaml
  label: hunta-ai Reckon API
  slug: hunta-ai-reckon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-reckon-api-openapi.yml
- filename: hunta-ai-reconcile-api-openapi.yml
  format: yaml
  label: hunta-ai Reconcile API
  slug: hunta-ai-reconcile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-reconcile-api-openapi.yml
- filename: hunta-ai-whoami-api-openapi.yml
  format: yaml
  label: hunta-ai Whoami API
  slug: hunta-ai-whoami-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunta-ai/openapi/hunta-ai-whoami-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Hunta Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'hunta-ai publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the hunta-ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: hunta-ai
provider_slug: hunta-ai
schemes: []
scope_count: 4
scope_names:
- memory:write
- memory:capture
- memory:read
- memory:curate
scopes:
- description: Write canon directly via POST /v1/memories
  flows: []
  scope: memory:write
- description: Propose memory via POST /v1/memories/capture
  flows: []
  scope: memory:capture
- description: Read memories and facts via GET endpoints and POST /v1/memories/search
  flows: []
  scope: memory:read
- description: Supersede or invalidate facts via POST /v1/facts/{id}/supersede or invalidate
  flows: []
  scope: memory:curate
slug: hunta-ai-scopes
source_filename: hunta-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.hunta.ai/docs/api\nscopes:\n  - name: memory:write\n    description: \"Write canon directly via POST /v1/memories\"\n  - name: memory:capture\n    description: \"Propose memory via POST /v1/memories/capture\"\n  - name: memory:read\n    description: \"Read memories and facts via GET endpoints and POST /v1/memories/search\"\n  - name: memory:curate\n    description: \"Supersede or invalidate facts via POST /v1/facts/{id}/supersede or invalidate\"\n"
source_yaml_url: https://artifacts.apis.io/hunta-ai/scopes/hunta-ai-scopes.yml
summary_line: 4 scopes
tags:
- Company
- AI
- Memory
- API
- MCP
- Attestable
token_bound: false
token_urls: []
---
