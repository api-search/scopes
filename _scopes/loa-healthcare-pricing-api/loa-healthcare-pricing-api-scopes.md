---
api_specs:
- filename: loa-healthcare-pricing-api-entities-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Entities API
  slug: loa-healthcare-pricing-api-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-entities-api-openapi.yml
- filename: loa-healthcare-pricing-api-entity-analytics-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Entity Analytics API
  slug: loa-healthcare-pricing-api-entity-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-entity-analytics-api-openapi.yml
- filename: loa-healthcare-pricing-api-entity-updates-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Entity Updates API
  slug: loa-healthcare-pricing-api-entity-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-entity-updates-api-openapi.yml
- filename: loa-healthcare-pricing-api-prices-api-openapi.yml
  format: yaml
  label: Loa Healthcare Pricing API Prices API
  slug: loa-healthcare-pricing-api-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/openapi/loa-healthcare-pricing-api-prices-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.loacare.com/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Loa Healthcare Pricing Api Scopes
name_suffix: OAuth Scopes
note: OAuth applies to the MCP surface only; the REST OpenAPI declares a single optional apiKey scheme with no oauth2 flows (derive-oauth-scopes found no spec-declared scopes). Scopes below are the identity scopes the protected-resource metadata advertises — there are no resource-permission scopes; access tiers (authenticated / suggestions / linked provider) are enforced per-account, not per-scope.
overview: 'Loa Healthcare Pricing API uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Loa Healthcare Pricing API
provider_slug: loa-healthcare-pricing-api
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: loa-healthcare-pricing-api-scopes
source_filename: loa-healthcare-pricing-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://www.loacare.com/.well-known/oauth-protected-resource\ndocs: https://www.loacare.com/mcp\nnote: >-\n  OAuth applies to the MCP surface only; the REST OpenAPI declares a single optional apiKey scheme with\n  no oauth2 flows (derive-oauth-scopes found no spec-declared scopes). Scopes below are the identity\n  scopes the protected-resource metadata advertises — there are no resource-permission scopes; access\n  tiers (authenticated / suggestions / linked provider) are enforced per-account, not per-scope.\nauthorization_server: https://eknkfyyjqxuvgdzocccu.supabase.co/auth/v1\nscopes:\n  - name: openid\n    description: OpenID Connect authentication for MCP tool calls.\n  - name: email\n    description: Submitter email identity, used by reviewed update submissions.\n  - name: profile\n    description: Basic profile identity for linked-provider affiliation signals.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loa-healthcare-pricing-api/refs/heads/main/scopes/loa-healthcare-pricing-api-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Healthcare
- Price Transparency
- medical pricing
- Hospitals
- Providers
- Provider Directory
- hospital prices
- CPT
- HCPCS
- MCP
- agent-native
- OpenAPI
- llms-txt
token_urls: []
---
