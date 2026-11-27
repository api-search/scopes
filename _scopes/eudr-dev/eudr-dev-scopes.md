---
api_specs:
- filename: eudr-dev-a2a-api-openapi.yml
  format: yaml
  label: eudr.dev A2a API
  slug: eudr-dev-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-a2a-api-openapi.yml
- filename: eudr-dev-agent-api-openapi.yml
  format: yaml
  label: eudr.dev Agent API
  slug: eudr-dev-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-agent-api-openapi.yml
- filename: eudr-dev-discovery-api-openapi.yml
  format: yaml
  label: eudr.dev Discovery API
  slug: eudr-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-discovery-api-openapi.yml
- filename: eudr-dev-engineer-api-openapi.yml
  format: yaml
  label: eudr.dev Engineer API
  slug: eudr-dev-engineer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-engineer-api-openapi.yml
- filename: eudr-dev-ops-api-openapi.yml
  format: yaml
  label: eudr.dev Ops API
  slug: eudr-dev-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-ops-api-openapi.yml
- filename: eudr-dev-public-api-openapi.yml
  format: yaml
  label: eudr.dev Public API
  slug: eudr-dev-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-public-api-openapi.yml
- filename: eudr-dev-reference-api-openapi.yml
  format: yaml
  label: eudr.dev Reference API
  slug: eudr-dev-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-reference-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: eudr.dev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'eudr.dev publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the eudr.dev API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: eudr.dev
provider_slug: eudr-dev
schemes: []
scope_count: 2
scope_names:
- eudr:read
- eudr:write
scopes:
- description: read the organisation's records
  flows: []
  scope: eudr:read
- description: compile and sign statements
  flows: []
  scope: eudr:write
slug: eudr-dev-scopes
source_filename: eudr-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: https://eudr.dev/openapi.json\nscopes:\n  - name: eudr:read\n    description: \"read the organisation's records\"\n  - name: eudr:write\n    description: \"compile and sign statements\"\n"
source_yaml_url: https://artifacts.apis.io/eudr-dev/scopes/eudr-dev-scopes.yml
summary_line: 2 scopes
tags:
- EU Deforestation
- Compliance
- Agriculture
- Artificial Intelligence
- Environmental
token_bound: false
token_urls: []
---
