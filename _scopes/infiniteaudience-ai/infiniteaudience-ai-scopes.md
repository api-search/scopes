---
api_specs:
- filename: infiniteaudience-ai-a2a-api-openapi.yml
  format: yaml
  label: Infinite Audience A2A API
  slug: infiniteaudience-ai-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-a2a-api-openapi.yml
- filename: infiniteaudience-ai-account-api-openapi.yml
  format: yaml
  label: Infinite Audience Account API
  slug: infiniteaudience-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-account-api-openapi.yml
- filename: infiniteaudience-ai-audiences-api-openapi.yml
  format: yaml
  label: Infinite Audience Audiences API
  slug: infiniteaudience-ai-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-audiences-api-openapi.yml
- filename: infiniteaudience-ai-auth-api-openapi.yml
  format: yaml
  label: Infinite Audience Auth API
  slug: infiniteaudience-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-auth-api-openapi.yml
- filename: infiniteaudience-ai-campaigns-api-openapi.yml
  format: yaml
  label: Infinite Audience Campaigns API
  slug: infiniteaudience-ai-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-campaigns-api-openapi.yml
- filename: infiniteaudience-ai-deliveries-api-openapi.yml
  format: yaml
  label: Infinite Audience Deliveries API
  slug: infiniteaudience-ai-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-deliveries-api-openapi.yml
- filename: infiniteaudience-ai-discovery-api-openapi.yml
  format: yaml
  label: Infinite Audience Discovery API
  slug: infiniteaudience-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-discovery-api-openapi.yml
- filename: infiniteaudience-ai-enrichment-api-openapi.yml
  format: yaml
  label: Infinite Audience Enrichment API
  slug: infiniteaudience-ai-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-enrichment-api-openapi.yml
- filename: infiniteaudience-ai-integrations-api-openapi.yml
  format: yaml
  label: Infinite Audience Integrations API
  slug: infiniteaudience-ai-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-integrations-api-openapi.yml
- filename: infiniteaudience-ai-mcp-api-openapi.yml
  format: yaml
  label: Infinite Audience MCP API
  slug: infiniteaudience-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-mcp-api-openapi.yml
- filename: infiniteaudience-ai-oauth-api-openapi.yml
  format: yaml
  label: Infinite Audience OAuth API
  slug: infiniteaudience-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-oauth-api-openapi.yml
- filename: infiniteaudience-ai-partnerships-api-openapi.yml
  format: yaml
  label: Infinite Audience Partnerships API
  slug: infiniteaudience-ai-partnerships-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-partnerships-api-openapi.yml
- filename: infiniteaudience-ai-segments-api-openapi.yml
  format: yaml
  label: Infinite Audience Segments API
  slug: infiniteaudience-ai-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-segments-api-openapi.yml
- filename: infiniteaudience-ai-settings-api-openapi.yml
  format: yaml
  label: Infinite Audience Settings API
  slug: infiniteaudience-ai-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-settings-api-openapi.yml
- filename: infiniteaudience-ai-triggers-api-openapi.yml
  format: yaml
  label: Infinite Audience Triggers API
  slug: infiniteaudience-ai-triggers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-triggers-api-openapi.yml
- filename: infiniteaudience-ai-webhooks-api-openapi.yml
  format: yaml
  label: Infinite Audience Webhooks API
  slug: infiniteaudience-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-webhooks-api-openapi.yml
- filename: infiniteaudience-ai-workflows-api-openapi.yml
  format: yaml
  label: Infinite Audience Workflows API
  slug: infiniteaudience-ai-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteaudience-ai/openapi/infiniteaudience-ai-workflows-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Infiniteaudience Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Infinite Audience publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Infinite Audience API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Infinite Audience
provider_slug: infiniteaudience-ai
schemes: []
scope_count: 4
scope_names:
- discovery
- creator
- account-read
- account
scopes:
- description: Explore catalogs, counts and status; some queries refresh cached state. Does not purchase records.
  flows: []
  scope: discovery
- description: Create or change segments/audiences, match records and deliver results; execution can incur usage.
  flows: []
  scope: creator
- description: Read account usage, balance and existing top-up status through MCP/A2A and supported account endpoints; cannot purchase or change terms.
  flows: []
  scope: account-read
- description: Trusted account management; role restrictions also apply. Not available through delegated OAuth.
  flows: []
  scope: account
slug: infiniteaudience-ai-scopes
source_filename: infiniteaudience-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://docs.infiniteaudience.ai/auth/scopes/\nscopes:\n  - name: discovery\n    description: Explore catalogs, counts and status; some queries refresh cached state. Does not purchase records.\n    required: true\n  - name: creator\n    description: Create or change segments/audiences, match records and deliver results; execution can incur usage.\n    required: true\n  - name: account-read\n    description: Read account usage, balance and existing top-up status through MCP/A2A and supported account endpoints; cannot purchase or change terms.\n    required: true\n  - name: account\n    description: Trusted account management; role restrictions also apply. Not available through delegated OAuth.\n    required: false\n"
source_yaml_url: https://artifacts.apis.io/infiniteaudience-ai/scopes/infiniteaudience-ai-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Identity Resolution
- Data Enrichment
- Audiences
- Marketing
- MCP
- A2A
token_bound: false
token_urls: []
---
