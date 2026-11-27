---
api_specs:
- filename: ezel-ai-openapi-generated.yml
  format: yaml
  label: Ezel API
  slug: ezel-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ezel-ai/openapi/_ae-authored/ezel-ai-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ezel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ezel publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ezel API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ezel
provider_slug: ezel-ai
schemes: []
scope_count: 2
scope_names:
- read
- write
scopes:
- description: 'Every query endpoint: whoami, usage, listing and reading matters and files, ask, search, case law, and reading review tables.'
  flows: []
  scope: read
- description: 'Mutations: create or delete a matter, upload or delete a file, and create or run a review table.'
  flows: []
  scope: write
slug: ezel-ai-scopes
source_filename: ezel-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://ezel.ai/docs#scopes\nscopes:\n  - name: read\n    description: \"Every query endpoint: whoami, usage, listing and reading matters and files, ask, search, case law, and reading review tables.\"\n  - name: write\n    description: \"Mutations: create or delete a matter, upload or delete a file, and create or run a review table.\"\n"
source_yaml_url: https://artifacts.apis.io/ezel-ai/scopes/ezel-ai-scopes.yml
summary_line: 2 scopes
tags:
- Artificial Intelligence
- Legal Tech
- Software-as-a-Service
- Platform
- Company
token_bound: false
token_urls: []
---
