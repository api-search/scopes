---
api_specs:
- filename: clment-com-collaborators-api-openapi.yml
  format: yaml
  label: Clment Collaborators API
  slug: clment-com-collaborators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-collaborators-api-openapi.yml
- filename: clment-com-contracts-api-openapi.yml
  format: yaml
  label: Clment Contracts API
  slug: clment-com-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-contracts-api-openapi.yml
- filename: clment-com-conversion-api-openapi.yml
  format: yaml
  label: Clment Conversion API
  slug: clment-com-conversion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-conversion-api-openapi.yml
- filename: clment-com-insights-api-openapi.yml
  format: yaml
  label: Clment Insights API
  slug: clment-com-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-insights-api-openapi.yml
- filename: clment-com-jobs-api-openapi.yml
  format: yaml
  label: Clment Jobs API
  slug: clment-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-jobs-api-openapi.yml
- filename: clment-com-key-dates-api-openapi.yml
  format: yaml
  label: Clment Key dates API
  slug: clment-com-key-dates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-key-dates-api-openapi.yml
- filename: clment-com-reviews-api-openapi.yml
  format: yaml
  label: Clment Reviews API
  slug: clment-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-reviews-api-openapi.yml
- filename: clment-com-rulebooks-api-openapi.yml
  format: yaml
  label: Clment Rulebooks API
  slug: clment-com-rulebooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-rulebooks-api-openapi.yml
- filename: clment-com-search-api-openapi.yml
  format: yaml
  label: Clment Search API
  slug: clment-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-search-api-openapi.yml
- filename: clment-com-taxonomy-api-openapi.yml
  format: yaml
  label: Clment Taxonomy API
  slug: clment-com-taxonomy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-taxonomy-api-openapi.yml
- filename: clment-com-usage-api-openapi.yml
  format: yaml
  label: Clment Usage API
  slug: clment-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clment-com/openapi/clment-com-usage-api-openapi.yml
authorization_urls: []
description: ''
docs: https://clment.com/help/connecting-claude-desktop
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Clment Scopes
name_suffix: OAuth Scopes
note: Scopes apply to the OAuth 2.1 flow of the remote MCP server only; the REST API uses bearer API keys and declares no oauth2 scheme in the OpenAPI.
overview: 'Clment publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clment API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clment
provider_slug: clment-com
schemes: []
scope_count: 2
scope_names:
- read
- read_write
scopes:
- description: Read access to the authorized organization's workspace (as published on the developer hub; no further description given).
  flows: []
  scope: read
- description: Read and write access to the authorized organization's workspace (as published on the developer hub; no further description given).
  flows: []
  scope: read_write
slug: clment-com-scopes
source_filename: clment-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clment.com/developers\ndocs: https://clment.com/help/connecting-claude-desktop\nnote: Scopes apply to the OAuth 2.1 flow of the remote MCP server only; the REST API uses bearer API keys and declares no oauth2 scheme in the OpenAPI.\nscopes:\n- name: read\n  surface: mcp\n  description: Read access to the authorized organization's workspace (as published on the developer hub; no further description given).\n- name: read_write\n  surface: mcp\n  description: Read and write access to the authorized organization's workspace (as published on the developer hub; no further description given).\n"
source_yaml_url: https://artifacts.apis.io/clment-com/scopes/clment-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Contract Review
- Legal Tech
- Artificial Intelligence
- Contract Management
- Redlining
- MCP
- REST API
token_bound: false
token_urls: []
---
