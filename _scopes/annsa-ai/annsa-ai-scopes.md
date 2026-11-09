---
api_specs:
- filename: annsa-ai-agents-api-openapi.yml
  format: yaml
  label: Annsa Agents API
  slug: annsa-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-agents-api-openapi.yml
- filename: annsa-ai-ingest-api-openapi.yml
  format: yaml
  label: Annsa Ingest API
  slug: annsa-ai-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-ingest-api-openapi.yml
- filename: annsa-ai-service-api-openapi.yml
  format: yaml
  label: Annsa Service API
  slug: annsa-ai-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-service-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Annsa Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Annsa publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Annsa API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Annsa
provider_slug: annsa-ai
schemes: []
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read priorities, specs, survey results and search.
  flows: []
  scope: read
- description: Change state — start building, mark shipped, share back with customers.
  flows: []
  scope: write
slug: annsa-ai-scopes
source_filename: annsa-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: \"https://annsa.ai/openapi.json\"\nscopes:\n  - name: read\n    description: \"Read priorities, specs, survey results and search.\"\n  - name: write\n    description: \"Change state — start building, mark shipped, share back with customers.\"\n"
source_yaml_url: https://artifacts.apis.io/annsa-ai/scopes/annsa-ai-scopes.yml
summary_line: 2 scopes
tags:
- Project Management
- Customer Management
- Agent Teams
- Artificial Intelligence
- Software-as-a-Service
token_bound: false
token_urls: []
---
