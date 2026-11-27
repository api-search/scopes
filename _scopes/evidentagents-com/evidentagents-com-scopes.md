---
api_specs:
- filename: evidentagents-com-demands-api-openapi.yml
  format: yaml
  label: Evident Demands API
  slug: evidentagents-com-demands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-demands-api-openapi.yml
- filename: evidentagents-com-personal-api-openapi.yml
  format: yaml
  label: Evident Personal API
  slug: evidentagents-com-personal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-personal-api-openapi.yml
- filename: evidentagents-com-quality-api-openapi.yml
  format: yaml
  label: Evident Quality API
  slug: evidentagents-com-quality-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-quality-api-openapi.yml
- filename: evidentagents-com-service-config-api-openapi.yml
  format: yaml
  label: Evident Service Config API
  slug: evidentagents-com-service-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-service-config-api-openapi.yml
- filename: evidentagents-com-service-feedback-api-openapi.yml
  format: yaml
  label: Evident Service Feedback API
  slug: evidentagents-com-service-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-service-feedback-api-openapi.yml
- filename: evidentagents-com-services-api-openapi.yml
  format: yaml
  label: Evident Services API
  slug: evidentagents-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-services-api-openapi.yml
- filename: evidentagents-com-task-benchmarks-api-openapi.yml
  format: yaml
  label: Evident Task Benchmarks API
  slug: evidentagents-com-task-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-task-benchmarks-api-openapi.yml
- filename: evidentagents-com-task-canaries-api-openapi.yml
  format: yaml
  label: Evident Task Canaries API
  slug: evidentagents-com-task-canaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-task-canaries-api-openapi.yml
- filename: evidentagents-com-task-candidates-api-openapi.yml
  format: yaml
  label: Evident Task Candidates API
  slug: evidentagents-com-task-candidates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-task-candidates-api-openapi.yml
- filename: evidentagents-com-task-contract-api-openapi.yml
  format: yaml
  label: Evident Task Contract API
  slug: evidentagents-com-task-contract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-task-contract-api-openapi.yml
- filename: evidentagents-com-task-execute-api-openapi.yml
  format: yaml
  label: Evident Task Execute API
  slug: evidentagents-com-task-execute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-task-execute-api-openapi.yml
- filename: evidentagents-com-task-match-api-openapi.yml
  format: yaml
  label: Evident Task Match API
  slug: evidentagents-com-task-match-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-task-match-api-openapi.yml
- filename: evidentagents-com-task-plan-api-openapi.yml
  format: yaml
  label: Evident Task Plan API
  slug: evidentagents-com-task-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-task-plan-api-openapi.yml
- filename: evidentagents-com-task-schema-api-openapi.yml
  format: yaml
  label: Evident Task Schema API
  slug: evidentagents-com-task-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-task-schema-api-openapi.yml
- filename: evidentagents-com-workspace-api-openapi.yml
  format: yaml
  label: Evident Workspace API
  slug: evidentagents-com-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidentagents-com/openapi/evidentagents-com-workspace-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Evident Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Evident publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Evident API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Evident
provider_slug: evidentagents-com
schemes: []
scope_count: 3
scope_names:
- review:prepare
- review:submit
- merchant:reply
scopes:
- description: Token for preparing a review (1 hour)
  flows: []
  scope: review:prepare
- description: Token for submitting a review (1 hour)
  flows: []
  scope: review:submit
- description: Token for merchant reply (24 hours)
  flows: []
  scope: merchant:reply
slug: evidentagents-com-scopes
source_filename: evidentagents-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/evidentagents-com-openapi.json\nscopes:\n  - name: review:prepare\n    description: Token for preparing a review (1 hour)\n  - name: review:submit\n    description: Token for submitting a review (1 hour)\n  - name: merchant:reply\n    description: Token for merchant reply (24 hours)\n"
source_yaml_url: https://artifacts.apis.io/evidentagents-com/scopes/evidentagents-com-scopes.yml
summary_line: 3 scopes
tags:
- Artificial Intelligence
- Agents
- Tools
- Marketplace
- Search
token_bound: false
token_urls: []
---
